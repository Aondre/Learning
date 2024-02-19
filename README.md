# Learning CSS Folder

## CSS Topics

1. Selectors
2. Colors
3. Units & Sizes
4. Box Model
5. Typography
6. Styling Links
7. List Styles
8. Mini Project
9. Display
10. Floats
11. Columns
12. Position
13. Flexbox
14. Grid Layout
15. Images
16. Media Queries
17. Card Project
18. Pseudo
19. Variables
20. Functions
21. Animations
22. Organization
23. Final Project

## CSS Notes

What is CSS? Cascading Style Sheets is a stylesheet language used to describe the presentation of a document written in HTML or XML (including XML dialects such as SVG, MathML or XHTML). CSS describes how elements should be rendered on screen, on paper, in speech, or on other media.

You can get CSS styles from a few different sources: External Style Sheets, styles that are defined in the header, & styles that are defined inline.
The browers will take the inline styles over the other 2. Depending on if you define the style in header before you reference the external style sheet will determine which takes precendent.

Anatomy of a CSS ruleset:
`p {
color: red;
}`

p = Selector

color = Property

red = Property Value

color: red = Declaration

Ruleset is often referred to as rule.

A way to validate CSS files is to use a CSS Validation Service like: https://jigsaw.w3.org/css-validator/

Best not to use id for CSS. Rare to never. Use classes instead. If you want to specify a specific element, there are different ways to do that.

You can group selectors with a comma: h1, h2, p, div {property: propert value}
If you want to target a nested element use: div h1 {property: property value}

Universal selector \*. It's rarely used outside of CSS reset.

CSS works top down (like a cascade). If define a rule at order 1 & then define again further down the cascade, the rule down the cascade will override the initial ruleset. Classes are an exception to this.
