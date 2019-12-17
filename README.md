# Ahnen.js
A set of javascript functions for interpreting [Ahnentafel](https://en.wikipedia.org/wiki/Ahnentafel) numbers for genealogy.

Works with node.js. A standalone version of the code is available in the Standalone folder

## Functions
``` js
ahnen.sex(int)
```

Returns string `Male` or `Female` associated with the Ahnen number `int`.

```js
ahnen.line(int)
```

Returns string `'rootPerson'`, `'fathersLine'`, `'mothersLine'`, or `'undetermined'`.

```js
ahnen.fullLine(int)
```
__IMPORTANT!__
In this function M means Mother and F means Father, NOT male and female.

Returns an array of the relationship between ahnen number int and ahnen number 1.
For example, the ahnen number 10 would return the array `[M, F, M]`, 
meaning the root person's mother's father's mother.
