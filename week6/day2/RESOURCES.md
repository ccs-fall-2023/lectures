# Resources

## Web App Ideas

* [Flavio Copes: A list of sample Web App Ideas](https://flaviocopes.com/sample-app-ideas/)

## Single Page Applications

* [Mary Boyd: Single Page Applications: A Powerful Design Pattern for Modern Web Apps](https://medium.com/a-lady-dev/single-page-applications-a-powerful-design-pattern-for-modern-web-apps-ec3590bb7e7a)
  This article is ~5 years old, but the pros/cons section is still accurate.
* [Dev.to: Visualization of route navigation in a React app](https://dev.to/manu4216/visualization-of-route-navigation-in-a-react-app-35lg)

## CRUD

* [Free Code Camp: CRUD Operations – What is CRUD?](https://www.freecodecamp.org/news/crud-operations-explained/)
* [Build a CRUD application in React with Firebase Web SDK v9](https://blog.logrocket.com/build-crud-application-react-firebase-web-sdk-v9/)
  **NOTE**: This is relatively current still, although some of the React installation might be from before Vite.

## Debugging

* [Matt Rickard: Lessons from Debugging](https://matt-rickard.com/lessons-from-debugging?utm_source=changelog-news)
* [Changelog Youtube Channel:Trying to find a bug? It's almost always your fault...](https://www.youtube.com/watch?v=X42aF-ofrx8)

## React Router

* [Log Rocket: Migrating to React Router v6: A complete guide](https://blog.logrocket.com/migrating-react-router-v6-guide/)
* [Remix.run: Remixing React Router](https://remix.run/blog/remixing-react-router)
* [Official v5 to v6 Migration Guide](https://github.com/remix-run/react-router/discussions/8753)
* [React Router v6: Migrating to RouterProvider](https://reactrouter.com/en/main/upgrading/v6-data#migrating)

> The first thing to be aware of is the presence of a handful of new Data APIs that only work on routes defined via the new data routers (i.e., createBrowserRouter). These include a few categories of APIs:
> * Route-level data APIs such as loader, action, shouldRevalidate, handle, and lazy
> * In-component data hooks such as useLoaderData, useActionData, useFetcher, useMatches, useNavigation, etc.
> * Error-handling APIs such as route.errorElement, route.ErrorBoundary, and useRouteError
>
>The rest of the APIs that existed prior to v6.4.0 are still usable in both BrowserRouter and RouterProvider apps. These include common hooks/components such as useNavigate, useLocation, useParams, <Link>, <Outlet />, etc.

This is new with the current version of React Router (v6.4):

* [React Router v6: `createBrowserRouter`](https://reactrouter.com/en/main/routers/create-browser-router)

> This is the recommended router for all React Router web projects. It uses the DOM History API to update the URL and manage the history stack.
> It also enables the v6.4 data APIs like loaders, actions, fetchers and more.

If you look at tutorials from _before_ v6.4, this will likely be the biggest difference.
