# React Router DOM v6 Catch All Route Issue

This repository demonstrates a common issue encountered when using catch-all routes (`/*`) in React Router DOM v6. The problem is that the catch-all route does not always trigger when an invalid route is accessed.

## Problem

The `App.js` file contains a basic React Router setup with a catch-all route intended to handle 404 errors.  However, this catch-all route is not correctly catching all invalid routes. 

## Solution

The `AppSolution.js` file demonstrates a solution to this problem. The order of routes matters! The catch-all route must be placed at the end of the `Routes` component. This ensures that it only matches routes that haven't already been matched by more specific routes.