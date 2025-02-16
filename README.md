# React Router Dom v6 Catch-all Route Issue

This repository demonstrates a common issue encountered when using catch-all routes (`/*`) in React Router Dom v6 with nested routes.  The catch-all route unintentionally intercepts all other routes, preventing them from rendering correctly.

## Problem

The provided example showcases a simple React application with a home page, an about page, and a not-found page. The `/*` catch-all route, intended to handle 404 errors, is incorrectly preventing access to the `/about` route.

## Solution

The solution involves a proper order and more specific pathing for your routes to make sure that your catch all route only matches the routes which are not matched by the specific routes.