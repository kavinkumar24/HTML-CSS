# Tabbed Content Interface

## Created a webpage that allows user to navigate various tabs to find the tourist places

- Used a basic html and css tags
- `<input type="radio" name="tab" id="tab1" checked>` - Radio format input collector
- `<nav>`, `<ul>`, `<li>`, `<h1>`
```
input[type="radio"] {
    display: none;
}
```
- this allows to hide the radio input and make them clickable through their labels

```
transition: opacity 0.5s ease, transform 0.5s ease, visibility 0s 0.5s; 
```
- this represents the smooth transition between the content
- `#tab1:checked ~ .tab_content#content1` - ~ is a  subsequent-sibling combinator selects all elements that are next siblings of a specified element.
- `:checked` - This Pseudo class defines which one want to display or apply a style to specific element (like a active state of tab bar)

## Output Images for Web and Mobile View
![alt text](./assests/Output.gif)
