# Ski Cross Club

![Responsive screenshot](/assets/images/ski-cross-club-responsive-overview.jpg)

# Site aim

This website was created as a fictional club of Ski Cross enthusiasts and/or people who wanted to discover the sport especially after the Winter Olympics. The scope in terms of audience ranges from those who are completely new to the sport to those who want to find a community of other people interested in the sport where they can share their passion.

The site has 4 pages in total built using HTML and CSS.

This is the first of 5 projects as part of the Diploma in Software Development from Codeinstitute and was part inspired by the project done previously with guidance called "Love Running".

A link to the live website can be found here:

https://alyt89.github.io/Milestone-Project-One/events.html



# User goals

The website is expected to attract users who:

- Are looking to discover a new sport having seen the winter olympics

- Have been skiing and want to find a community based environment

- Struggling to find a way to get into the sport of Ski Cross




The website will allow users to:

- Find out information about the sport

- Find out information about the club including its aim

- Discover events nearby and register their interest in these events

- Contact the club for any questions


## Requirements

This project required creating a static website and documenting its progress through GitHub containing key functionalities and features such as a nav bar, links and images/video.

## Color scheme

The color scheme for the website was relatively simple using 2 main colours throughout, these were whitesmoke (rgb(245,245,245) and slightly lighter shade of black (rgb(7, 1, 20)) in varying degrees of opacity to contrast and fir in with the skiing/snow theme.


## Fonts

The fonts used were taken from Google Fonts and applied throughout the project.

The font used for headings was Josefin Sans and for other blocks of text was Josefin Slab. This combination was suggested on the following forum/website: https://www.freshwateragency.com/4-great-google-font-pairings/

# Site features

## Header and Navigation

![Responsive screenshot](/assets/images/ski-cross-club-header-section.jpg)

The header contains the site's name (Ski Cross Club) in the largest font to clearly indicate to site visitors the name of the site and is maintained across the 4 pages of the site for consistency. 

The navigation bar section allows customers to navigate to the other pages on the site, the current page the user is on is shown by the underline styling.

The hero image for the  page begins at the top of each page and sits behind the header/navigation bar and continues below showing a person skiing in the background.

The hero image has an overlay applied with an absolute positioning to allow the white text to contrast more pleasingly for better user experience.

There is an animation applied to the tagline for the website "Join the club discover ski cross" to draw the user's attention each time the page loads. The code required to animate this section has been duly credited in the CSS file.

On the Events, Gallery and Sign Up pages there is no animation applied but the page summary is positioned and sized the same way with a small description underneath.


## Aim and history section

![Responsive screenshot](/assets/images/ski-cross-club-aim-history-section.jpg)

This section is intended to give the user an idea of what to expect from Ski Cross Club and its current stature. The section reconfirms that it is intended for various levels of ability and age.

The history is important to allow the user to know what to expect from the club as it is quite new and growing.

The section maintains the same colour scheme and has a background image of a skier with their ski's in a cross formation.



## What is Ski Cross section

![Responsive screenshot](/assets/images/ski-cross-club-what-is-ski-cross-section.jpg)

This section is inteded to give those with less of a knowledge of winter sports and in particular skiing what the sport is and what it involves. The section aims not only to inform but encourage users to discover more and get involved.


## Visual navigation links

![Responsive screenshot](/assets/images/visual-navigation-links.jpg)

This section is inteded to reinforce the nav bar at the top of the page as this is not fixed so users would have to scroll up to find this otherwise.The images provide a further visual clue to what the page they are clicking on will contain. Each image has an effect when hovered over to come into focus before the user clicks.


## Footer

![Responsive screenshot](/assets/images/ski-cross-club-footer.jpg)

The footer is consistent across the 4 pages of the website and contains links to the 3 social media platforms to find out more information on the relevant platforms.

The links have been coloured suitably as per the company's logo and animate on hover to show the user they are about to select the link.

## Events page

![Responsive screenshot](/assets/images/ski-cross-club-aim-events.jpg)

The events page contains 6 upcoming events to give users information about where, when and what the club is planning for the remainder of the year.

The events are set out in a grid layout for consistent display.

The events details section below it provides additional basic information that is applicable to all events the user would want to know before registering their interest in one of the events via the sign up form. This includes the equipment that is provided and information on how to register their interest.

## Sign up form

![Responsive screenshot](/assets/images/ski-cross-club-aim-form.jpg)

The form is intended to collect the basic information from the user where they can specify which events they are interested in.

There is a minimal amount of information required to enter to encourage the user to send their details and hear back from the club so they can start to get involved.

Once submitted the form redirects the user to a page to confirm the information has been captured successfully and will receive and email in due course.

## Contact information

The club's email address for any other questions is provided in another section below the form consistent with the styling on previous pages.


# Testing

## HTML validator

The HTML on all pages was validated by testing through https://validator.w3.org/#validate_by_input with no errors found as shown below:

![Responsive screenshot](/assets/images/ski-cross-html-validator-testing.jpg)

## CSS validator

CSS validation was done via Jigsaw validator on the following link with no errors found: https://jigsaw.w3.org/css-validator/#validate_by_input

![Responsive screenshot](/assets/images/ski-cross-club-css-validator-testing.jpg)

## Lighthouse

Testing was done via Lighthouse and scored as below on Desktop and Mobile:

### Desktop:

![Responsive screenshot](/assets/images/ski-cross-club-lighthouse-desktop.jpg)


### Mobile:

![Responsive screenshot](/assets/images/ski-cross-club-lighthouse-mobile.jpg)


The site has been tested on Google Chrome, FireFox and Microsoft Edge. It has also been tested on a mobile device to check the responsiveness.

Throughout the development of the site I have used Google DevTools to ensure that the responsiveness is working and any bugs encountered are identified during development.

There have been regular commits to github with clear remarks on each update to easily track progress of the project.

All links both internal and external have been tested and any external links open in a new tab to maintain good user experience.

The site has also been tested by an impartial user to test for intuitiveness, ease of use and layout/visibility issues. One issue raised from this was the text contrast on one of the visual links and this was subsequently resolved by increasing opacity/constrast.

## Main issues discovered and resolved

1. Section overlay not matching image height

- I wanted to darken the background images on the sections to allow the text to stand out clearly however by using absolute height values for the sections when the padding and margins were added the overlay would not match up. This was identified and adjusted so the sections did not overlap.

2. Text overflowing section

- Again due to the absolute px values given to sections some of the text overflowed the section when the screen size was reduced. Line height and font size were adjusted in the media queries to correct this.

3. Conflicting CSS selectors

- Through development I noticed that using the DevTools some of my styling were not being applied as being overriden by another class or id alreay updated in my CSS file which was of higher specificity. This was corrected by identifying any unnecessary or duplicated class/id and increasing specificity where needed.

4. Error on redirect page for signup form

- On submission of form I wanted the user to be redirected to a page confirming details were submitted correctly however this returned an error. On inspection through Slack forums I discovered that the method should remain as "GET" instead of "POST".

5. Images for Visual Navigation Links not working when site deployed

- I noticed the images on the index.html page providing links to the other pages were not displaying, when these were adjusted to relative file paths instead of absolute file paths the problem was resolved.



# Deployment

This project was hosted and deployed on GitHub, steps taken to deploy are as follows:

- Open relevant GitHub repository and navigate to 'Settings' tab.

- Navigate to 'Pages' option located in the 'Code and Automation' section 

- Under 'Source' heading select the main branch and 'root' folder, once done click 'save'

- Refresh page until the active URL is provided


# Future site enhancements

In time the site could have additional pages incorporated such as a member's directory and a forum to discuss topics and offer Ski Cross related equipment second hand.

# Credits

Through the development of this site I have used various resources to help me especially when applying the Grid and Flexbox principles, the guidance on https://css-tricks.com/snippets/css/a-guide-to-flexbox/ and https://css-tricks.com/snippets/css/complete-guide-grid/#prop-grid-template were particularly helpful for this.

In addition I have used the W3Schools website to assist with general HTML and CSS queries such as Z-index and position.

Specific credits are noted in the CSS file for animations on the home and gallery pages.

## Images

Images were sourced from a combination of https://unsplash.com/ and Google Images. As Ski Cross is quite a unique sport there were limited images for specific elements of Ski Cross that were required for the gallery page and therefore Google Images was required.

