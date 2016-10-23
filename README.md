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


## 6. flex-basis, flex-shrink, flex-grow

Recommend to use `flex-basis` to control the width.
`flex-shrink`: use the min space, default = 1
`flex-grow`: use the all available space, default = 0

```css
.title-1 {
  background: #dd5f40;
  flex-basis: 0px; 
}
```

## Example
[DEMO: flex-basis, flex-shrink, flex-grow](https://embed.plnkr.co/GRnTfSBWD5U8257ymDBF/)

## 7. flex: shorthand syntax:

```css
.title-1 {
  background: #dd5f40;
  flex: 1;
    /* flex-grow: 1;
       flex-shrink: 1;
       flex-basis: 0;
    */
}

.title-2 {
  background: #3d483a;
  flex: 20px;
    /* flex-grow: 1;
       flex-shrink: 1;
       flex-basis: 20px;
    */
}

.title-3 {
  background: #468e5d;
  flex: 0 80px;
    /* flex-grow: 0;
       flex-shrink: 1;
       flex-basis: 80px;
    */
}
```

## 8. align-content
 
affect the whole wrapper, not single element

[DEMO flex-wrap, align-contetn](https://embed.plnkr.co/5t0R7xH9eVmekxGalAQa/)

## 9. 