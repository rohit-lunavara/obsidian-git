---
tags:
  - fleeting
---
# Field-Level Cohesion

```tsx
import { useForm } from "react-hook-form";

export function Form() {
  const {
    register,
    formState: { errors },
    handleSubmit
  } = useForm({
    defaultValues: {
      name: "",
      email: ""
    }
  });

  const onSubmit = handleSubmit((formData) => {
    // Form data submission logic
    console.log("Form submitted:", formData);
  });

  return (
    <form onSubmit={onSubmit}>
      <div>
        <input
          {...register("name", {
            validate: (value) =>
              isEmptyStringOrNil(value) ? "Please enter your name." : ""
          })}
          placeholder="Name"
        />
        {errors.name && <p>{errors.name.message}</p>}
      </div>

      <div>
        <input
          {...register("email", {
            validate: (value) => {
              if (isEmptyStringOrNil(value)) {
                return "Please enter your email.";
              }

              if (!/^[A-Z0-9._%+-]+@[A-Z0-9.-]+\.[A-Z]{2,}$/i.test(value)) {
                return "Please enter a valid email address.";
              }

              return "";
            }
          })}
          placeholder="Email"
        />
        {errors.email && <p>{errors.email.message}</p>}
      </div>

      <button type="submit">Submit</button>
    </form>
  );
}

function isNil(value: unknown): value is null | undefined {
  return value == null;
}

type NullableString = string | null | undefined;

function isEmptyStringOrNil(value: NullableString): boolean {
  return isNil(value) || value.trim() === "";
}
```

# Form-Level Cohesion

```tsx
import * as z from "zod";
import { useForm } from "react-hook-form";
import { zodResolver } from "@hookform/resolvers/zod";

const schema = z.object({
  name: z.string().min(1, "Please enter your name."),
  email: z
    .string()
    .min(1, "Please enter your email.")
    .email("Please enter a valid email address.")
});

export function Form() {
  const {
    register,
    formState: { errors },
    handleSubmit
  } = useForm({
    defaultValues: {
      name: "",
      email: ""
    },
    resolver: zodResolver(schema)
  });

  const onSubmit = handleSubmit((formData) => {
    // Form data submission logic
    console.log("Form submitted:", formData);
  });

  return (
    <form onSubmit={onSubmit}>
      <div>
        <input {...register("name")} placeholder="Name" />
        {errors.name && <p>{errors.name.message}</p>}
      </div>

      <div>
        <input {...register("email")} placeholder="Email" />
        {errors.email && <p>{errors.email.message}</p>}
      </div>

      <button type="submit">Submit</button>
    </form>
  );
}
```

https://frontend-fundamentals.com/code-quality/en/code/examples/form-fields.html