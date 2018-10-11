# Factory Component Pattern

## Overview

A factory component accepts a component as a prop and determines how the accepted component will render.

Using factory components for creation is similar to using a decorator to render a higher-order component. The biggest difference is, a factory component can dynamicaly change how the wrapped component is rendered via prop values.

```js
const Root = (parentProps) => (
  <Component parentProps>
    <Factory type={ SomeComponent } childProps parentProps />
  </Component>
)
```

## Example

```js
const SignupForm = (props) => 
  <Form onSubmit={ props.onSubmit }>
    <FormField fieldType={ Input } type='email' validator={ emailValidtor } />
    <FormField fieldType={ Input } type='password' validator={ passwordValidtor } />
    <FormField fieldType={ Button } type='submit' />
  </Form>
)
```
