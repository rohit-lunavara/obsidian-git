---
tags:
  - fleeting
---
# References

```tsx
if (a >= b && a <= c) {
  ...
}

if (score >= 80 && score <= 100) {
  console.log("Excellent");
}

if (price >= minPrice && price <= maxPrice) {
  console.log("Affordable price");
}
```

to

```tsx
if (b <= a && a <= c) {
  ...
}

if (80 <= score && score <= 100) {
  console.log("Excellent");
}

if (minPrice <= price && price <= maxPrice) {
  console.log("Affordable price");
}
```

https://frontend-fundamentals.com/code-quality/en/code/examples/comparison-order.html