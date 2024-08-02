# Centering stuff in HTML 
Apparently in the frontend community, "centering a div" is a simple, but age-old problem that many developers faced in the past. I still struggle with centering things regardless :D. 
So, here are a few ways to center things, so I can remember and refer to them when I inevitably struggle again. 

## Centering stuff horizontally

### Using flexbox 
When using flexbox, remember to apply 

```
display: flex;
```

to the parent container, so that its children are included into the workflow. 
Then, center the children by applying

```
justify-content: center;
```
By default, the main axis should be row, so we don't need to worry about the flex-direction. FYI older browsers may not support flexbox, so in that case another method needs to be a sought. 

### Margin auto

```
margin: 0 auto;
```

The line above sets the top/bottom margins to 0, but sets the right/left margin to whatever is default. 
