# Personal_Website
Repository for tinkering with Javascript on Personal Website

1:44 AM July 10 2020
Everything is working. Rations are running low.

3:44 AM July 11 2020
Fixed page width overflow. It was an issue with the row class from Bootstrap. Quoting an answer from stackoverflow: "
***CODE
.container-fluid .row {
    margin-left: 0px;
    margin-right: 0px;
}
CODE***
For some reason when using container-fluid bootstrap doesn't take into account that it is using a negative margin on rows. So by adding the css above it will fix your issue."
I used row within the pageTwo and pageThree classes I made in my CSS. Adding the following style rules to my CSS fixed the width overflow:
***CODE
.pageTwo .row {
    margin-left: 0px;
    margin-right: 0px;
}
.pageThree .row {
    margin-left: 0px;
    margin-right: 0px;
}
CODE***
Source:https://stackoverflow.com/questions/25808485/bootstrap-3-row-too-wide-giving-horizontal-scrollbar


4:23 AM July 11 2020
Fixed the transparency of Navbar without affecting text link transparancy. Was able to do this through utilitizing background-color and rgba in CSS.
Source: https://stackoverflow.com/questions/16943825/css-how-to-change-opacity-of-container-but-not-text

5:15 AM July 11 2020
Fixed Github and Linkedin button text color on page 1. Had to assign ID to page one, then assign text color property to the ID.

5:17 AM July 11 2020
Next things to fix:
*Everything contained in Bootstrap columns has priority on Z-Axis. Example: Profile pic and about me are in front of navbar when scrolling. Same with reserved columns for embedding projects.
*sI font in about me section hard to read?
*Make text more responsive
*Make sure website is responsive for different platforms
*Make logo for tab
*

1:45 AM July 12 2020
Fixed an issue regarding items in Bootstrap column elements taking Z-index priority over the navigation bar. This was fixed by applying a Z-index of 1 to the .sticky class in the CSS and a Z-index of 0 to a newly created .row class in the CSS file. In order for the Z-index attribute to work, a position must also be stated. The .sticky class already had position: sticky. I gave the row class position: relative.


1:49 AM July 12 2020
Fixed white space at bottom of webpage. Was caused by an ending to a comment that I forgot to remove.

2:29 AM July 12 2020
Added an image link to the git repository for the portfolio website.

2:53 AM July 12 2020
May have found out how to set the pageOne div as a video background to give the site a more modern look. Going to focus on applying the block class to the pageFour container first. W3 Schools has an interesting page for embedding videos: https://www.w3schools.com/howto/howto_css_fullscreen_video.asp and there are free stock videos available at https://www.pexels.com/videos/

5:11 AM July 12, 2020
Removed Contact page and moved that information to footer. The footer had links that were already in the navbar so this cuts down on clutter within page. There was white space at the bottom of the footer but that was fixed temporarily by changing footer height from 50px to 60px. Currently working on creating a table to contain education and work experience information on page 1. Also trying to figure out how to have block class work behind the table and paragraph elements.

5:46 AM July 12, 2020
Successfully put the block behind the About me text and table. Not sure what I changed to make it work. 
Next things to fix:
*Make sure website is responsive for different platforms
*Make logo for tab
*Insert video on first page
*There was white space at the bottom of the footer but that was fixed temporarily by changing footer height from 50px to 60px. Figute out better way to fix this.


11:19 AM July 13, 2020
Fixed the profile picture touching the about me section block when in mobile view by adding a <br> element in the html. I think there is a better way to do this by adding padding to a css element but I can't figure out how to get it to work

11:24 AM July 13, 2020
Figured out why the Github and LinkedIn icons at bottom are over white space on mobile view. The columns are stacking on top of eachother rather than side by side.

12:21 PM July 13, 2020
Was able to fix the issue of the columns stacking. Changed the attribute within the bootstrap columns from MD to XS so that they stayed next to each other rather than stacking when contained in a smaller view.*"With bootstrap you want to develop using the smallest device in mind first. This means to use xs on your columns. If you change md to xs your columns should no longer wrap on a smaller device:"* source:https://stackoverflow.com/questions/41943463/prevent-wrapping-stacking-of-columns-in-bootstrap-when-shrinking-the-size


