# React Native Dimensions API Issue

This repository demonstrates a common issue when using the `Dimensions` API in React Native to obtain screen dimensions. The problem arises when accessing dimensions too early in the component's lifecycle, before the layout has fully initialized.  The solution involves using the `useEffect` hook to ensure dimensions are retrieved after the component has mounted.

## Problem

The `IncorrectDimensions.js` file showcases the problem.  It attempts to access screen dimensions immediately in the component's render method. This often results in incorrect or inconsistent values, leading to rendering problems.

## Solution

The `CorrectDimensions.js` file demonstrates a solution using the `useEffect` hook.  The dimensions are only fetched after the component mounts, ensuring accurate measurements.

## Usage

Clone the repository and run the project using a React Native development environment.