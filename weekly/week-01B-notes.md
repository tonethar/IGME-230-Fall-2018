# Week 1B - Review of *banjo.rit.edu* & FTP

## Topics
- FTP review
- Setting up your `230` directory
- Scripting the server with `.htaccess` files

## I. FTP Demo
FTP demo and review (we will do this together in class):
   - Create a local 230 directory, and put a *hello.html* file in it
   - **Reminder:** always keep backups, bring a flash drive to class; the `230` folder on people.rit.edu is where course work will usually be posted

**hello.html**
```
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="utf-8" />
	<title>Hello Page</title>
</head>
   <body>
      <h1>Week 1 in 230!</h1>
      <p>I am stoked about this class!</p>
   </body>
</html>
```
 
1. connect to `banjo.rit.edu` with an FTP client - instructions are here: [How to post to RIT's *banjo* web server](../notes/posting-to-banjo.md)
1. create a `230` folder and place it in your `www` folder
1. post `hello.html` to your banjo `230` folder
1. review file/folder permissions to be sure they are correct
1. **Reminder:** `banjo.rit.edu` is the FTP name, but the browser will access the URL `people.rit.edu`
1. navigate a browser to that directory - `http://people.rit.edu/~abc1234/230/hello.html` and you should see your *hello.html* page
1. remember CSS? Let's add some CSS style rules to the page!

## II. htaccess Demo
*A .htaccess ("hypertext access") file is a directory-level configuration file supported by the major web servers, used for configuration of site-access issues, such as URL redirection, URL shortening, Access-security control (for different webpages and files), and more.*

In class, let's "demo first" what .htaccess files can do. We will look at the following htaccess directives:

1. `DirectoryIndex hello.html` - makes the default file for the folder *hello.html* rather than *index.html*
2. `Options -Indexes` - turns off file listing for folders so that users can't see your files and folders directly
3. `Header add X-HeaderName "Header Value"` - sends a custom header. `X-` is a convention used for naming non-standard headers
4. `Redirect /~acjvks/230/hello.html http://www.rit.edu` - redirects the browser from a file to another domain
5. `Redirect /~acjvks/230/ /~acjvks/110/` - redirects the browser from a folder, to a different folder
6. `ModPagespeed off` - turns off the ModPagespeed extension

## III. Presentation
- [Auth and htaccess PDF](../docs/Auth_and_htaccess.pdf)

## IV. Exercises
See mycourses dropboxes for due dates:
- ["Fixing Banjo" instructions](../exercises/week-1/Fixing-Banjo.md)
- [Custom 404 Pages and Authentication files (ZIP)](../exercises/week-1/Custom_404_Auth_start.zip)

## V. Reference
- Banjo Authentication Docs: https://www.rit.edu/webdev/authenticating-and-authorizing-rit-users
- Advanced Scripting with .htaccess files: https://www.askapache.com/htaccess/
- https://en.wikipedia.org/wiki/List_of_HTTP_status_codes
- https://sitesdoneright.com/blog/2013/03/what-is-418-im-a-teapot-status-code-error

<hr><hr>

[<-- Back to IGME-230 Schedule](../schedule.md)

