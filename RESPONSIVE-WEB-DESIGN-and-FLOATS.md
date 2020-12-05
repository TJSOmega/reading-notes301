# Responsive Web Design and Floats

## Responsive Web Design

-  The term responsive web design refers to a type of design style in where a website adapts to any situation.

-  The other design styles are Adaptive, and Mobile *(Adaptive is basically interchangeable, while mobile is a whole new website created for mobile devices but it is the worst option)*

-  Ethan Marcotte was the one who coined the term responsive web design.

- **Responsive Web design formula is target ÷ context = result**
- *The formula is based around taking the target width of an element and dividing it by the width of it’s parent element. The result is the relative width of the target element.*

### Media Queries
-  Media Queries are rules that are created for specific browsers.

- There are a couple different ways to use media queries, using the @media rule inside of an existing style sheet, importing a new style sheet using the @import rule, or by linking to a separate style sheet from within the HTML document. Generally speaking it is recommend to use the @media rule inside of an existing style sheet to avoid any additional HTTP requests.


### Mobile First

- One popular technique with using media queries is called mobile first. The mobile first approach includes using styles targeted at smaller viewports as the default styles for a website, then use media queries to add styles as the viewport grows.


## Floats

- A Float is a CSS Property that sends a page object somewhere on a page.

- When an object is floated it is not removed from the page *flow*.

- There are 4 values for the Float Property *(Left, Right, None, and Inherit)*

- Clear allows you to bypass regular document flow and send an object down onto the next available line.

-
