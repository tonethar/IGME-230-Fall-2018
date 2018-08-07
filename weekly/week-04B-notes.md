# Week 4B - Responsive Design and Media Queries

## Topics
- Responsive Design
- CSS Media Queries

Responsive design all boils down to a visual design that responds to the size of a user's device or screen. Flexible, "liquid" layouts are one part of this, but to really optimize the experience for any given device we need to utilize custom CSS for each device. Enter: media queries!

This involves two parts. First, in your CSS:

```
@media screen and (max-width: 480px) {
  */ note that you can target multiple screen widths, using multiple media queries /*
  */ Style rules here that adapt to the smaller screen /*	
} 
```

and then in the head of your HTML:

``` 	
<meta name="viewport" content="width=device-width, initial-scale=1.0"> 
```

## Reference
- http://getbootstrap.com/
- http://www.templatemo.com/

We will look at Bootstrap and other frameworks later, but for now it's nice to see how it does responsive design!

## Media Query Resources
- http://www.w3.org/TR/css3-mediaqueries/
- http://webdesignerwall.com/tutorials/responsive-design-with-css3-media-queries
- http://cssmediaqueries.com/

## Presentations
- [Responsive Design](https://github.com/tonethar/IGME-230-Master/tree/master/presentations/4B-Responsive-Design.pdf)

## Demo
- [Responsive page demo](https://github.com/tonethar/IGME-230-Master/tree/master/other-files/Responsive_Demo.zip)

## Exercise
- [Responsive Design with CSS Media Queries](https://github.com/tonethar/IGME-230-Master/tree/master/exercises/week-4/ICE-ResponsiveCSS.pdf)
- [Responsive Design start files](https://github.com/tonethar/IGME-230-Master/tree/master/exercises/week-4/darth_start_files.zip)

<hr><hr>

| <-- Previous Unit | Home | Next Unit -->
| --- | --- | --- 
| [**week-04A-notes.md**](week-04A-notes.md)     |  [**IGME-230 Schedule**](../schedule.md) | [**week-05A-notes.md**](week-05A-notes.md)

