# Project 4 - Sprite-based Game or Experience

## I. Overview
*Using PixiJS, create an Interactive Game or Rich Media "experience"*:

- For this project you (and optionally a partner) are creating a JavaScript-driven game or experience, as you outlined in Project 1
- You will be updating/re-writing your web site from Project 1 to reflect the game/experience you intend to create (in other words, you are allowed to change your original idea)
- If you would like to see examples of previous projects, check out the Project 4 links on the [week-01A-notes.md](../weekly/week-01A-notes.md#project4examples) page

You will use **ONE** of these technology stacks:
- **JavaScript & PixiJS** (which wraps WebGL): 
    -  [About this PixiJS Tutorial Series](https://github.com/tonethar/IGME-230-Master/blob/master/notes/pixi-js-0.md) has links to the [Circle Blast!](HW-circle-blast-1.md) exercise and other demos that can get you started **OR**
- **JavaScript & the Browser DOM** - these exercises will give you an idea of what is possible, and also represent some nice "starter" code:
    - [DOM Adventure!](https://github.com/tonethar/IGME-230-Master/blob/master/notes/HW-adventure.md) is a tile-based game that uses arrow keys for movement, and simple sound
    - [DOM Chibi Matching](https://github.com/tonethar/IGME-230-Master/blob/master/notes/HW-chibi-matching.md) is a card matching game that uses CSS animations
    - [DOM Life](https://github.com/tonethar/IGME-230-Master/blob/master/notes/HW-life.md) is a tile-based game that explores simple [cellular automata](https://en.wikipedia.org/wiki/Cellular_automaton)
    - [Magentic Poetry](https://github.com/tonethar/IGME-230-Master/blob/master/notes/HW-magnetic-poetry.md) uses CSS transforms and absolute positioning, and mousemove events

- **IMPORTANT: YOU MAY NOT USE THE CANVAS 2D DRAWING API FOR THIS PROJECT - DOING SO WILL RESULT IN A GRADE OF ZERO**

- **IMPORTANT: THIS PROJECT NEEDS TO BE _YOUR WORK_:**
    - If you are using *Circle Blast!* or another game we gave you as a template, be sure to "change it up" and go well beyond what we gave you in the start code. Think about changing the game genre, control system, and how the opponents behave. We are only going to give you credit for the code you wrote, so if 90% of your submission is the same as one of our in-class exercises, you are going to get very little credit for the coding and functional sections of the rubric
    - You must change the fonts, graphics, spritesheets, and sounds from what we gave you in the starting exercises. If you simply reuse what we gave you, points will be deducted in the design and interaction section of the rubric
    - One reason for the above is that we want you to have a potential portfolio piece that you can show employers, and if your project just looks like the in-class exercises that everyone else is showing them, then you will likely not get the position


## II. Goal
- Your goal is to use one of the tech stacks above to create an interactive media experience or game that is easy to use, functional, and aesthetically pleasing.

- Ideally the experience will run in all modern browsers, but at a bare minimum it must run in recent versions of Chrome.

- You will be evaluated on:
    - your creativity
    - the quality of the experience you create
    - the soundness of your programming in your chosen tech stack
    - how far you went beyond what we did in class, as described below

## III. Requirements

### A. Functional
- You will use one of the above tech stacks above as your underlying graphics engine
- Your game or app should do something useful, and be easy to use
- The functionality goes beyond what we have done in similar in-class examples
- There will be no JavaScript errors or exceptions thrown by the app
- You must utilize an additional HTML5 feature, like localStorage (for high scores), drag and drop, or location services

### B. Design & Interaction
- Pleasing graphic design
- Widgets are well labeled
- User should be able to figure out how to use the app with minimal instruction (and be sure to provide instruction and tooltips if necessary!), and user errors are handled gracefully
- While it doesn't need to be responsive, it should look good on a range of displays; don't design it just to work on your huge screen at home. If a 1024 x 768 display can't show the whole layout, it's a problem

### C. Media
- Images are properly optimized for web delivery - e.g. cropped and scaled to appropriate dimensions, and saved as a JPEG or PNG
- Sound is used to enhance the experience
- you have changed the fonts, graphics, spritesheets, and sounds from what was provided in the in-class examples

### D. HTML/CSS
- Valid HTML5 - https://validator.w3.org
- Valid CSS - https://jigsaw.w3.org/css-validator/
- Most CSS is in an external style sheet
- Use HTML5 semantic and structural elements where practical

### E. Code Conventions
- `let` and `const` (no `var`!)
- `querySelector()` and `querySelectorAll()` for DOM traversal (DO NOT use the older methods)
- Utilize at least one ES6 `class` of your own creation
- D.R.Y. - Don't Repeat Yourself. Repeated blocks of nearly identical code should be factored out and placed in a separate function.
- Separation of Concerns. Similar to how the *Circle Blast!* HW was structured, have a separate .js file for your classes, utility functions, and main code. If you have more than 3 CSS rules, then put them in an external stylesheet
- Variable and function names must begin with a lowercase letter
- Well-commented code. Each and every function gets a comment indicating what it does
- Delete or comment out your `console.log()` calls

## IV. Milestones
- Proposal: Update your site from Project 1 to reflect what you are building for this project - see MyCourses dropbox for the due date
- Checkpoint: create a working draft of the project - see MyCourses dropbox for the due date
- Final project deliverable is due during our scheduled finals week meeting - see MyCourses dropbox for the due date and submission instructions. Be sure to post the project to the web, and put the link in the comments field of the mycouses dropbox.
- At our scheduled final exam time, we will have a show and tell of your projects (see below)

## V. Documentation
- Update the documentation on your Project 1 site to include your process for this project, cite any sources, tell me where to find anything special you want me to see, and also explain how you met the requirements
- If you worked in a pair, explain what each team member did. Remember, everyone is responsible for contributing throughout the project, not just to one aspect

## VI. Presentation
At the time of our scheduled meeting during finals week, you will present your project to the class in a brief demo. **Attendance for this is mandatory.** For this demo, show us:
- What you made
- What's cool, and what you think is "above and beyond"
- How you overcame any serious challenges
- Resources utilized (for libraries, tutorials, etc.), if you used any

## VII. Grading
- *Both* partners must contribute equally to the project. This is NOT a project where team members are allowed to specialize into "Art Director" and "Software Developer" roles! Both team members shall be "Artist/Coders" (doing both) for this project.

Your project will be graded on the following criteria:

| Criteria | Weight | Your Score |
| -------- | ------ | ---------- |
| **A. Functionality** | **30** | |
|  - Is useful and/or entertaining | |
|  - Demonstrates creativity | |
|  - Uses an additional HTML5 technology | |
|  - Runs without errors | |
|  - Functionality is either distinct from the in-class examples, or goes significantly beyond them in scope | |
| **B. Design & Interaction** | **20** | |
|  - Visual design is pleasing | |
|  - Sound (both incidental and background) enhances the experience | |
|  - Interface is clear and well labeled | |
|  - Prevents and handles errors well | |
| **C. and D. Media/HTML/CSS**  | **10** | |
|  - Optimized Images | |
|  - HTML and CSS validate | |
|  - CSS is primarily in a single external stylesheet | |
|  - Makes proper use of structural tags, etc. | |
|  - Media (sound, fonts, images, etc) has been changed from what was provided in class | |
| **E. Implementation and Code** | **20** | |
|  - Code is well formatted and commented, and follows coding standards | |
|  - Code is logically broken out into separate JS files | |
|  - Code is distinct from, and/or goes beyond what we have done in class | |
| **Above and Beyond (see below)** | **10** | |
| **Presentation** | **10** | |
| **Possible Total Points** | **100** | |
| Deduction if proposal is not updated on time | -20 | |
| Deduction if prototype is not submitted on time | -20 | |
| Deduction if final documentation is not submitted on time | -20 | |

Note for "above and beyond":
- **Good** (Meet all requirements above reasonably well) = 90%
- **Better** (Go beyond expectations in 2 or more areas) = 95%
- **Best** (Go significantly beyond expectations in 2 or more areas) = 100%
