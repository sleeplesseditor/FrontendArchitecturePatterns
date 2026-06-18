# Single-Page Application

#### Table of Contents
- [Description](#description)
- [Benefits of Approach](#benefits-of-approach)
- [Common Issues](#common-issues)
- [Use Instructions](#use-instructions)

## Description
An example of a single-page application architecture, using a simple JavaScript app. The app was then revised to use Vite, with a route and navigation setup manually created to mitigate against full-page reloads when moving between 'pages' and loading unnecessary files.

## Benefits of Approach
- Improved Performance – due to reduction of server requests, page load times and transitions are reduced
- Enhanced Interactivity – with a reduction in full-page reloads, users experience smoother interactions with the app
- Easier Development – using the modular nature of frontend frameworks and the ability to use components, development can be streamlined
- Common Usage – the majority of frontend frameworks come with SPA options readily available, and SPAs can be created from Command Line Interfaces (CLIs) with relative ease

## Common Issues
- Search Engine Optimization (SEO), due to empty HTML on inital load
    - Use of SSR (Server-side Rendering) or SSG (Static Site Generation) as alternative pattern
    - Third-party pre-rendering services are available, but come with their trade-offs
    - Injection of dynamic meta tags with third-party libraries (such as [React Helmet](https://www.npmjs.com/package/react-helmet)) can help search engines understand the purpose of each 'page' of the app
- Load Performance – initial load times can be excessive, if not managed carefully
    - Lazy Loading – defers loading of non-critical resources until needed (i.e. loading of page-related resources)
    - Caching – latency and repeat operations can be reduced, but can cause memory issues if not used selectively

## Use Instructions
- CD into project folder
- Run `npm install`
- Run `npm run dev`