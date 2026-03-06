# Lab 07 – Code Splitting with React.lazy and Suspense

## Description

This project demonstrates code splitting in a React application using `React.lazy` and `Suspense`. Lazy loading allows components to be loaded only when they are needed, improving application performance and reducing the initial bundle size.

## Technologies

- React
- Vite
- React Router
- JavaScript

## Project Structure

src/

- pages/
  - Home.jsx
  - Dashboard.jsx
  - Settings.jsx
  - Profile.jsx
- components/
  - LoadingSpinner.jsx
- App.jsx

## Implementation

### Lazy Loading

The pages `Dashboard`, `Settings`, and `Profile` are loaded using:

```javascript
const Dashboard = lazy(() => import("./pages/Dashboard"));
