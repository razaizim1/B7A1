# Why `any` is a Type Safety Hole and Why `unknown` is Safer in TypeScript

## Introduction
TypeScript is designed to give developer type safety, meaning we can catch errors during development instead of runtime. However, the `any` type breaks this safety system. On the other hand, `unknown` provides a safer alternative when dealing with unpredictable data.

---

## Why `any` is a Problem

When we use `any`, TypeScript stops checking the type completely. This means we can do anything with the value, even if it is unsafe.

### Example:
```ts
let data: any = "Hello";

data.toUpperCase(); // works
data.toFixed(); // runtime error (string has no toFixed)