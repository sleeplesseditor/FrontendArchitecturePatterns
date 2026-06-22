# Microfrontends

#### Table of Contents
- [Description](#description)
- [Benefits of Approach](#benefits-of-approach)
- [Additional Points](#additional-points)
- [Common Issues](#common-issues)
- [Use Instructions](#use-instructions)

## Description
- Using a very basic Vanilla JS app, this is a demonstration of how microfrontends can be assembled and run on different ports, whilst using the same component base. One variant uses all the existing components, whilst the other two utilise only specific components.

## Benefits of Approach
- Decomposition
    - Components can be more readily isolated on focused on specific business cases
- Independence
    - Specific technologies can be selected by individual teams to best serve their unique focuses, rather than using one technology and having to work around its limitations
- Autonomy
    - Different teams can work independently with each microfrontend, potentially facilitating faster development cycles and easier maintenance

## Additional Points
- Buildtime Integration Approach – Module Federation
    - Allows for the sharing of dependencies between microfrontends
- Runtime Integration Approach
    - Use of iframes do come with downsides – largely around performance and communication limitations
- Web Components
    - Can be used as NPM packages, which can be made available for use in containerised projects

## Common Issues
- Incorrect application to smaller projects/smaller developer teams
    - Microfrontends aren't necessary for smaller organisations (typically with fewer than 3-4 developer teams). If the project is released as a single unit, microfrontends can add unnecessary complexity
- Mixing of frontend technologies
    - In some instances, teams have been known to utilise different frameworks and libraries for their respective parts of a microfrontend architecture. The maintenance overhead this adds to a project is significant and should be avoided at all costs where possible

## Use Instructions
- CD into project folder
- Run `npm install` in project folder, and the container, shipments and tracker subfolders
- Run `npm run dev` in project folder
- Use localhost on ports 8080, 8081 and 8082 to see the microfrontend areas running