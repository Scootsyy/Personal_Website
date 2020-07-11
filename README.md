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
