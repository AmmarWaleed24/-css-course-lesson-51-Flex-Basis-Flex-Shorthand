# Flexbox, Flex-Basis & Flex Shorthand in CSS lesson 51

## Flexbox in CSS
Flexbox is a CSS layout model designed to distribute space and align items efficiently within a container, even when their sizes are dynamic.

### Key Flexbox Properties
- **`display: flex;`** → Enables flexbox on a container.
- **`flex-direction`** → Defines the direction of items (`row`, `column`, etc.).
- **`justify-content`** → Aligns items along the main axis (`center`, `space-between`, etc.).
- **`align-items`** → Aligns items along the cross axis (`flex-start`, `center`, etc.).
- **`flex-wrap`** → Controls whether items wrap onto a new line (`nowrap`, `wrap`).

### Example:
```css
.container {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
}
```

---

## Flex-Basis in CSS
The `flex-basis` property defines the initial size of a flex item before any shrinking or growing occurs.

### Values:
- **Length values** (e.g., `200px`, `50%`) → Sets a fixed initial size.
- **`auto`** (default) → Uses the element’s original size.
- **`0`** → Makes the element fully flexible.

### Example:
```css
.item {
    flex-basis: 150px;
}
```

---

## Flex Shorthand
The `flex` shorthand combines three properties:
1. **`flex-grow`** → Defines how much an item should grow.
2. **`flex-shrink`** → Defines how much an item should shrink.
3. **`flex-basis`** → Sets the initial size.

### Syntax:
```css
flex: [flex-grow] [flex-shrink] [flex-basis];
```

### Examples:
#### 1. Equal Flexible Items:
```css
.item {
    flex: 1;
}
```
Equivalent to `flex: 1 1 0;`, meaning items grow equally and can shrink.

#### 2. Fixed Initial Size with Flexibility:
```css
.item {
    flex: 2 1 150px;
}
```
This means the item starts at `150px`, grows twice as fast as others, and can shrink.

#### 3. Prevent Shrinking:
```css
.item {
    flex: 1 0 100px;
}
```
The item grows but never shrinks.

---

## License
This project is open-source. Feel free to use and modify it as needed.

## Author
[Ammar Waleed]

