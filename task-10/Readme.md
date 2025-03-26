# Interactive Multi-Page Website Simulator with CSS Only

## Created a webpage that allow to navigate different section with the connectivity of id

## HTML used Elements:

| **HTML Tag**                               | **Description**                                                                 |
| ------------------------------------------ | ------------------------------------------------------------------------------- |
| `<div class="main_container">`             | Defines a main section that holds a content                                     |
| `<nav class="navbar">`                     | Defines navbar for the page                                                     |
| ` <li><a href="#men">MEN</a></li>`         | List with anchor tag helps to navigate along sections and pages.                |
| `ul`                                       | Represents a unordered list.                                                    |
| `<div class="content">`                    | Represents a content below the header which holds a sidebar and main_content.   |
| `  <section class="collections" id="men">` | Represents a Section of the page which is connected by id to the hyperlink tag. |

## CSS used Elements:

| **CSS Elements**                           | **Description**                                                                 |
| ------------------------------------------ | ------------------------------------------------------------------------------- |
| `z-index: 1000`                            | Defines a layer which stacks the content based on the input                     |
| `display:none`                             | Hides the other sections and `block` will be active once it is targeted         |
| `.collections:target`                      | Allows to make the section visible by setting the opacity to 1.                 |
| `grid-template-columns: repeat(3, 1fr);`   | Represents a grid with a repetitive column of 3 with 1 fractional unit.         |
| `transition: opacity 0.5s ease-in-out, visibility 0.5s ease-in-out;`                    | Allows to provide the animation (fade in and out) while navigating to the sections   |
|  | Other basic CSS elements is used. |

## Output Images for Web and mobile View
![alt text](./assests/Output.gif)