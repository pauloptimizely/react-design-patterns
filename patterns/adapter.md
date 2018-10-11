# Adapter Component Pattern

## Overview

> The adapter pattern allows the interface of an existing class to be used as another interface. It is often used to make existing classes work with others without modifying their source code. [1]

The adapter component pattern can be to used to create a more uniform interface by mapping props from a Root component to a third party component.

```js
const Root = (parentProp) => (
  <Component foreignProp={ parentProp }>
  </Component>
);
```

## Examples


## Resources

- [1] https://en.wikipedia.org/wiki/Adapter_pattern
