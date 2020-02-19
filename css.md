# CSS

### cascading!

Styles can be overwritten by other styles... there is a hierarchy of ways to apply styles

- inline JSX styles `style={{}}`
- ids `#my-button{}` (cant be shared)
- classes `.my-button{}`
- tag name `button{}`

### units

- px
- %
- vw / vh (viewWidth, viewHeight)
- rem (proportional to the font-size of the <html> element)
- calc()

### common style rules

- display
- background or background-color
- margin
- padding
- position
- height / width
- color (text color)
- font-size
- font-weight
- border 
- border-radius
- z-index: how elements overlap. Needs a "position" rule to work
- etc etc etc

### flexbox

- `display:flex`
- `flex-direction`: row/column/row-reverse/column-reverse
- `align-items`: center, flex-start
- `justify-content`: center, space-between, space-around
- `flex-shrink:0;` will make your flex children NOT shrink

### position

- `relative`: positioned according to the elements around it
- `absolute`: means that the element can be positioned with "top","left","right","bottom" rules (relative to its first parent that has `position:relative;`)