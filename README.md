reflux-create-reducer
===

[This code packaged as a node module](https://github.com/rackt/redux/blob/9b0630fe9ea8209777fed7cac78fee7ee76fce67/docs/recipes/ReducingBoilerplate.md#generating-reducers)

Usage:

```js
import { createReducer } from 'reflux-create-reducer';
import * as ActionTypes from '../constants/ActionTypes';

export const todos = createReducer([], {
  [ActionTypes.ADD_TODO](state, action) {
    let text = action.text.trim();
    return [...state, text];
  }
}
```
