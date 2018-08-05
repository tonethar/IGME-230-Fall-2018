# Week 1A: Course Introduction & Intro to HTTP Protocol
Welcome to the course!

## I. Overview
Welcome to IGME-230 Web Site Design & Implementation! There is more to this course than the title implies, as we will be learning a lot more than just the design and implementation of static web sites. 
Hopefully the skills you acquire in the class will help you to get a co-op position, and give you the skills you need to create "passion pieces" for your professional portfolio.


## II. Prerequisites
Students in this class should have a basic working knowledge of HTML, CSS, and publishing to RIT's web hosting environment (people.rit.edu). This material was covered in IGME-110. You can review much of that material here: [IIM-Web-Review/](../IIM-Web-Review)

If you need to brush up on your HTML and CSS skills, I recommend using the CodeAcademy tutorials that we currently use in IGME-110:  -  [Lynda.com HTML Essential Training, Lessons 1-7](https://www.lynda.com/HTML-tutorials/HTML-Essential-Training/170427-2.html?org=rit.edu). We will be doing a very brief review, but you shouldn't expect to rely on that to cover all of the prerequisite knowledge.

You will also need a GitHub account, and the [GitHub Student Developer Pack](https://education.github.com/pack) so that you can create and access private repos.

If you have questions between now and the start of class, feel free to send me an email! 

## III. What this course is about
Official description from SIS: *This course provides an introduction to web development tools and technologies, such as HTML, CSS, Javascript and DHTML, AJAX, web platforms and environments, and server-side programming methods.*
We will:
* review basic **web publishing** (HTML/CSS/FTP) and HTML validation
* learn **how a web server works** and how to do basic scripting of it
* expose you to the PHP scripting language that runs on most web servers
* explore advanced CSS layout utilizing the CSS box model and the latest specifications
* go beyond *type*, *class*, and *id* CSS selectors by utilizing advanced CSS 3 selectors
* learn how to add **advanced interactivity** to web pages. Building web apps and web games requires knowledge of more than just HTML & CSS, but also of the JavaScript programming language that runs in all web browsers. We will be covering the current "standard" version of JavaScript known as ES5 (ECMAScript 5), as well as some of the well-supported and powerful features of ES6 (AKA ECMAScript 6 or ECMAScript 2015)
* construct **web applications**. A web app is a client–server software application in which the client (or user interface) runs in a web browser. Examples of web apps you might use are github.com, Gmail, and Google Drive. Web App assignments we will complete in class include:
    - an [Image Gallery](../notes/HW-image-gallery.md)
    - an app that allows the user to search for and [view animated GIFs](../notes/HW-gif-finder.md)
    - a [Pixel Art](../notes/HW-pixel-artist.md) application
* construct **interactive games** that run in the web browser (these are also considered to be web applications):
  * utilizing the DOM (Document Object Model) and modern CSS features we will build:
      - an [interactive concentration game](../notes/HW-chibi-matching.md)
      - an [adventure game](../notes/HW-adventure.md)
      - and a [Conway's game of Life simulation](../notes/HW-life.md)
  * utilizing the Pixi.js rendering framework, we will build sprite-based games such as [Circle Blast!](../notes/HW-circle-blast-4.md)
* utilize a **CSS framework** such as [Bootstrap](http://getbootstrap.com) or [Skeleton](http://getskeleton.com) to construct a **responsive web portfolio**
When the course is complete, you will hopefully have at least the beginnings of a "portfolio piece" or two that you will be able to show to prospective employers.
  
## IV. Discussion
This course is not focused on "web design", but instead on developing highly interactive web applications and web games that heavily utilize the JavaScript programming language.  The major topics of this course are split roughly into thirds:
1. web publishing (HTML/CSS) both "from scratch" as well as with the Bootstrap or Skeleton CSS framework
2. web application development (HTML/CSS/JavaScript & a little PHP)
3. web game development (JavaScript & the Pixi.js rendering engine)

Once you complete this course you should be able to do the following:
- publish a "traditional" multi-page website to the web. The content will be properly "chunked" and the site navigation will be intuitive and easy to use.
- publish a single-page application (SPA) web site portfolio. You can see an example here: http://dougwatro.com - this example has eight distinct "pages" of content that are presented on a single web page.
- code a web application that can connect to web services, and download/display their data.
- code a DOM web game that uses HTML/CSS for the User Interface, and JavaScript for game logic & interactivity.
- code a sprite-based game such as a shooter or platformer utilizing JavaScript and PixiJS. 

## V. <a id="section5"></a>Projects and other stuff for inspiration
There are a lot of reasons to improve your web development skills. Think about how much you use the Web every day, and how integrated it is into the games and new media interactive development fields. Games on the Web are pretty big right now. Also, it's a fantastic medium for showing off your work to the world, including potential employers!

Past Student Portfolios:
- http://katiepustolski.com/
- http://brianemling.com/
- http://dougwatro.com

Some sample IGME-230 projects from last year:
- Portfolio:
    - http://barringtoncampbell.com/
    - https://people.rit.edu/mxb9517/portfolio/
    - https://people.rit.edu/ctb4332/portfolio/
    - https://people.rit.edu/mac9406/portfolio/
    - https://people.rit.edu/sxf5282/portfolio/
    - https://people.rit.edu/sml6783/230/portfolio/
    - https://people.rit.edu/lpn4937/portfolio/
    - https://people.rit.edu/djs5435/portfolio/
    - https://people.rit.edu/jds7523/portfolio/
    - https://people.rit.edu/drs4149/portfolio/
    - https://people.rit.edu/ekt6170/portfolio.html
    - https://people.rit.edu/axw1799/portfolio/
    - https://people.rit.edu/wjb5377/230/portfolio/
- DOM Game or App (Project 2)<a id="project2"></a>:
    - https://people.rit.edu/mac9406/230/project2/index.html
    - https://people.rit.edu/~kts6823/230/project2/index.html
    - https://people.rit.edu/lpn4937/230/project2/minesweeper.html
    - https://people.rit.edu/~deb2610/230/project2/PixelPainterExtended.html
    - https://people.rit.edu/btf6119/230/projects/2/index.html
    - https://people.rit.edu/dso2890/230/projects/project2/index.html
    - https://people.rit.edu/djs5435/230/project2/
    - https://people.rit.edu/~wcd7037/230/Project2/Life/pixel-life.html
    - https://people.rit.edu/paa9307/230/project2/
    - https://people.rit.edu/axs6207/230/project2/musicFinder.html
    - https://people.rit.edu/arw2013/WhoSays/whoSays.html
- PixiJS Sprite Game (Project 3)<a id="project3"></a>:
    - https://people.rit.edu/~jpa3216/230/project1/
    - https://people.rit.edu/~hhn2884/230/project1/
    - https://people.rit.edu/mro5772/230/project1/PlayGame
    - https://people.rit.edu/~txm1918/230/project1/index.html
    - https://people.rit.edu/djs5435/230/project1/project3/project.html
    - https://people.rit.edu/~jds7523/230/project1/project.html
    - https://people.rit.edu/axw1799/Bananagans/Bananagans/game.html
    - https://people.rit.edu/axs6207/230/project3/project.html
    - https://people.rit.edu/scr3876/230/project1/project.html
    - https://people.rit.edu/cke1622/230/Project_3/game.html
    - https://people.rit.edu/~ctq6891/230/projects/project1/project.html
    - https://people.rit.edu/tmh6112/230/project3/project.html
    - https://people.rit.edu/~deb2610/230/project1/project.html
    - https://people.rit.edu/sxf5282/230//project1/project.html
    - https://people.rit.edu/mxr2091/230/finalproject/game.html
    - https://people.rit.edu/ngm9939/230/project1/game.html
    - https://people.rit.edu/~wcd7037/230/Project1/project.html
    
And some other really cool stuff:
- http://www.chromeexperiments.com/

## VI. Pedagogy (how this course is taught!)
- A typical classroom day will be:
    - a review of the days topics utilizing powerpoints or our Github lecture notes
    - a live "demo" by the professor that reinforces the day's topics
    - if time remains, students will be able to work on homework assignments
- The assignments given in this class break into two categories:
    - homework assignments/in-class exercises that focus narrowly on one of more concepts
    - Three projects, that are considerably more freeform, and allow you to exercise considerable freedom and creativity in meeting their requirements.
- A large part of this course is taught similar to a typical math course: there will be several small HW assignments given every week, and because these assignments build upon one another, it is essential that they be completed both on-time and in-order, thus they have strict due dates.
- You need to review the week's lecture notes *prior* to attending class for that week
- Keep an eye on the dropboxes in mycourses for what and when things are due. HW assignments will not be accepted late without prior permission from the instructor - if something comes up and you need an extension you need to get in touch with us ASAP before the assignment is due. **Reminder:** *all code files (HTML, CSS, JavaScript) must be zipped when put in a dropbox, because otherwise mycourses strips out the JavaScript and CSS, and you will likely get a zero on the assignment.*
- The due dates for these assignments will be clustered around the same days, often on Monday night. This means that you should plan ahead, and not try to tackle them all in the last hour before they are due.
- Please get to class on time! Lectures will begin promptly at the start of class.

## VII. Required Reading
* [syllabus.md](../syllabus.md)
* [schedule.md](../schedule.md)
* [GitHub's Hello World tutorial](https://guides.github.com/activities/hello-world/)

## VIII. Today's Lecture Notes - Intro to HTTP Protocol
* [http-protocol-intro.md](../notes/http-protocol-intro.md)
* [http-protocol-demo.md](../notes/http-protocol-demo.md)

## IX. Homework
- **Always keep a close eye on the mycourses dropboxes so that you know what's due & when!**
- Get a GitHub account (if you don't have one already), and go through the tutorial above. 
- Set up a repository *for this course* in your account, named *IGME230* or something similar, and put a link to it in the comments field of the myCourses "GitHub Accounts" dropbox. This should be a public repository (otherwise the link won't work).
- Create a `230` folder on `banjo.rit.edu` - put it in your `www` folder and be sure that the permissions are set so that it is web viewable.

## X. Any time left?
- If there is time left today, let's head to the notes for our next class meeting -  [week-01B-notes.md](week-01B-notes.md) - and do a little bit of HTML & FTP review!

<hr><hr>

[Home <-- Back to IGME-230 Schedule](../schedule.md)

[Next Unit --> week-01B-notes.md](week-01B-notes.md)
