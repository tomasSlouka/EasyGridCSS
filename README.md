# YMELLO - EasyGridCSS

The most easy grid css framework on the web.  
One file, easy setup, almost no learning cuve.  

## How to use

To use EasyGridCSS link css file `grid.css` to you project.  
Initialize grid on the element by using class `grid`  

## Basic example

To divide layout to 3 cols we use class `col-3`  

```html
<div class='grid col-3'>
  <element-1>
  <element-2>
  <element-3>
  <element-n>
</div>
```

## Classes for parrent element
### Basic
`grid` - initialize grid on the element  
`auto` - child elements will automatically adjust its width to fill available space
`col-n` - divide element to `n` cols where n is number from 1 to 12  

### Display specific
`xs-col-n` - extra small display (max-width : 576px)  
`sm-col-n` - small display (min-width : 576px)  
`md-col-n` - tablet size display (min-width : 768px)  
`lg-col-n` - desktop display (min-width : 992px)  
`xl-col-n` - extra large display (min-width : 1200px)  

### Content and items alignment (self-explanatory)
`align-content-start`  
`align-content-end`  
`align-content-stretch`  
`align-content-center`  
`align-content-space-around`  
`align-content-space-between`  
`align-content-space-evenly`  

`justify-content-start`  
`justify-content-end`  
`justify-content-stretch`  
`justify-content-center`  
`justify-content-space-around`  
`justify-content-space-between`  
`justify-content-space-evenly`  

`align-items-start`  
`align-items-end`  
`align-items-stretch`  
`align-items-center`  

`justify-items-start`  
`justify-items-end`  
`justify-items-stretch`  
`justify-items-center`  

### Gaps between child element
`gap1` - `gap100` - from 1px to 100px  

## Classes for child element (item)
### Item column span
`span-n` - span child element to `n` cols where n is number from 1 to 12  

### Item column start
`start-n` - start child element at `n` column where n is number from 1 to 12

### Display specific item span
`xs-span-n` - extra small display (max-width : 576px)  
`sm-span-n` - small display (min-width : 576px)  
`md-span-n` - tablet size display (min-width : 768px)  
`lg-span-n` - desktop display (min-width : 992px)  
`xl-span-n` - extra large display (min-width : 1200px) 

### Self alignment (self-explanatory)
`align-self-start`  
`align-self-end`  
`align-self-stretch`  
`align-self-center`  

`justify-self-start`  
`justify-self-end`  
`justify-self-stretch`  
`justify-self-center`

## Advanced example
### Problem
Divide layout to 4 cols on desktop display, 2 cols on tablet and 1 col on mobile devices. On tablet the third one item should span 2 cols. Items should be align to top and center  

### Solution
```html
<div class='grid lg-col-4 md-col-2 xs-col-1 align-items-start justify-items-center'>
  <element-1>
  <element-2>
  <element-3 class='md-span-2'>
  <element-4>
  <element-5>
  <element-6>
</div>
```
