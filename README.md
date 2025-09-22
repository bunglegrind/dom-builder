# DOM Builder: A vanilla Javascript alternative to JSX

## Inspired from https://www.crockford.com/domjs.html

Usage:

```javascript
const dom = domBuilder(document);
dom.<tag>(id|props)(...children)
```
For void elements
```javascript
const dom = domBuilder(document);
dom.input(id|props)
```
Argument can be a string (id) or an object literal (props) with attribute => value properties. If attribute is `class`, value can be an array of string.
If value is a function, it is added as a listener for the attribute event.
If a node does not have children, there is no need to invoke the function without argument. It is automatically invoked by the dom builder.
