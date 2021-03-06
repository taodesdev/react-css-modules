# react-css-modules
react app webpack with css-modules

## How to play
1. clone the repo
2. cd react-css-modules
3. npm install
4. npm start

## CSS Modules
CSS Modules have an extend functionality that can be used across files with the from keyword

### Composition
```
.className {
  color: green;
  background: red;
}

.otherClassName {
  composes: className;
  color: yellow;
}
```

### Dependencies Composing from other files
```
.otherClassName {
  composes: className from "./style.css";
}
```

### Dependencies Composing from global class names
```
.otherClassName {
  composes: globalClassName from global;
}
```

### Use with preprocessors
```
:global {
  .global-class-name {
    color: green;
  }
}
```

More about CSS Modules : https://github.com/css-modules/css-modules#composition

See also : https://css-modules.github.io/webpack-demo/

Theming with CSS Modules : https://github.com/css-modules/css-modules/blob/master/docs/theming.md

Install ref : https://www.triplet.fi/blog/practical-guide-to-react-and-css-modules/