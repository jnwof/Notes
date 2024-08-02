# Flexbox
Flexbox allows you to arrange items in rows or columns in a more easier and dynamic way. 

## Setting up the flexbox 
To use the flexbox model, the parent element of all the other elements you want to arrange needs to be transformed into a flex container. 
This is done by changing the display value of the parent element to:

```
parent {
  display: flex;
}
```
Once this is done, the children (all elements inside the parent flex container) will be affected when changing the flex attributes. 

## Anatomy of the flexbox 
<p align="center">
  <img src="https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox/flex_terms.png" alt="flexbox model">
</p>

* Items are layed out in the flex container following the direction of the <b>main axis</b>.
* The <b>cross axis</b> is always perpendicular to the main axis. 

## Direction of the flexbox layout
The main axis determines the direction of the flexbox - the direction that the flex items are placed. 
The default direction of the main axis is row (i.e. horizontal). This becomes important as the justify-content declaration refers to the main axis when modifying position of the flex items. 

You can change the direction of the main axis using the flex-direction declaration. There are four "modes" as stated below. 

```
flex container {
  flex-direction: row row-reverse column column-reverse;
}
```
## Use justify-content to change the layout of flex items in the main axis
There are more than 10 different values that the justify-content can take. The ones below include only the ones I have used so far. 

```
flex container {
  justify-content: center flex-start flex-end space-between space-evenly space-around;
}
```

## Use align-items to modify items on the cross axis
```
flex container {
  align-items: center flex-start flex-end start end;
```

Naturally, using the justify-content and align-items declaration appropriately makes centering elements easier. 

## Prevent items overflowing using flex-wrap
If there are too many items on the main axis of the flex container, it can overflow. According to the MDN Web Docs, this is because flexbox always tries to place all items in a single row or column. Resultantly, viewers may have to scroll horizontally to see everything on the screen which is inconvenient and also unattractive. 

Items can be made to wrap to the next line if they reach the extent of the viewport's dimensions using flex-wrap. 

```
flex container {
  flex-wrap: flex;
}
```

