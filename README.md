# OnRecord-Project-Overview
Overview of our work with OnRecord

Live site is available at [onrecord.online](https://onrecord.online/)

Most functionality is behind signup, so below are a few screenshots some the different pages.
*Note: All of these screenshots were taken on a demo version, none of these users are real, and the info on the admin panel does not reflect the status of the production version*
(I'm actively working on this, More will be coming shortly)

### Home Screen
Upon signing up and completing the form, users will be taken to the home screen of the app

![App Home](App_Home.png)

This page shows the graph-based interface that is central to most of the apps functionality. 
The central node always remains fixed, with peripheral nodes floating nearby, spaced around the central node according to the nubmer of nodes. 
This interface was entirely custom, and was implemented largely using Framer Motion, which allowed us to create entrance/exit animations and subtle
floating animations that make the interface seem natural and welcoming. 

the icons at the bottom are your skills, and the button at the bottom allows you to put yourself into the pool of musicians awaiting a match. When you 
put yourself in the matching pool, one 'seshpoint' is subtracted (indicated top center of the navbar) and the button will change to indicate that a 
match will come soon. Once in the pool, they will be included next time the algorithm runs, and they will show up in the unmatched pool in the admin panel 
to be included in a manually created band.

The peripheral nodes on this page represent bands that you have been matched into. Clicking on it will take the user to that band's page.

### Band Page

![Band Page](Band_Page.png)

The band page is where you communicate and share files with your bandmates. Clicking on the band node opens up a modal which allows you to change the name of the band, edit the band's colors (name and colors randomly assigned on creation), leave the band, or report users for misconduct.

Hovering over a member node will show when they were last on the site. Clicking on a member node opens a modal with their basic profile info (skills, genres of interest, bio, social meida)

In the bottom right, there is a chat window, which allows them to communicate with their bandmates, share file, and submit their completed project to the next competition.

![Band Chat](Band_Page_w_Chat.png)


### Profile Page
From the **Home screen**, you can click on the 
