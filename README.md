<h1>Metallica - The best in the business (a.k.a Milestone 1 Project - Kieran Cunnane)</h1>
<p>This site/project has been created to showcase effectively the catalogue of music provided by Metallica.

The site is a simple, easy to navigate site, designed specifically to cherry pick the best examples of the band without overloading the user with content.
</p>

<h2>UX</h2>
I wanted to make this site as simple to use as possible, which I why I chose the single page parallax design. Mainly the objective of this is to show off the important point of the band in a simple, easy to use, one page solution. The page shows music, which is the main focus for the band, then the stage presence, finally finishing off with an about section should the user be interested in the bands history. 

<h2>Features</h2>

* Pallax Effect
* Opacity Shift Logo
* Scroling Encouragement (avoiding false bottom to page)
* iFrame Embedding
* Data Validation
* Smooth Scrolling
* Hidden Music (404 page)


The main feature of this site, which the site revolves around is the [parallax effect](https://www.w3schools.com/howto/howto_css_parallax.asp). This was decided before the project started, but was only implimented halfway through the working build process. It feels like the best way to showcase the band abilities, without bouncing users to multiple pages, and keeps everything in one easy to use page.

The main logo at the start of the page changes color when hovered, as the static white image just seemed a little boring alone. To enable to color shift in the main logo, I have currently employed two images overlayed, and when hovered, shifts one of the logos to become visible.

I have also allowed part of the next section to be visible in the desktop site, to encourage the user to start scrolling as there is more content below.

I've also implimented several embedded youtube and soundcloud links to showcase the band back catalogue. These are customised to the best of my ability by altering the links which isn't a default feature of the iframe taken form the sites.

The form at the bottom of the page, while it does have data validation, doesn't work entirely the way as intended due to the limitations of CSS and HTML, but this is outlined in the "Features left to Impliment" section below. Currently this addition feature is implimented with 

Smooth scrolling is also a big feature for this site, as it works in conjunction with the anchor tags placed at the start of each section (with offsets to allow for the static navbar), and allows for a smooth transition into each section. 

The main navbar is a great feature because it moves you to each section on the page, without the need for reloading the page, and with smooth scrolling, means the user can fast scroll through the webpage with ease.

The contact form is designed with a pyramid symmetry in mind, as when the boxes are extended to the size of the query box, they just seem too long for the page. So the contact form now has relevant width, without the boxes being too wide. This was also decided to match the rest of the page content, as most of the content on desktop is 10 columns wide with an offset of 1, and initially the contact form was 6 columns wide with an offset of 3, meaning it felt out of place in the flow of the page.

As an added bonus, there is a 404 page, with custom GIF background, and a musical background. On this page, I've implimented a pulsing sound button to encourage users to click and fire the Soundcloud link hidden off screen.

---

<h3>Features Left to Implement</h3>

1. A feature left to impliment is a javascript to enable to the [form to complete without a reload of the page](https://www.w3schools.com/jsref/met_loc_reload.asp), possibly with a thank you message and redirect to the social links. I've explored this via the [Bootstrap Toast](https://getbootstrap.com/docs/4.3/components/toasts/) message, but due to the limitations of HTML and CSS, and my lack of knowledge in Javascript, this will be left as a feature to impliment once I have learned more about Javascript. This space is currently filled with an onsubmit dialogue box, with reload of the page.

2. I also plan to impliment a time delayed hidden navbar. When the user pulls the screen on mobile, the navbar will appear, but when inactivity on the screen meets a certain time criteria, the navbar will disappear off screen until activity is detected again.

3. I would also like to change the 404 sound button in the future to allow the Soundcloud link to fire without a page reload.

4. A final feature to possibly impliment is the [Bootstrap Scrollspy](https://getbootstrap.com/docs/4.3/components/scrollspy/) to work in conjunction with the current nav bar, unfortunately the design of the navbar wouldn't work as expected, and would require a complete rework of the nav element. This will need to be revisited at a later time as it requires a little bit of Javascript to be able to impliment this plan effectively.

<h2>Technologies Used</h2>

* [HTML](https://www.w3schools.com/html/html_intro.asp)
* [CSS](https://www.w3schools.com/css/)
* [Bootstrap](https://getbootstrap.com/)
* [SoundCloud Embedding](http://www.soundcloud.com)
* [Youtube Embedding](http://www.youtube.com) 
* [Google Fonts](https://getbootstrap.com/)
* [Font Awesome](https://getbootstrap.com/)

The current framework used in this site is [Bootstrap](https://getbootstrap.com/), and is solely built using HTML, CSS, and [Bootstrap](https://getbootstrap.com/) framework.

[Soundcloud](http://www.soundcloud.com) and [Youtube](http://www.youtube.com) were used for iframe embedding, with slight alterations to the iframe embedding code. These were used to showcase both the musical catalogue, and the stage presence of the band.

In this section, you should mention all of the languages, frameworks, libraries, and any other tools that you have used to construct this project. For each, provide its name, a link to its official site and a short sentence of why it was used.

<h2>Testing</h2>
This site has been tested both on Chrome and IE11. 

Unfortunately not all of the features work fully on IE11. Currently the smooth scrolling option is not fully functioning on IE, and will require movement possibly to JavaScript instead of the inbuilt smooth scroll feature.

I am currently aware that the main logo does not align correctly, but after much investigation, I am unable to correct this as of yet without affecting the layout on Chrome. Also the parallax effect which the site is built around does not work on IE11, and currently only stutters the images when scrolling, instead of holding the images static.

Testing via Chrome went more smoothly. Mainly to point, when running an audit using the inbuilt developer tools, scored 100 across the board once deployment was completed as shown below.

![Audit Results](https://github.com/Legaeldan/milestone-1/blob/master/assets/images/audit-results.PNG "Audit Results")

During testing, due to limitations of browsers, the 404 page does not allow the Soundcloud links to fire on load, and I've had to impliment a reload button, as the media will fire on a reload as opposed to a redirect from another page. Unfortunately I was unable to change the z-index effectively, and resorted to moving the image far enough off screen that it will not be seen despite screen width, and set the page overflow to hidden so that the user cannot scroll to it, or even know it is there.

During mobile testing, several issues arose, mainly pertaining to the nav bar. The way the nav items are set up, unfortunately I was unable to scale them correctly, so the code is now corrected to remove the 3rd, 4th and 6th borders on scaling, and add them correctly back after scaling back to desktop.

I have also tested the functionality of the main logo on mobile, and while it changes on mobile, it only changes when the user clicks and holds the item. I will be looking further into correcting this with Javascript to show the item when it is on screen, as opposed to held.

All code is checked via a [HTML Validator](https://validator.w3.org/) and [CSS Validator](https://jigsaw.w3.org/css-validator/validator), and I'm currently aware of an warning in the HTML, but as it's only a warning, I have decided that it's an acceptable warning due to the layout of the page.

<h2>Deployment</h2>

This project was developed using the [Cloud9 IDE](https://c9.io) initially before moving locally to [Visual Studio Code](https://code.visualstudio.com/) and [Git](https://git-scm.com/downloads), committed to a local [Git](https://git-scm.com/downloads) repository, and pushed to [GitHub](https://github.com/Legaeldan/milestone-1) using a locally installed version of [Git](https://git-scm.com/downloads) via command prompt.

The main method of deployment, [GitHub Pages](https://legaeldan.github.io/milestone-1/index.html), was chosen after a discussions with my mentor, and I was notified of GitHub pages, meaning I didn't need to boot up Cloud9 everytime I wished to showcase my site.

All deployment to [GitHub](https://github.com/Legaeldan/milestone-1) have been done using [Visual Studio Code](https://code.visualstudio.com/), with [Git](https://git-scm.com/downloads) installed locally to push to the repository.

There are currently two branches posted to [GitHub](https://github.com/Legaeldan/milestone-1/branches). 
* The master which incorporates all commits from the start of the project. And includes the parallax branch merge from the middle of the project.
* The parallax branch, which was the point of change from a multi page site, to a single scrolling site.

The project is essential one large branch, but has been split to allow back tracking should parallax not work out, and I'd need to revert back to the multi page layout.



<h2>Credits</h2>

Backgrounds and images all found via Google Images with the exception of the whiskey background linked below. Unfortunately I did not take note of each site linked in Google Images.

[Whiskey Background](https://blackenedwhiskey.com/wp-content/uploads/2018/11/Blackened_Story_Hero_New.png?id=1631)

Exceptions to this include the contact for background, and the about us background, which are custom created from other images.

About us section is a copy from [Wikipedia](https://en.wikipedia.org/wiki/Metallica)

All music links are from [Soundcloud](http://www.soundcloud.com) and all videos are linked from [Youtube](http://www.youtube.com).

<h3>Acknowledgements</h3>

I received inspiration and assistance on this project from Simen Daehlin (Eventyret), who assisted above and beyond to help improve the site, especially to the point that I definately intend to return to this site once I have Javascript under my belt. He's certainly helped show me what features will be available to me later on down the line.
