# State Management

#### Table of Contents
- [Description](#description)
- [Benefits of Approach](#benefits-of-approach)
- [Common Issues](#common-issues)
- [Use Instructions](#use-instructions)

## Description
An example of a single-page application architecture, using a simple JavaScript app, with a simple counter element that increments when a user clicks an associated button. The app then had a vanilla JavaScript state management constructed, so as to demonstrate the basic workings of contemporary third-party libraries.

## Benefits of Approach
- Efficient use of global state management tools ensures that data remains consisteny and synchronised for use across the app
- Third-party libraries (such as [Redux](https://redux.js.org/)) are widely documented and have established patterns to help developers build and test efficiently

## Common Issues
- Performance degradation after state expansion
    - Selective use of memoization can cut down on the reliance of storing data in the global state. This approach can come with its own perfomance issues if not properly managed, however.
- State synchroniation
    - Avoid conflicts between local and global state (which can cause unnecessary re-renders) by ensuring one single source of truth
- Debugging/Troubleshooting Difficulties
    - Use of browser-based Developer Tools (such as [Redux DevTools](https://github.com/reduxjs/redux-devtools))
    - Efficient use of error handling can help identify issues earlier
- Maintainability/Scalability
    - Regular code reviews can help identify which state management tools are most effective for a specific app (i.e. the React [Context API](https://react.dev/reference/react/useContext) tends to be more useful for smaller applications, whilst libraries such as [Redux](https://redux.js.org/)) are better employed for larger apps)
- Integration and Testing
    - Focusing on the use of state-related functionalities can offer better coverage (such as use of mocking or stubbing to isolate components during testing)
    - Integration testing can offer a more comprehensive understanding of state manageement performance

## Use Instructions
- CD into project folder
- Run `npm install`
- Run `npm run dev`