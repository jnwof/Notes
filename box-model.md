# The Box Model

## What is the box model? 
The box model describes how an element exists in a webpage - it describes its size and space taken. We can imagine that every element is surrounded by boxes.
There are four layers of these boxes, described in the following order (interior to exterior). 

<p align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/7/7a/Boxmodell-detail.png" alt="Visualization of the Box Model">
</p>

1. Content (Most interior) 
2. Padding
3. Border
4. Margin (Most exterior)

***

### Content
* The content box is where the texts and images appear.

```
div {
  width: 
  height: 
}
```

### Padding
* The padding is the blank space between the content (text and image) and the border.
* The color of the padding can be changed, and this is referred to as the background color.

```
p {
  padding: top right bottom left; <-- 4 values
  padding: top right/left bottom; <-- 3 values
  padding top/bottom right/left; <-- 2 values

  padding-top: 
  padding-right: 
  padding-left:
  padding-bottom: 

  background-color: hsla(241, 72%, 46%, 0);
}
```

### Border
* The border encapsulates the content and padding.

```
h1 {
  border: thickness style color; <-- 3

  border-width:
  border-style: solid, dotted etc. 
  border-color:  
}
```

### Margin
* The margin creates an empty area around the border.
* It can be used to create space between two elements.
* The margin is transparent.

```
div {
  margin:
}
```
