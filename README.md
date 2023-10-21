# HTML-CSS-JAVASCRIPT_Notes
### px vs rem vs em
* px: absolute (doesn't change)</br>
* em: changes relative to parent</br>
* rem: changes relative to root</br>

!!! default font-size of HTML is 16px=1em=1rem.

### flex
Center your content
```
.flex {
  display: flex;
  justify-content: center;
  align-items: center;
 }
```
Prevent overflowing (better alternative available with grid)
```
.flexContainer {
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
}
```
### grid
Grid of 4 columns
```
.grid-container {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
}
```
Grid with more flexibility using media quries (better alternative available)
```
// if the screensize is >= 60em, columns = 4
// if 40em <= screensize <= 60em, column = 2
// if screensize < 40em, column = 1
.grid-container {
  display: grid;
}

@media (min-width: 40em) {
  .grid-even-columns {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (min-width: 60em) {
  .grid-even-columns {
    grid-template-columns: repeat(4, 1fr);
  }
}
```
<img width="1275" alt="Screen Shot 2023-10-19 at 10 21 05 PM" src="https://github.com/diwassapkota805/HTML-CSS-JAVASCRIPT_Notes/assets/102276270/93bf78be-2736-489f-a60a-b32b42b1a85d">

## Grid vs Flexbox
Flexbox are generally good for 1D.  
Grid is generally good for 2D.


