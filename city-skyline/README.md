# City Skyline

A Colored Markers webpage created using CSS in different ways to set color values and pair colors with each other.

## Tech Stack

- HTML
- CSS

## Screenshot
![City Skyline Screenshot](../assets/images/screenshots/city-skyline.png)

On Mobile:

![City Skyline Mobile Screenshot](../assets/images/screenshots/city-skyline-mobile.png)


## Notes
### Variable
Variable declarations begin with two dashes (-) and are given a name and a value like this: --variable-name: value;

```CSS

.bb1 {

  --building-color1: #999;
}
```

To use a variable, put the variable name in parentheses with var in front of them like this: var(--variable-name). Whatever value you gave the variable will be applied to whatever property you use it on.

```CSS
.bb1a {
  width: 70%;
  height: 10%;
  background-color: var(--building-color1);
}
```



#### fallback value
You should add a fallback value to a variable by putting it as the second value of where you use the variable like this: 

```CSS
var(--variable-name, fallback-value).
```

#### declare in :root selector
*The variables do not work in sibling elements*. That's just how CSS works. Because of this, variables are often declared in the :root selector. This is the highest level selector in CSS; putting your variables there will make them usable everywhere.


```CSS
:root {
  --building-color1: #aa80ff;
  --building-color2: #66cc99;
  --building-color3: #cc6699;
}
```
