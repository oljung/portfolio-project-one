# Iateria Wiki

The Iateria wiki will let you, the lucky user, explore an intuitive and informative website containing all the information needed to learn all you need to know about Iateria, a fantasy world created for players to engage in using the Dungeons and Dragons 5e ruleset. 

The site will contain useful information about the continent of Iateria, the various people that live there and the countries and factions they have formed. You will also learn about the magic that is abundant throughout the world of Iateria.

The Iateria Wiki will be useful for players about to engage in a role playing adventure set in the world of Iateria, for dungeon masters looking for inspiration for at plot or for experienced players of the world wanting to read up on a concept or place of interest they encounter when exploring the wonderous locations of Iateria.

## Features

This wiki consists of a landing page, with basic information about what Iateria is, and what the user can explore further in the site.

### Existing features

As the project moves along development, completed features will be listed here.

- __Navigation bar__

    - Featured on all pages of the site, the navbar will contain 2 parts: A logo and menu to the main pages of the site, and a sub menu that will be specific to each site and subsite
    - This feature will allow for easy navigation to the main parts of the sites.
    - Has a collapsable menu by clicking a "burger" icon on smaller screens.

- __Landing Page__

    - This feature will greet the user with an image explaining the purpose of the site, as well as what to expect on it.

    - The main parts of the site will be displayed and given short information. These small infomartion segments will also contain a clickable link. This section will be divided into three parts with images to the left and right, and text in the center.

- __The footer__

    - The footer looks the same on every page of the site. It will contain links to some of the sources referenced on the site, such as Wizards of the Coast (the company behind DnD) as well as where to find many of the rule books mentioned on the site.

### Features left to implement (near future)

Here a list of all features to be implemented

- __Subsection navigation bar__
    - This feature will be a "hamburger" icon used to navigate the subsections of a information page.

### Information pages

These pages will all follow the same format and structure, making information easy to find and making them feel intuitive. The page about dwarves will be stuctured the same as the page for orcs, for instance.

- __The continent page__

    - This feature is the first of the main parts of the site and contains information about the continent and its history.

    - Will contain the subsections (may be made into separate pages if they become to long and to densly packed with information) geography, history and magic.

- __The races page__

    - This site will give a short presentation about the different races one might expect to find in on the continent of Iateria. It will provide links to further reading on many of the more prominent races.

    - The site will contain subsections for a number of different races, including humans, dwarves, halflings, elves orcs and more.

- __The countries and factions page__

    - This feature will give a brief rundown on the different nations, factions and alliances that currently exist on the continent. Links to further reading for many of them will be provided.

    - This section will aslo lead to different subsections where additional information on many nations or factions will give the user more knowledge about the world of Iateria.

- __The footer__

    - Social media links to project social media accounts

### Features left to implement (distant future)

- __Search function__

    - This feature will allow the user to enter a keyword in a textpox and if it is on the site, the user will be provided with links to the page where it can be found.

    - This feature requires tech outside of the scope for this project

- __Performance tracker__

    - This section will allow a player participating in a game on the continent to view their performance so far by reading information about roll averages, damage done and healing provided.

    - This feature requires tech outside of the scope for this project

## Testing

- __nav bar__

    The navbar was positioned correctly from the first test, however it became clear that more space was needed between each link. The styling went as intended, with the default styling removed and color and font of the site applied. The active page was given a background color and different text color, and after testing I decided to add some padding to the active class, making the background color cover some area around the text as well. The same style was then applied to the hover pseudo class, which also had its font increased in size to make the link "pop out" when hovered over.

    The entire header is fixed in position. This proved problematic at first, as it would not display apart from on different places of the site. the solution, apart from placing it in the correct position and fixing position, was to adjust z-index to 1. placing it in front of all other elements.

    When adapting the nav bar to smaller screens, I followed a tutorial by [Mark Caron](https://medium.com/@heyoka/responsive-pure-css-off-canvas-hamburger-menu-aebc8d11d793) to create a collapsable menu using only css elements. This code was then adapted to fit the sites layout and coloring. This led to significant testing to find out what part of the css changed what part of the menu. After some toubleshooting, quite a bit of bugfixing due to spelling mistakes, I was able to adapt the menu to fit my intentions. All in all this testing process took about 45 minutes, which compared to other parts of the testing and bugfixing is rather significant.

- __Landing page__

    After som issues with hero image and finding one that fit both feeling of the page and was large enough, I decided on crumbled pages to give it an "old document" feeling. The covertext proved a bit troublesome, requiring multible adjustments and refeshes using dev tools before the text was aligned according to my wishes and spaced out in the box. The box itself was rather troublesome to place, as I wanted it centered. I found a solution on stack overflow, [here](https://stackoverflow.com/questions/1776915/how-can-i-center-an-absolutely-positioned-element-in-a-div), which helped alot. It is the "Responsive Solution" post that helped. For the main part of the ladning page, a flex box display was used. I followed a tutorial found [here](https://www.w3schools.com/css/css3_flexbox_container.asp#justify-content) on w3s and adapted it to suite my needs. Above the 3 part section there is an information about hte site, simply a paragraph with slightly larger font size and a margin to separate it from the hero image. It took some testing to get the flex box to display the way i wanted, for the "justfity-content: space-between; to work i needed to remove the width of the images. Further testing will continue (written 2021-07-12) to find out if that was the issue.

    When replacing placeholder images with the correct once the entire site bugged out. This was solved by tagetting the images and setting their sizes to inherit from parent element, whose size is controlled by the flexbox display. This rendered teh images to display correctly down to a size of 1200px where responsive design will take over.

- __Footer__

    The footer was given opposite coloring to the heder, with background of dark slate grey and color of old lace. When links are highlighted they are colored in the background highlight for header links. This part proved to be pretty straight forward with minor tweaking of margins to get everything in a comfortable position. There is room for social media links, should the world of Iateria have social media platforms in the future.



### Validator testing

### Unfixed bugs

## Deployment

## Credits

### Content

### Media


