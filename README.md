# DOM Builder: A vanilla Javascript alternative to JSX

## Inspired from https://www.crockford.com/domjs.html

Usage:

class can be an array

```javascript
const dom = domBuilder();
dom.<tag>(id|props)(...children)
```
For void elements
```javascript
const dom = domBuilder();
dom.input(id|props)
```

Function attributes (onclick, etc.) are note supported.
