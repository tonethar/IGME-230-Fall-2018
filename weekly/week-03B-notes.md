# Week 3B - Review of CSS

## I. Topics & Overview
- Where we can put CSS
- Selectors, IDs, classes, pseudo-classes
- Styles
- Float
- Inheritance
- Validation

## II. Review and Demo
Together, we'll add to our previous Web page, reviewing the following:
- Inline, embedded, and external (linked) CSS
- IDs, classes, pseudo-classes
- Basic styles
- Styling anchor tags
```
a:link{}
a:visited{}
a:active{}
a:hover{}
```
- Inheritance

## III. The CSS Box Model
![BoxModel](../other-files/BoxModel.png)

+ *margin* is space that is "outside the box"
+ *padding* is space that is "inside the box"

## IV. Validation
http://jigsaw.w3.org/css-validator/

## V. Presentations
[Intro to CSS](../presentations/CSS-Intro.pdf)

## VI. Reference
- [Lynda.com: Learning CSS, Sections 1-3](https://www.lynda.com/CSS-tutorials/CSS-Fundamentals/417645-2.html)
- https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors - lot's of nice examples of selectors in action
- https://www.w3.org/TR/css3-selectors - when in doubt, check the spec!

## VII. CSS Selectors you need to know
- CSS Selector Reference - the "spec" - https://www.w3.org/TR/css3-selectors/#selectors
- CSS Selector Tutorial - https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Selectors
- Basic selectors: type,class,id,universal
- rollovers -  `:link`, `:visited`, `:hover`, `:active`
- descendant - `E F`
- child - `E > F`
- adjacent sibling - `E + F`
- general sibling - `E ~ F`
- attribute - `E[foo="bar"]  /* exact match */`
- attribute - `E[foo*="bar"] /* contains */`

## VIII. Exercises
- [CSS Styling - Recipe ICE](../exercises/week-2/Recipe-ICE.zip)
- [230 Home Page](../exercises/week-2/230-home-page.md)

<hr><hr>

[<-- Back to IGME-230 Schedule](../schedule.md)
