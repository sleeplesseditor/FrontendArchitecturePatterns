# Server-Side Rendering (SSR)

#### Table of Contents
- [Description](#description)
- [Benefits of Approach](#benefits-of-approach)
- [Common Issues](#common-issues)
- [Use Instructions](#use-instructions)

## Description
A basic example of SSR achieved using a simple Express server serving an EJS file to the browser.

## Benefits of Approach
- Search Engine Optimization (SEO)
    - Use of SSR can ensure that SEO crawlers can received a fully popuilated HTML document, and avoid finding an empty shell, as can be the case for other architecture approaches
- Faster Load Times
    - Users get a visible UI far faster, as they have a populated HTML file, rather than an empty shell, potentially in a loading state
- Better Performance on Lower Spec Devices
    - With the server handling heavier computational duties, lower tier devices experience better performance when loading the UI

## Common Issues
- Server Load
    - Computational responsibilities being offloaded to the server means that the server has to process/generate HTML files for every single page request
    - Supporting this requires more expensive back-end solutions
- Delayed Interactivity
    - Whilst content is visible quickly, interactivity can be delayed as JavaScript bundles are downloaded to the browser (otherwise known as ['hydration'](https://www.workingsoftware.dev/understanding-ssr-with-hydration-for-software-architects/))
    - This issue also manifests in page-to-page navigation being slower, as it can often require re-fecthing entire pages from the server

## Use Instructions
- CD into project folder
- Run `npm install`
- Run `npm run dev`