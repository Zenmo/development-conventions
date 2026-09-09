Frontend component code style
===

## Separate responsibilities

A component should not combine many responsibilities.

These are common examples of separate responsibilities which should go in separate components or functions:

| Responsibility      | Examples                                                           |
|---------------------|--------------------------------------------------------------------|
| Styling             | Button<br />Header<br />Portrait<br />Dropdown                     |
| Image display       | SVG Icon<br />Picture                                              |
| Layout              | Responsive row<br />Data table<br />Page layout<br />Card or Panel |
| Handling user input | Upload element<br />Search box                                     |
| Form hydration      | Load inputs into a typed object                                    |
| Form logic          | Filter a data table<br />Submit to a database                      |
| State management    | Store the currently logged in user<br />Currently active filters   |
| Library adapter     | Chart<br />GIS map                                                 |

## Prefer plain code

Components should not contain large amounts of logic which can exist independent of the component. This should go in separate files.

Examples:

- Type definitions
- Clients to communicate with the backend or an external API
- State management
- Data transformation

Files with components should avoid exporting any other symbols.

## Maximum size

A component has a maximum size of 200 lines of code. This includes the HTML, CSS and JavaScript.

When using utility classes such as Tailwind or Bootstrap, this maximum is 150 lines.

Exempted are components which are mostly content and contain no logic. These have no maximum size.
