# Progressive Web Apps

#### Table of Contents
- [Description](#description)
- [Benefits of Approach](#benefits-of-approach)
- [Common Issues](#common-issues)
- [Use Instructions](#use-instructions)

## Description
A basic example of a Progressive Web App, using Vanilla JS and the minimum setup files required. The example shows simple HTML elements and an image file cached via instructions on the manifest JSON file and service worker file in the public folder.

## Benefits of Approach
- Offline UI options
    - The option to be able to display limited offline content for web applications can be appealing when attempting to cultivate a specific user experience
- Availability in existing frameworks/libraries (such as [Angular](https://v17.angular.io/guide/service-worker-getting-started), [React](https://create-react-app.dev/docs/making-a-progressive-web-app/) or [Vue](https://blog.logrocket.com/building-pwa-vue/))

## Common Issues
- Search Engine Optimization
    - Use of service workers has been known to confuse search engine bots due to the PWA caching mechanism
- Hardware limitations
    - PWAs have been known to be inconsistent on whether they can access specific hardware sensors, as well as encountering issues with device browsers (such as Safari on iOS)
- Lack of User Awareness
    - PWAs don't have the same general visibility and user pre-conditioning that come with native apps and how they're used

## Use Instructions
- CD into project folder
- Run `npm install`
- Run `npm run dev`
- To test the offline option, open the Network tab in your browser's Developer Tools and set the throttling option to 'Offline'. Then reload the page – the content should still render.