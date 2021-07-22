# Iateria Wiki

The Iateria wiki will let you, the lucky user, explore an intuitive and informative website containing all the information needed to learn all you need to know about Iateria, a fantasy world created for players to engage in using the Dungeons and Dragons 5e ruleset. 

The site will contain useful information about the continent of Iateria, the various people that live there and the countries and factions they have formed. You will also learn about the magic that is abundant throughout the world of Iateria.

The Iateria Wiki will be useful for players about to engage in a role playing adventure set in the world of Iateria, for dungeon masters looking for inspiration for at plot or for experienced players of the world wanting to read up on a concept or place of interest they encounter when exploring the wonderous locations of Iateria.

## Features

### Existing features

- __Navigation bar__

    - Featured on all pages of the site, the navbar will contain 2 parts: A logo and menu to the main pages of the site, and a sub menu that will be specific to each site and subsite

    ![Header with navbar](assets/images/readme-images/header-large.png)


    - This feature will allow for easy navigation to the main parts of the sites.
    - Has a collapsable menu by clicking a "burger" icon on smaller screens.

    ![Header with navbar for smaller screens](assets/images/readme-images/header-small.png)

- __Subsection navigation bar__
    - This feature is a "hamburger" icon used to navigate the subsections of a information page on a smaller screen. On larger screens the menu is placed underneath the heading.

- __Landing Page__

    - This feature will greet the user with an image explaining the purpose of the site, as well as what to expect on it.

    - The main parts of the site will be displayed and given short information. These small infomartion segments will also contain a clickable link. This section will be divided into three parts with images to the left and right, and text in the center.

- __The footer__

    - The footer looks the same on every page of the site. It will contain links to some of the sources referenced on the site, such as Wizards of the Coast (the company behind DnD) as well as where to find many of the rule books mentioned on the site.

    - Social media links to project social media accounts are also included in the footer to direct the user to our social media.

- __The Iateria page__

    - This feature is the first of the main parts of the site and contains information about the continent and its history.

    - Contains the subsections continent, history , underdark and magic, reachable via a subsection menu.

- __The races page__

    - This site will give a short presentation about the different races one might expect to find in on the continent of Iateria. It will provide links to further reading on many of the more prominent races.

    - The site will contain subsections for a number of different races, including humans, dwarves, halflings, elves orcs and more.

- __The factions page__

    - This feature will give a brief rundown on the different nations, factions and alliances that currently exist on the continent. Links to further reading for many of them will be provided.

    - This section will aslo lead to different subsections where additional information on many nations or factions will give the user more knowledge about the world of Iateria.

- __Sign up form__

    This sign up form will allow the user to sign up for a newsletter. At this point there is no database connected to it, so the action is not yet in place. Most of the design for this form was taken from the love running project on the CI course, but adapted to better suite the style of the page in term os coloring and backgrounds. The form has inputs for name and email, both required, as well as a submit button.


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

    The same method used for main menu collapsable for smaller screens was used for subsection menu as well. The code then again had to be adapted to suite the new menu, classes renamed and the css-code changed. This resulted in some testing and bugfixing but the experience of the main menu helped and it was over all a success.

    At the very end of the project, when running the validators I noticed that the subsetion menu were at the wrong side of the screen. It took me a while to find what rule put it on the left side. It was the .sub-menu-burger rule of left:10; that placed it there. Removing that rule put it in the correct place.

- __Landing page__

    After som issues with hero image and finding one that fit both feeling of the page and was large enough, I decided on crumbled pages to give it an "old document" feeling. The covertext proved a bit troublesome, requiring multible adjustments and refeshes using dev tools before the text was aligned according to my wishes and spaced out in the box. The box itself was rather troublesome to place, as I wanted it centered. I found a solution on stack overflow, [here](https://stackoverflow.com/questions/1776915/how-can-i-center-an-absolutely-positioned-element-in-a-div), which helped alot. It is the "Responsive Solution" post that helped. For the main part of the ladning page, a flex box display was used. I followed a tutorial found [here](https://www.w3schools.com/css/css3_flexbox_container.asp#justify-content) on w3s and adapted it to suite my needs. Above the 3 part section there is an information about hte site, simply a paragraph with slightly larger font size and a margin to separate it from the hero image. It took some testing to get the flex box to display the way i wanted, for the "justfity-content: space-between; to work i needed to remove the width of the images. Further testing will continue (written 2021-07-12) to find out if that was the issue.

    When replacing placeholder images with the correct once the entire site bugged out. This was solved by tagetting the images and setting their sizes to inherit from parent element, whose size is controlled by the flexbox display. This rendered teh images to display correctly down to a size of 1200px where responsive design will take over.

- __Footer__

    The footer was given opposite coloring to the heder, with background of dark slate grey and color of old lace. When links are highlighted they are colored in the background highlight for header links. This part proved to be pretty straight forward with minor tweaking of margins to get everything in a comfortable position. There is room for social media links, should the world of Iateria have social media platforms in the future.

- __Iateria page__

    The implementation of this page was rather straight forward, not presenting too many issues. After consulting with my mentor we decided to change the layout, so that it alternates between text on the left and text on the right. The structure will then be the same for all information pages, sharing the same styling. 

    - Images
        Some issues with sizing, but much was solved when adding the fixed size for main content container, as suggested by mentor.

    - Padding was added to h3 and p elements to create a more clearly distinguished heirarchy on the page and to make it more obvious what text is connected to which header.

- __Races page__

    To implement this page I simply copied the Iateria page and changed all the text/image content. This worked like a charm on the first four sections. The fifth section, an additional section compared to the Iateria page, did not work as intended however. For some reason, this entire section falls outside of the container div, even though the html is clearly inside it. I have yet to find a solution to this problem (2021-07-20) EDIT: Issue solved by adding the rule "overflow: auto;" to the container class (2021-07-21)
    When adding images to the races and factions pages, I noticed that I needed to add a max hight to pictures, as some pictures would otherwise take up to much space of they were "narrow" in their size ratio. In order to keep the ratio of the image intact I also added the object-fit: contain; rule to all iamges.

- __Factions page__

    Implementing the factions page was very straight forward, as most of the bugs that appeared previously were sorted, and no additional issues arose when adding the factions page. The only thing left to do was adjust the menues as they have different lengths, resulting in padding and margin issues. This was easily solved by adding additional classes and target those in the style.css.

- __Subestcion menu__

    - This menu was originally placed in the container and part of the main content, but has been moved to the header to make the page layout more intuitive. It has also been given a smaller size than the main menu, both on large and small screens, to clearly indicate that it is a sub-menu.

- __Responsive design__

    Implementing responsive design proved less troublesome than I orgininally feared. I decided on three different stylings for the landing page, one for sizes larger than 1200px, one for between 1200-800px and one for smaller than 800px. For the information pages only two layouts are needed, as the layout for larger and medium size work the same, with only smaller screens needing a different approach. As the layout is devided left to right on both landing page and information pages, the decision to stack content vertically on smaller screens felt like the most natural approach. In that case just removing any flex display or float left/right and instead centering content sorted display in of itself.

    After meeting with mentor I got a lot of suggestions on how to align the content properly using paddings, and on the information pages padding text relating to different sections to make it clearer what belongs the what. I was also notified of some hierarchy issues on the landing page, sorted using some additional headings.


### Validator testing

    The HTML was tested using this [validator](https://validator.w3.org/) with no errors or warnings for any of the .html files

    The CSS was tested using this [validator](https://jigsaw.w3.org/) with 2 errors and 9 warnings. The errors were quickly fixed, they were the simple errors of forgetting the "px" at the end of a size-rule. The 9 warnings are all from the part of the hamburger nav bar menues where I followed a tutorial. I decided to keep that code as is, as the code runs ands the nav bar works. When going through the validator code I also noticed that the subsection menu was placed at the wrong side, see nav bar for more info.

### Unfixed bugs

    **FIXED
    - Issue with screen scrolling on horizontal axis on some of the smaller screens. I have looked at all the page content to try to find which element that is too wide and causes this issue, but have been unable to find it. it is really bugging me out, pardon the pun, and as of yet the problem is eluding me.
    **FIXED
    Solution: Adjust width of container div to be somewhat less wide, removing the issue of elements overflowing. The overflow: auto; is still necessary for all elements to fall into the container on pages with alot of content.

## Deployment

   - The site was deployed to GitHub pages. The steps to deploy are as follows:
    - In the GitHub repository, navigate to the Settings tab and select the "Pages" page
    - From the source section drop-down menu, select the Master Branch
    - Once the master branch has been selected, the page will be automatically refreshed with a detailed ribbon display to indicate the successful deployment.

    The live link can be found here - https://oljung.github.io/portfolio-project-one/

## Credits

    The concept and idea of Iateria is the work of my good friend Joakim Linde, whom I have asked permission to use his ideas and content for the creation of this wiki. 

### Content

    All information on the Iateria, Races and Factions pages are the work of Joakim Linde, written for use in his DnD campains in Swedish and translated by me for this project. All credit for the amazing content goes to him.

### Media

    Images used on this site are from these open source galleries: [pixabay](https://pixabay.com/), [unsplash](https://unsplash.com/) and [istock](https://www.istockphoto.com/en).

