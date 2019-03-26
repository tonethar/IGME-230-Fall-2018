# Project 2 - Web Service Application

## I. Overview

For this project you (and optionally a partner) are creating a JavaScript driven Web application that utilizes a Web service.
- Your goal is to create an application that is easy to use, functional, and aesthetically pleasing.
- Ideally the experience will run in all modern browsers, but at a bare minimum it must run in recent versions of Chrome.
- The objective of this project is for you to demonstrate your mastery of HTML5/CSS/JS programming in a [web browser DOM](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction) context. 
- You will be evaluated on:
    - your creativity
    - the quality of the experience you create
    - the soundness of your programming
    - how far you went beyond what we did in class, as described below
    
- Resources:
    - Our entire Web apps series: [Web Apps 0 - About this Web App Tutorial Series](https://github.com/tonethar/IGME-230-Master/blob/master/notes/web-apps-0.md)
   - This HW pulls together most of what you need to know into a working example -> [GIF Finder HW](https://github.com/tonethar/IGME-230-Master/blob/master/notes/HW-gif-finder.md) 
   - Here are some working web service examples for you to look at - you can use any of these APIs in your project except for GIPHY: [web-service-app-starters.md](https://github.com/tonethar/IGME-230-Master/blob/master/notes/web-service-app-starters.md)
   - https://developer.mozilla.org/en-US/docs/Web/JavaScript

## II. Requirements

### A. Functional
1. Your application will utilize a web service from this list:
    - https://github.com/toddmotto/public-apis
        - try to use an API that supports *CORS* (Cross-origin resource sharing) - if the API says **NO** in the **CORS** column then it will definitely **NOT work** for this project
        - **DO NOT** use any API that requires *OAuth* authentication
        - if an API requires an API Key, be sure that there is a "free tier", and that the API does not have a short trial period
    - You may optionally utilize an API from this list (although these have not been as extensively curated):
      - https://github.com/abhishekbanthia/Public-APIs
    - Finally, these APIs will definitely work, and there is code to get you started (although you are not allowed to use the GIPHY API for this project): [web-service-app-starters.md](https://github.com/tonethar/IGME-230-Master/blob/master/notes/web-service-app-starters.md)
    - Here are the "Blacklisted" APIs that you **MAY NOT** use for this project:
      - Any API from GIPHY - https://developers.giphy.com/docs/
      - The iTunes Search API - https://affiliate.itunes.apple.com/resources/documentation/itunes-store-web-service-search-api/
- **Important note:** Most of the "sports score" APIs have strict rate limits and/or short trial periods. In the past, most students attempting to use these APIs on their projects ended up having to change their project idea to something else at the last minute. Use such APIs at your own risk.

2. You will save the last term searched by the user in the browser local storage - this was covered here: [Web Apps 9 - WebStorage API](https://github.com/tonethar/IGME-230-Master/blob/master/notes/web-apps-9.md):
    - we are going to test this capability by typing in a search term, doing a search, and then closing the browser window. When we re-open the window, the user's last search term should still be in the field.
    - ideally this will also be true of the other controls, but we won't require it.

3. Required controls - there will be a MINIMUM of 3 controls that a user can use to filter and display the results. Search buttons or similar don't count towards the 3 controls. For example, GIF Finder has these controls:
    - a search button (which doesn't count)
    - a search term field (&lt;input>) that the user types into
    - a pulldown (&lt;select>) that the user can use to limit the number of results

  -  **So you will need at least one additional kind of control. What kind of control to use depends on what parameters the web service will allow you to search it on. Here are some ideas:**
  
     - a **rating** pulldown - if we had this on the GIPHY HW then a user would be able to choose between viewing "G" and "PG" videos for example
     - a **sort by** pulldown to allow the user to view the results sorted A->Z, Z->A, by date, etc 
     - a **date** chooser to filter the results by date - jQuery has a Datepicker Widget that would help with this -> https://jqueryui.com/datepicker/
     - **next** and **previous** buttons - another really nice option is to allow the user to "page" through large numbers of results. In the GIPHY HW did you notice that we always get the same 100 "cat" GIFs back when we search?
       - This is because there are ***thousands*** of cat GIFs on GIPHY, and if we don't otherwise specify we will always get them returned from the web service starting at index 0, which means we always get the first 100 (index 0-99) back.
       - We can instead write code that requests a higher starting index.
       - In the GIPHY API this can be done by tracking and adding an `offset` value to the query string that is sent over to the API.

4. Finally, there will be no JavaScript errors or exceptions thrown by the app.

### B. Design & Interaction
- Pleasing graphic design:
  - with a custom interface coded in HTML/CSS, by you
  - this interface does not resemble the GIPHY homework's UI
- Widgets are well labeled and follow interface conventions, for example:
  - radio buttons are for mutually exclusive options, checkboxes are for when you want to let the user choose *multiple* options - https://delib.zendesk.com/hc/en-us/articles/203430309-Radio-button-vs-checkbox-what-s-the-difference-
  
- Users should be able to figure out how to use the app with minimal instruction:
  - be sure to provide instruction and tooltips if necessary
- User errors must be handled gracefully:
  - for example, if the user forgets to type in a search term before clicking the Search button, the app should tell the user something like "Please enter a search term first"
- Users must know what *state* the app is in at all times:
  - for example, when they click the search button, there should some indication that a search is happening:
    - text that says "Searching for 'Tacos' near you" and so on
    - a "spinner" or other "indeterminate progress" animation - [Google search "indeterminate progress"](https://www.google.com/search?q=indeterminate+progress&client=safari&rls=en&source=lnms&tbm=isch&sa=X&ved=0ahUKEwj-sNCal4neAhVr34MKHWKqA98Q_AUIDigB&biw=1036&bih=583)
    - here are some "spinner" images you could use (show them when the search starts, and hide them when the search ends): http://ajaxloaders.net/2012/10/spinner-loading-animations-set-1/
- While the app doesn't need to be fully responsive, it should look good on a range of displays. For example, don't design it just to work on your huge 24" screen at home (as I'll be grading it on a laptop with a much smaller screen). The main controls of the application must fit in a 1024x768 window.
- You are allowed and encouraged to use a CSS framework for this project - see below!

### C. HTML/CSS & Media
- Valid HTML5 - https://validator.w3.org
- Valid CSS - https://jigsaw.w3.org/css-validator/
- Most CSS is in an external style sheet.
- Use HTML5 semantic and structural elements where practical.
- Images are properly optimized for Web delivery.
- you ARE allowed to use CSS frameworks on the UI for this (and future) projects, such as:
    - http://getbootstrap.com
    - http://materializecss.com
    - https://purecss.io
    - https://github.com/troxler/awesome-css-frameworks


### D. Code Conventions
- All code is an external JavaScript file - inline event handlers are not allowed
- `let` and `const` must be used to declare variables (no `var`!)
- `querySelector()` and `querySelectorAll()` must be used for DOM traversal (DO NOT use the older methods)
- D.R.Y. - Don't Repeat Yourself. Repeated blocks of nearly identical code must be factored out and placed in a separate function.
- Variable and function names must begin with a lowercase letter.
- Well-commented code. Each and every function gets a comment indicating what it does.
- Delete or comment out any `console.log()` calls.

## III. Milestones
- Project proposal with mockup - see myCourses for due date/time. One submission per team please. Make sure both team members' names are included.
- Final project deliverable - see myCourses for due date/time. One submission per team please. Again, make sure both team members' names are included.

## IV. Documentation
- As with Project 1, include a Documentation page (put the link in the comments field of the dropbox, as well as an easy to find link in the project site itself) where you document your process, cite any sources, tell me where to find anything special you want me to see, and also explain how you met the requirements. Finally, give yourself a grade for the project that you feel fairly represents what its worth.
- If you worked in a team, explain what each team member did. Remember, everyone is responsible for contributing throughout the project, not just to one aspect.

## V. Grading
- *Both* partners must contribute *both* JavaScript code AND HTML/CSS to the project. This is NOT a project where team members are allowed to specialize into "Art Director" and "Software Developer" roles! Both team members shall be "Artist/Coders" (doing both) for this project.

Your project will be graded on the following criteria:  
(note:  This rubric is subject to change prior to 3/30/2019, after that date, it will no longer change)

| Criteria | Weight | Your Score |
| -------- | ------ | ---------- |
| **Functionality** | **40** | |
|  - Is useful and/or entertaining | |
|  - Demonstrates creativity | |
|  - Runs without errors | |
|  - *Does not remember last search term* | *(-10)* |
|  - *Missing controls* | *(-15 each)* |
| **Design & Interaction** | **20** | |
|  - Visual design is pleasing | |
|  - Interface is clear and well labeled | |
|  - Standard interface conventions followed | |
|  - The *state* the application is in is obvious | |
|  - Prevents and handles errors well | |
|  - *Interface looks like GIF Finder HW* | *(-10)* |
|  - *Interface "broken" at 1024x768 or lower resolutions* | *(-10)* |
| **HTML/CSS/Media**  | **10** | |
|  - HTML and CSS validate | |
|  - CSS is primarily in a single external stylesheet | |
|  - Makes proper use of structural tags, etc. | |
|  - *Image dimensions and/or file size unnecessarily large* | *(-5)* |
| **Code**  | **10** | |
|  - Code is well formatted and commented | |
|  - Code is located in an external JavaScript file | |
|  - Code follows coding standards detailed above | |
| **Documentation** | **10** | |
| **Above and Beyond (see below)** | **10** | |
| **Possible Total Points** | **100** | |
| Deduction if proposal is not submitted to dropbox on time | -10 | |

Note:
- **Good** (Meet all requirements above reasonably well) = 90%
- **Better** (Go beyond expectations in 2 or more areas) = 95%
- **Best** (Go significantly beyond expectations in 2 or more areas) = 100%

## VI. Submission
- ZIP and post the completed project and documentation page to to the mycourses dropbox
- Post the project to Banjo and link it from your 230 home page

<hr><hr>

**[Table of Contents <- About this Web App Tutorial Series](../notes/web-apps-0.md)**
