# Designing Art Gallery using Dynamic Segments with useParams in React Router

**On a traditional website, when a user clicks on a URL, the browser makes a full-page request from the server and directs the user to a new page. This is referred to as static routing.**

This is very useful if you need to navigate the user to a new page. But with the development of web apps, there's more need for pages to render on the client or load dynamically.

This involves updating particular parts of the URL called segments, as well as rendering new content or updating the content on the same page without making a request from the server or reloading the entire page.

This is very common and useful in modern web apps. It enables client-side rendering, improves webiste navigation, and enables smooth transitions and animations (since the browser doesn't need to reload the page from external servers).

This can overall improve website performance and enable a good user experience.

## Client-Side Routing

In React Router, navigation is relative between the `path` attribute and the `to` property. When a user clicks using the `<Link>` component (`<a>` tag), it navigates to the specified `path` within the route componet and renders the component when it matches.

This type of navigation is called client-side routing because we are not rendering the pages from the server, but rather navigating from one components to another within the app.

## Dyanmic Segments

A Dynamic Segment, as the name suggests, is a way of rendering a new component (UI) by updating a particular segment in teh URL called params. You use the [useParams](https://reactrouter.com/en/main/hooks/use-params) hook from `react-router-dom` to do this.

This is very useful in situations where content needs to render dynamically from a partiduclar component or third-party API.

In a real-world application, Dynamic Segments are mostly used to render content dynamically when the segement `:itemId` matches the `id` of the returned APIs.

## Nested Routing

Nested routing makes it possible to nest routes to render new components on the same page for easy navigation and quick interactivity of the element. Nested routes make listed items function as a tab. As soon as any tab is clicked, the content that matches the corresponding tab gets displayed.
