# React Router v6 Trailing Slash Bug

This repository demonstrates a common, yet subtle, bug in React Router v6 related to routes with trailing slashes.  The issue arises when navigating to a route that has a trailing slash, resulting in unexpected 404 errors.

## Bug Description

The provided `bug.js` demonstrates a simple React app with two routes: `/` and `/about`. Navigating to `/about` works correctly, but navigating to `/about/` (with a trailing slash) returns a 404. This is inconsistent and often leads to debugging headaches.

## Solution

The `bugSolution.js` file provides a solution by using the `useSearchParams` hook to handle the trailing slash gracefully.  It's a robust approach that ensures a smooth user experience.