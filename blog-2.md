# How Generics Enable Reusable and Strictly Typed Components in TypeScript

## Introduction
Generics in TypeScript allow us to build **reusable functions, classes, and components** while still maintaining strong type safety. Instead of fixing a type, generics let us pass the type dynamically.

---

## Why We Need Generics

Without generics, we often lose flexibility or type safety.

### Example Problem:
```ts
function identity(value: any) {
    return value;
}