# Builder Component Pattern

## Overview

> The intent of the Builder design pattern is to separate the construction of a complex object from its representation. [1]

Since are components represent in a tree-like hierarchy where the top most component encapulates behave of child components; the builder pattern is the most straight forward React design pattern to follow.

The construct a builder component, simply allow the top-level component to render sub-components as children. Construction of the sub-components
can be controled by passing props from the parent component to child.

This example represents a parent component passing props down to a child prop. The creation of `SubComponent` is abtracted aways from the create of the `Root` component.  

```js
const Root = (parentProp) => (
  <Component parentProp>
    <SubComponent childProp parentProp />
  </Component>
)
```

## Examples

## References

- [1] https://en.wikipedia.org/wiki/Builder_pattern
