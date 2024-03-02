# Learning CSS Folder

## CSS Topics

1. Selectors
   Anatomy of a CSS ruleset:
   `p { color: red;}`
   p = Selector

   color = Property

   red = Property Value

   color: red = Declaration

   Ruleset is often referred to as rule.

   What is CSS? Cascading Style Sheets is a stylesheet language used to describe the presentation of a document written in HTML or XML (including XML dialects such as SVG, MathML or XHTML). CSS describes how elements should be rendered on screen, on paper, in speech, or on other media.

   You can get CSS styles from a few different sources: External Style Sheets, styles that are defined in the header, & styles that are defined inline.
   The browers will take the inline styles over the other 2. Depending on if you define the style in header before you reference the external style sheet will determine which takes precendent.

   A way to validate CSS files is to use a CSS Validation Service like: https://jigsaw.w3.org/css-validator/

   Best not to use id for CSS. Rare to never. Use classes instead. If you want to specify a specific element, there are different ways to do that.

   You can group selectors with a comma: h1, h2, p, div {property: propert value}
   If you want to target a nested element use: div h1 {property: property value}

   Universal selector \*. It's rarely used outside of CSS reset.

   CSS works top down (like a cascade). If define a rule at order 1 & then define again further down the cascade, the rule down the cascade will override the initial ruleset. Classes are an exception to this.

2. Colors
   There 140 color names recognized by HTML. For setting backgroun colors, you can use background-color or background property (the shorthand comes with other choices)
   Font color can be changed with the color property.
   RGB (Red, Green, Blue) is a way we use to set color by utilizing values from 0 & 255: rgb(255, 0, 0). If you set r to 255 & the other values to 0. you'll get the red color. If you do the same for g, you'll get green. Do the same for b and you'll get blue.
   RGBA is the same as RGB but the a refers to alpha or the transparency. This value is anything between 0 & 1 and sets the transparency of the element that's targeted.
   Hexadecimal is another way to set colors. It uses numbers 0-9 and letters A-F. You can use a combination of numbers & letters.
   HSL is another way to set colors & it stands for Hue, Saturation & Lightness. hue gives the color, saturation gives off grey to the full color & lightness gives out the light to dark version of the color. The max value for Hue is 360.
   There a couple of tools that I can use for choosing color pallets and checking contrast; Coolors.co (https://coolors.co/) does both, while https://webaim.org/resources/contrastchecker/ is a contrast checker.

3. Units & Sizes
   For CSS there are several absolute length units: cm [Centimeter] (1cm = 37.8px = 25 2/64inch), mm [Millimeter] (1mm = 1/10th of 1cm), Q [Quater-millimeter] (1Q = 1/40th of 1cm), in [Inch] (1in = 2.54cm = 96px), pc [Picas] (1pc = 1/6th of 1in), pt [Points] (1pt = 1/72th of 1in), & px [Pixel] (1px = 1/96th of 1in). For CSS Pixel will be the absolute value most commonly be used.
   In general we don't want to use an absolute value because we want the users to be able to adjust things like font size. Using absolute values on something like borders is fine.
   We can use percentage (%) to set the size of things like width or height.
   Relative length uits; are relative to something else. em (Font size of the parent, in the case of typographical properties like font-size, and font size of the element itself, in the case of other properties like width.), ex (x-height of the element's font.), ch (The advance measure (width) of the glyph "0" of the element's font.), rem (Font size of the root element.), lh (Line height of the element), rlh (Line height of the root element. When used on the font-size or line-height properties of the root element, it refers to the properties' initial value.), vw (1% of the viewpot's width), vh (1% of the viewport's height), vmin (1% of the viewport's smaller dimension), vmax (1% of the viewport's larger dimension), vb (1% of the size of the initial containing block in the direction of the root element's block axis.), vl (1% of the size of the initial containing block in the direction of the root element's inline exis.), svw/svh (1% of the small viewport's width and height, respectively), lvw/lvh (1% of the large viewport's width and height, respectively), dvw/dvh (1% of the dynamic viewport's width and height, respectively).
   We'll typically use rem to set font-size and rem refers to the root element which is defined by the browser.
   Using em, which set the size relative to the parent element.
   Good rule of thumb so far: use rem for font-size, then use em for margin & padding.
   You can use ch to help define columns. ch will set the character limit of each line.

   CSS reset:
   `*{margin: 0; padding: 0; box-sizing: border-box}`

   Note: when using 100vw, a problem arises vertically. If you content that extends the viewport beyond a 100vh it will create a horizontal scroll bar to account for the "extra" viewport width created by the vertical scroll bar. You can fix by using % instead of vw. No need to set 100% on the body because it should default to that.

4. Box Model
   Box Model: Content > Padding > Border > Margin
   CSS reset V2.0:
   `*{margin: 0; padding: 0; box-sizing: content-box}` don't use content-box because it will end calculating extra spacing to your overall size/padding/margin schema.
   The margin property is short-hand for margin-top, margin-right, margin-bottom, & margin-left and you can set the margins for each side in that order. example:
   `{margin: 1rem 1.5em 1.25rem 1.45em}` is the same as
   `{margin-top: 1rem; margin-right: 1.5em; margin-bottom: 1.25rem; margin-left: 1.45em}`
   The padding property is also short-hand with the same options as margin for p-top, p-right, p-bottom, p-left.
   The border property also similar to margin & property but there are a few extra options: line type & color
   There's also the outline property and it's added right outside (around) the border but it doesn't get calculated in the box model breakdown.
   Outline-offset pushes the outline from the border. If you use negative value, the outline will go inside the border.
   For margin, if you set the left & right value to auto: margin: 3rem auto, it will center the element horizontally in the center of the parent element.
   Setting your border-radius to half of the height/width of an element will create a circle element. Best if the height/width of that element is equal.

5. Typography
   Typography is the way text is arranged and presented.

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

Another tool that will help in my CSS journey: specifity Calculator (https://specificity.keegan.st/)
