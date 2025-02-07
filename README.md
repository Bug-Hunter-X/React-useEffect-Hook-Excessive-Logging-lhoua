# React useEffect Hook Excessive Logging
This repository demonstrates a common React bug involving the `useEffect` hook and how to fix it.

The problem occurs when the `useEffect` hook doesn't specify its dependencies correctly and causes unexpected re-renders and performance degradation. This example showcases the bug and provides a clear solution.

## Bug Description
The initial `useEffect` hook logs the `count` value to the console after *every* render, leading to unnecessary console output and performance implications. The improved version correctly adds the `count` variable to the dependency array, preventing excessive logging and improving performance.

## How to Run
1. Clone this repository.
2. Navigate to the repository's directory in your terminal.
3. Run `npm install` to install the dependencies.
4. Run `npm start` to start the development server.

## Solution
The solution correctly specifies `count` as a dependency within the `useEffect` hook's dependency array. This ensures the effect runs only when the `count` value changes, improving performance and reducing unnecessary console logging.