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

## 3. justify-content

flex-start, center, flex-end, space-between, space-around

```css
body {
  display: flex;
  flex-direction: column;
  justify-content: center; // default: flex-start; [flex-start, center, flex-end, space-between, space-around]
}
```

### Example
[DEMO: justify-content](https://embed.plnkr.co/UlflR3Oy36RxufplPyfP/)

## 4. align-item

```css
body {
  display: flex;
  flex-direction: row;
  align-items: baseline; //default: stretch; [stretch, flex-start, center, flex-end, baseline] 
}
```

### Image
![align-items](https://www.w3.org/TR/css-flexbox-1/images/flex-align.svg)

### Example
[DEMO: align-items](https://embed.plnkr.co/oay2ilxe26b2v2Dkt0DX/)

## 5. align-self

Same effect as `align-items`, but `align-self` only affect itself.

### Example:
[DEMO: align-self](https://embed.plnkr.co/KyYBRhOpFWlIL0T1Odcu/)


## 6. 