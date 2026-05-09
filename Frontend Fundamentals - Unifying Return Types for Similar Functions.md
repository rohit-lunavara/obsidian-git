---
tags:
  - fleeting
---
# References

```tsx
import { useQuery } from "@tanstack/react-query";

function useUser() {
  const query = useQuery({
    queryKey: ["user"],
    queryFn: fetchUser
  });

  return query;
}

function useServerTime() {
  const query = useQuery({
    queryKey: ["serverTime"],
    queryFn: fetchServerTime
  });

  return query.data;
}
```

to

```tsx
import { useQuery } from "@tanstack/react-query";

function useUser() {
  const query = useQuery({
    queryKey: ["user"],
    queryFn: fetchUser
  });

  return query;
}

function useServerTime() {
  const query = useQuery({
    queryKey: ["serverTime"],
    queryFn: fetchServerTime
  });

  return query;
}
```

https://frontend-fundamentals.com/code-quality/en/code/examples/use-user.html