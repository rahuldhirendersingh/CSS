# CSS Selectors

- CSS selectors are used to "find" (or select) the HTML elements you want to style.

## Element Selector

- The element selector selects HTML elements based on the element name.

**Example**

- Here, all <p> elements on the page will be center-aligned, with a red text color:

```
p {
  text-align: center;
  color: red;
}
```

## Id Selector

- The id selector uses the id attribute of an HTML element to select a specific element.

- The id of an element is unique within a page, so the id selector is used to select one unique element!

- To select an element with a specific id, write a hash (#) character, followed by the id of the element.

**Example**

- The CSS rule below will be applied to the HTML element with id="para1":

```
#para1 {
  text-align: center;
  color: red;
}
```

> Note: An id name cannot start with a number!

## Class Selector

- The class selector selects HTML elements with a specific class attribute.

- To select elements with a specific class, write a period (.) character, followed by the class name.

**Example**

- In this example all HTML elements with class="center" will be red and center-aligned:

```
.center {
  text-align: center;
  color: red;
}
```

> You can also specify that only specific HTML elements should be affected by a class.

**Example**

- In this example only <p> elements with class="center" will be red and center-aligned:

```
p.center {
  text-align: center;
  color: red;
}
```

> HTML elements can also refer to more than one class.

**Example**

- In this example the <p> element will be styled according to class="center" and to class="large":

```
<p class="center large">This paragraph refers to two classes.</p>
```

> Note: A class name cannot start with a number!

## Universal Selector

- The universal selector (\*) selects all HTML elements on the page.

**Example**

- The CSS rule below will affect every HTML element on the page:

```
* {
  text-align: center;
  color: blue;
}
```

## Grouping Selector

- The grouping selector selects all the HTML elements with the same style definitions.

- Look at the following CSS code (the h1, h2, and p elements have the same style definitions):

- To group selectors, separate each selector with a comma.

**Example**

- In this example we have grouped the selectors from the code above:

```
h1, h2, p {
  text-align: center;
  color: red;
}
```

# CSS Specificity

- If there are two or more CSS rules that point to the same element, the selector with the highest specificity value will "win", and its style declaration will be applied to that HTML element.

- Think of specificity as a score/rank that determines which style declaration is ultimately applied to an element.

- Every CSS selector has its place in the specificity hierarchy.

- There are four categories which define the specificity level of a selector:

1. Inline styles - Example: <h1 style="color: pink;">
2. IDs - Example: #navbar
3. Classes, pseudo-classes, attribute selectors - Example: .test, :hover, [href]
4. Elements and pseudo-elements - Example: h1, ::before

## Specificity Calculator

https://specificity.keegan.st/

## The !important Rule

- The !important rule in CSS is used to add more importance to a property/value than normal.

- In fact, if you use the !important rule, it will override ALL previous styling rules for that specific property on that element!

### Important About !important

- The only way to override an !important rule is to include another !important rule on a declaration with the same (or higher) specificity in the source code - and here the problem starts! This makes the CSS code confusing and the debugging will be hard, especially if you have a large style sheet!

- Here we have created a simple example. It is not very clear, when you look at the CSS source code, which color is considered most important:

**Example**

```
#myid {
  background-color: blue !important;
}

.myclass {
  background-color: gray !important;
}

p {
  background-color: red !important;
}
```

> Tip: It is good to know about the !important rule. You might see it in some CSS source code. However, do not use it unless you absolutely have to.
