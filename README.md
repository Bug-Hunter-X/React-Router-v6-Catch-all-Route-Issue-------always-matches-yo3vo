# React Router v6 Catch-all Route Issue

This repository demonstrates a problem with the catch-all route (`/*`) in React Router v6.  The issue is that the catch-all route always matches, even when a more specific route should match first.  This results in the wrong component being rendered.

The problem is shown in `App.js`. The solution is shown in `AppSolution.js`

## How to reproduce
1. Clone this repo
2. Run `npm install`
3. Run `npm start`
4. Navigate to `/` or `/about`. Notice that the `NotFound` component is rendered, even though `/` and `/about` are defined routes.