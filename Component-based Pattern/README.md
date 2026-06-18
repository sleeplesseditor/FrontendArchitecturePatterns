# Component-based Pattern

#### Table of Contents
- [Description](#description)
- [Benefits of Approach](#benefits-of-approach)
- [Common Issues](#common-issues)
- [Use Instructions](#use-instructions)

## Description
An example of component-based pattern architecture with a very simple JavaScript application. In this instance, a re-usable Header component has been created to ensure that all pages use the same Header, and thus any changes made to the component are available to all pages.

## Benefits of Approach
- Composability – components can be combined to form larger and more complex components
- Reusability – the same component can be re-used across projects 
- Encapsulation – promotes clean and modular code
- Ease of maintenance – changes made to the base component are reflected across all uses of said component
- Scalability – systems built with this methodology can more easily adapt as requirements change 

## Common Issues
- Tight component coupling
    - Components should only contain logic and behaviours inherent to it (i.e. not functionality unique to one specific area of the codebase)
- Scability issues
    - Consider relationships between the component and larger functionalities
    - Higher-level functionalities, such as network calls should not be included in lower-level components
- Complexity/Bloating
    - Split a growing component into different variants
    - Follow the [Single-responsibility principle](https://stackify.com/solid-design-principles/)

## Use Instructions
- CD into project folder
- Run `npm run dev`