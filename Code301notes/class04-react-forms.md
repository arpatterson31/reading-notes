# Readings: React and Forms

## Article - Forms

- Forms in HTML usually maintain their own state and update it based on user input
- Forms in React typically have state updated with `setState()`

- These 2 ways can be combined so the React state is the "single source of truth"
  - React component will render a form and also controls what happens in the form with user input

### Other difference HTML vs React

#### Textarea

- In HTML `<textarea>` defines its text by its children
- In React `<textarea>` uses `value` attribute
  - `value` can be put in state

#### Select

- In HTML `<select>` creates drop down list
- In React `<select>` uses `value` attribute on root `<select>` tag

### Multiple Inputs

- Handling multiple controlled `input` elements, add `name` attribute so the handler function can choose what to do based on the value `event.target.name`
- Name can be set in state to make it dynamic
