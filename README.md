# TypeScript Type Coercion Bug

This repository demonstrates a subtle bug in TypeScript where type coercion leads to a runtime error that isn't caught at compile time.

## Bug Description
The `add` function is defined to accept two numbers and return their sum. However, the code calls this function with a number and a string, which is not checked at compile time due to TypeScript's loose type checking in some scenarios. This results in a runtime type error.

## How to Reproduce
1. Clone this repository.
2. Compile and run the TypeScript code using `tsc bug.ts && node bug.js`.
3. Observe the runtime type error.