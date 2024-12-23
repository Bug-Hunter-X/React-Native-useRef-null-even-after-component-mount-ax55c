# React Native useRef Hook Unexpected Null Value

This repository demonstrates a common issue encountered when using the `useRef` hook in React Native: the `current` property unexpectedly being `null` even after component mounting. The example showcases the problem and provides a solution.

## Problem

The `useRef` hook is often used to access DOM elements or other mutable values within functional components. However, accessing `ref.current` within event handlers or callbacks may sometimes result in a `null` value, even though the component has already mounted. This is because the ref might not be fully initialized at the time of access.

## Solution

The provided solution demonstrates how to correctly handle potential `null` values using optional chaining (?.) or by ensuring the ref is accessed after the component is mounted and the ref is populated.