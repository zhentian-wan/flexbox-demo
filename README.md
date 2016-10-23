# Flexbox cheetlist


## 1. `display: flex` & `flex-direction`
 
`display: flex` will make align all sibling elements in row;
`flex-direction: column` make elms shows in column

```css
.main-nav ul {
  list-style: none;
  display: flex;
  flex-direction: column; // default : row
}
```

### Example:
[DEMO: display direction](https://embed.plnkr.co/aiWo0ykJbjrXNJ3nbqEe/)


## 2. `order`

Change the element order.

`order: -1` will put the element to the first place, if you have mutli `order: -1` defined, it will also according to the 
element order in DOM.

### Example
[DEMO: Order](https://embed.plnkr.co/yHethVQUyjem7G9mztFc/)

## 3. 