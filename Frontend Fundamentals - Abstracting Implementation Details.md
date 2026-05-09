---
tags:
  - fleeting
---
# References

```tsx
function LoginStartPage() {
  useCheckLogin({
    onChecked: (status) => {
      if (status === "LOGGED_IN") {
        location.href = "/home";
      }
    }
  });

  /* ... login related logic ... */

  return <>{/* ... login related components ... */}</>;
}
```

to Wrapper

```tsx
function App() {
  return (
    <AuthGuard>
      <LoginStartPage />
    </AuthGuard>
  );
}

function AuthGuard({ children }) {
  const status = useCheckLoginStatus();

  useEffect(() => {
    if (status === "LOGGED_IN") {
      location.href = "/home";
    }
  }, [status]);

  return status !== "LOGGED_IN" ? children : null;
}

function LoginStartPage() {
  /* ... login related logic ... */

  return <>{/* ... login related components ... */}</>;
}
```

or to HOC

```tsx
function LoginStartPage() {
  /* ... login related logic ... */

  return <>{/* ... login related components ... */}</>;
}

export default withAuthGuard(LoginStartPage);

// Define HOC
function withAuthGuard(WrappedComponent) {
  return function AuthGuard(props) {
    const status = useCheckLoginStatus();

    useEffect(() => {
      if (status === "LOGGED_IN") {
        location.href = "/home";
      }
    }, [status]);

    return status !== "LOGGED_IN" ? <WrappedComponent {...props} /> : null;
  };
}
```

https://frontend-fundamentals.com/code-quality/en/code/examples/login-start-page.html