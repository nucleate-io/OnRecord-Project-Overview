# OnRecord-Project-Overview
Overview of our work with OnRecord

Live site is available at [onrecord.online](https://onrecord.online/)

Most functionality is behind signup, so below are a few screenshots of the different pages.

*Note: All of these screenshots were taken on a demo version, none of these users are real, and the info on the admin panel does not reflect the status of the production version*
(I'm actively working on this, More will be coming shortly)

# The Interface

### Home Screen
Upon signing up and completing the form, users will be taken to the home screen of the app

![App Home](App_Home.png)

This page shows the graph-based interface that is central to most of the functionality of the app. 
The central node always remains fixed, with peripheral nodes floating nearby, spaced around the central node according to the number of nodes. 
This interface was entirely custom and was implemented largely using Framer Motion, which allowed us to create entrance/exit animations and subtle
floating animations that make the interface seem natural and welcoming. 

The icons at the bottom are your skills, and the button at the bottom allows you to put yourself into the pool of musicians awaiting a match. When you 
put yourself in the matching pool, one 'seshpoint' is subtracted (indicated top center of the navbar) and the button will change to indicate that a 
match will come soon. Once in the pool, they will be included next time the algorithm runs, and they will show up in the unmatched pool in the admin panel 
to be included in a manually created band.

The peripheral nodes on this page represent bands that you have been matched into. Clicking on it will take the user to that band's page.

### Band Page

![Band Page](Band_Page.png)

The **Band Page** is where you communicate and share files with your bandmates. Clicking on the band node opens up a modal that allows you to change the name of the band, edit the band's colors (name and colors randomly assigned on creation), leave the band, or report users for misconduct.

Hovering over a member node will show when they were last on the site. Clicking on a member node opens a modal with their basic profile info (skills, genres of interest, bio, social media)

In the bottom right, there is a chat window, which allows them to communicate with their bandmates, share file, and submit their completed project to the next competition.

![Band Chat](Band_Page_w_Chat.png)


### Profile Main Page
From the **Home Screen**, you can click on the profile node (central) to get to the profile edit page.

![Profile Page](Edit_Profile.png)

From here you can update your profile picture and get to your bio edit page and social media page

#### Profile Edit Page
![Profile Page](Bio_Page.png)

Here you can give yourself a bio that your bandmates can see, and you can toggle email notifications.


### Social Media Page
![Social Media Page](Social_Media.png)

Here, you can add links to your social media pages. Accepted platforms are Facebook, YouTube, SoundCloud, & Spotify. Clicking on 'Connect' in the empty node or 'Update' in one of the existing nodes opens up a modal.

![Social Media Modal](Social_Media_Modal.png)
Here you can paste your profile link to any of the supported platforms, and the modal detects the platform, highlights it, and allows you to add it. If it doesn't match any of the supported platforms, it's not allowed. This is just one of many modals on the site, as much of the site's interaction is through dialogs like this one, such as file sharing, competition submission, band feedback, and a lot more.



## Competitions
![Competitions Home](Competitions_Home.png)

Through the sidebar menu, you could access the competitions page, where users can see details about the upcoming competition. Just below, they will see any projects they have that have been submitted to a competition

#### User Submissions
![User Submissions](Competition_Song_Submissions.png)

Songs that have been submitted and are awaiting the submission deadline display with a countdown timer indicating when they can come back to vote. Submissions that have been submitted to a competition that is open for voting will dispay a "vote now" button


### Voting Page
![Voting Page](Voting_Page.png)

Voting is done by ranked choice, and uses this custom list of drag-and-drop players. Competitions are split up into voting groups based the number of submissions made to the competition, and each voting group has between 4 & 9 songs to vote on. Users must listen to at least a minute of each song before submitting their vote. The interface also allows users to give feedback on each song, which the members of each group can view once the competition is over. 

If there were multiple voting groups (more than 9 submissions made to the competition), then the competition will have mulitple rounds, taking the top 3 from each voting group into the next round, doing so until there is only one voting group left. The top 3 songs in the final round will be the winners of the competition.



