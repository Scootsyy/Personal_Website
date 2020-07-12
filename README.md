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
*Does font in about me section hard to read?
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
