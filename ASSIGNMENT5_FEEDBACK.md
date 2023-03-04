Hi Edu!

Very nice work!

As you will see blow I've left a few comments, but you met nearly all the requirements and did a very good job. The only major thing missing is a typography stylesheet, but you have thee correct css in a different file so its a quick fix.

Since the overall level of the assignment is high, I happy to say you've earnt yourself a Välgodkänt grade! Well done! YOU can fix the things below if you needd, but there's no need to resubmit.

I think you should reflect on what you've achieved in this subject, and you should be proud! I know it hasn't been easy at times, but you've shown real determination to learn and that's all you need. It gets easier with every piece of code you write.


*************************************

CRITERIA FOR GRADING

*************************************

GODKÄNT:
-------------------------------------

HTML
  index.html at root level for publishing on github pages ❌

  Multiple pages ✅

  Header, footer and navigational menu on all main pages (where possible) ✅
    project.html loads some bootstrap sass (.scss) that adds padding to .header .container so the header on that page is slightly different to the other pages
    The about page has a different BG colour so the header looks a bit different

  H1 on every page ✅ ❌
    Not of Portfolio3.html or Skills.html

  Mail to Contact form ✅

  Links to specific projects opening in new windows ✅

CSS
  External CSS ✅

  General style sheets for common elements ❌ ✅
    What you did with the header is great, it's in multilevel.css and every page uses it, but the footer code is almost identical in 4 different files.
    It's best to have the default styling in one file, then override what you need in the page specific files.

  Typography style sheet ❌
    The @font-face for Raleway should be moved in to a typograpy.css file.
    In the same file you should also set it as the body font (like you do in multilevel.css line 3) and declare any common styling for heading elements (h1, h2, h3 etc)

  Locally installed font ✅
  
  Separate stylesheets for each page ✅
    Nice!

  RWD
    Desktop ✅
    Mobile ✅
     Looks good!

JS
  jQuery plugin (such as a carousel) ✅

  JS/jQuery multi level menu (min 2 levels) ✅
    Nice! t's a bit confusing because thee level 2 items all link to the same page but I see you just wanted to demo the menu so no problem.

-------------------------------------

VÄLGODKÄNT:
-------------------------------------

  Project organisation ✅
    Great, but you should have an html directory
    Skills.html is empty so should be removed as well as the menu link to the skills page

  CSS prefixing where required ✅

  jQuery effects ❌ ✅
    I was after slide and fades - the built in jQuery effects, but you have nice slide effects on the menu 

  Semantic element naming ✅

  Code style
  A few missing indents, but very good!
   HTML: ✅ ❌
     <script> tags should be in the head section, with a defer property if thy are vanills JS
     <img> tags always should have an alt attribute
     
   CSS: ✅ ❌
     Have a space before the closing måsving }
     Have an empty line between selectors

      body{
	      line-height: 1.5;
	      font-family: 'Raleway', sans-serif;
	      font-weight: 400;
      }
      body.hidden-scrolling{
	      overflow-y: hidden;
      }

    Should be:

      body {
	      line-height: 1.5;
	      font-family: 'Raleway', sans-serif;
	      font-weight: 400;
      }

      body.hidden-scrolling {
	      overflow-y: hidden;
      }
  
   JS: ✅ ❌
     consts should always be written in SNAKE_CASE
     When adding a block of variables, you should indent the lines to match the variable name on the first line:

       const openNavMenu = document.querySelector(".open-nav-menu"),
       closeNavMenu = document.querySelector(".close-nav-menu"),
       navMenu = document.querySelector(".nav-menu"),
       menuOverlay = document.querySelector(".menu-overlay"),
       mediaSize = 991;

     Should be:

       const OPEN_NAV_MENU = document.querySelector(".open-nav-menu"),
             CLOSE_NAV_MENU = document.querySelector(".close-nav-menu"),
             NAV_MENU = document.querySelector(".nav-menu"),
             MENU_OVERLAY= document.querySelector(".menu-overlay"),
             MEDIA_SIZE = 991;