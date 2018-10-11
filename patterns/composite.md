# Composite Pattern

> The composite pattern describes a group of objects that is treated the same way as a single instance of the same type of object. The intent of a composite is to "compose" objects into tree structures to represent part-whole hierarchies. Implementing the composite pattern lets clients treat individual objects and compositions uniformly [1]

## Overview


```js
const Component = ({ children }) => (
  React.Children.map(children, (child) => (
    React.cloneElement(child, {
      handler: this.setState,
    })
  ))
)

const Root = () => (
  <Component>
    <SubComponent />
    <SubComponent />
  </Component>
)
```

## Example

## Resources

- [1] https://en.wikipedia.org/wiki/Composite_pattern
