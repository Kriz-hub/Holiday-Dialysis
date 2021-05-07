# Holiday Dialysis
Code Institute - Milestone Project 1

This project is a one page website about a Dialysis Center in the middle of The Netherlands. They offer a dialysis treatment for people who suffer from kidney failure and are open for guests who are on holiday. This is a made up center in the small city of Harderwijk, but actually I work in a real dialysis center in that place.It is also a satelite center of the big one in Amersfoort, 30km from Harderwijk. Important: this project is meant for the post-corona era, off course the situation will become better the comming months and certainly in 2022.


![Desktop Demo](https://github.com/Kriz-hub/Holiday-Dialysis/blob/master/Animatie.gif)

## UX
From a financial point of view it is very interesting for a hospital to add guests to their patient population. A descent website helps to get a good representation.
I know there is a real demand for a good website for the real dialysis center I work in, first one for holiday guests, later for the dialysys center as a whole.
To prevent that the Milestone 1 project will become too big, I am focussed on the part of Holiday Dialysis.

Business goals:
To get guests interested for there center, there are more to choose in a radius of 50 km. It's a tourist area, that also means they can atract the foreign guest.
The website must not be for a too young audience, the population which is interesting for a dialysis center is mainly 40 years and older.
The next goal for a center to have a descent website is simply to create goodwill, be representive.

Customer goals:
The kidney patient needs 3 times a week dialysis in his own center, but also wants to have an opportunity to get on holiday.
He needs to be informed which center he can choose and what they can offer him. So the website must be informing but not too corporate. He is in the mood for holiday and that mood should reflect the website. 

**Research**

I googled for dutch sites of dialysis centers to get the right feel and if I can learn from it. The websites appears to be not always that great:
* https://www.meandermc.nl/patientenportaal/patienten/afdelingen-specialismen/Dialyse-Centrum/Dialyse/Vakantiedialyse/
* https://www.dianet.nl/holiday-dialysis
* https://www.dcg.nl/behandeling-en-ondersteuning/vakantiedialyse?utm_campaign=Adwords+Vakantie
* http://www.dialysecentrumbeverwijk.nl/op-vakantie
* https://www.dialysecentrumravenstein.nl/

The first one is the center where I actually work. I certainly won't get a holiday feeling when I watch this as a potential guest for dialysis! (sorry)
The second one is too corparate, there isn't much happening.
The third is better but the red menu kills the view of the picture. It should have more pictures and movement.
The fourth isn't bad, but the sea view looks dead with an image wich almost lost his color, They could do better with a carousel view in my opnion.
The last one is very good.

But the real inspiration came when I saw this bike site: https://biketourharderwijk.nl/ (not even a dialysis site)
The pictures of the carousel blowed me away, I decided from that moment my front page of the project must be a carousel in a rectangle format.

## The start
On start I thought to make a website based on one big background picture of the rural area with a big title and subtitle, all to create that holiday dialyse feeling.
With scrolling the information moves over te background picture. The technique was inspired from this idea: https://valentina-b.github.io/par-excellance-restaurant/. 
Than other pictures of specific dialyse treatment should appear in a carousel after some scrolling.
In that first stage the mentor advised to use smaller pictures and add more text, because the purpose of the website (atract guests who wants to book dialyse treatments) wasn't clear enough. Also he advised to use a Google Map image for a better understanding where the center is situated.

Then after research I knew that I wanted a rectangular carousel with a fading effect in it, with a text column on the left with a little bit tourist information of the area "The Veluwe" and with a text that guests are welcome to come. The right column is the intro part for the center.
The About section gives more information about he center. De contact page gives information to get into contact.

## Structure
###Section1
* The homepage features a responsive navigationbar on the right and a logo on the left top, this bar is fixed. On mobile screens left en right side will split en become centered   in top of each order.
  The navigationbar has also a language button. With javascript and display=none and display=inline, the right language appear in front without loading the whole page.
* Below that is a fading carousel as the hero image. I didn't want to add control buttons to swap the images by hand, just images with a fading effect to each, for designing purposes as the reason.
  In that fading carousel a title "Holiday Dialysis" appears with a linear-gradient background directly beneath that text.
  In smaller devices the title becomes too big according to the pictures of the carousel, therefore the title emerges down the pictures in mobiles.
* Below are 2 columns of text. They appear down each other on a mobile device.

###Section2
* In section 2 a second, normal, carousel appears with some dialyse pictures. It is attached to the text column underneath. On the right there is a picture of the fantasy dialyse center, also attached to the unordered list underneath. 
* On mobile devices it wil appear below each other.

###Section3
* In desktop-devices section 3 appears as 3 column area. On the left side there's Google Map Iframe, the middle a form, and to the right a picture with adress.
* On tablet devices it breaks into a googlemap area with underneath a form and picture with adress on the left and right side. It is made possible by using a nested bootstrap Col element.
* On a mobile device everything appears below each other.

### Shadow, hover and transition effect after hover
To give this webpage a finishing feel, I have put a shadow effect on the images, carousels and google map. Then I added a transition effect after hovering as well, but only for laptop en desktop devices because it appears not really to be that cool for a small device. I discovered that the hovering of the fading carousel didn't work. The reason must have been it's relative position, because of the title "Holiday Dialysis" absolute position in it. I saw it wasn't really necessary for the title's position, so I removed the "relative position line". The title kept on the same place because the body itself is also relative. Also all titles have also some transition on it. For alle devices icons and navigation have a hovering effect. 
To get it really finished I brought an increase of shadow in after hovering. I saw an interesting youtube to do it on a way to keep the rendering significant lower, good for older devices, see Acknowledgements. The trick is animate opacity instead of animating shadow size.

###footer
* On the left 2 icons appear with Facebook and Twitter, on the right a copyright mark appears. Facebook and Twitter is enough for this site. Hospitals aren't that much into social media.

###Skeleton
The wireframe was made in Balsamiq. At first i Hadn't an idea of responsive design, I only thought how to get it right on my lap top. Therefore I couldn't make wireframes for tablet or smartphone. This were the early wireframes: 
https://github.com/Kriz-hub/Holiday-Dialysis/blob/master/OldWireframes/Wireframe%201.png
https://github.com/Kriz-hub/Holiday-Dialysis/blob/master/OldWireframes/Wireframe%202.png
https://github.com/Kriz-hub/Holiday-Dialysis/blob/master/OldWireframes/Wireframe%203.png

Later it evolved to a greater and responsive idea :
* laptop/desktop:
  Section1: https://github.com/Kriz-hub/Holiday-Dialysis/blob/master/NewWireframes/section%201%2C%20home.jpg
  Section2: https://github.com/Kriz-hub/Holiday-Dialysis/blob/master/NewWireframes/section%202%2C%20about.jpg
  Section3: https://github.com/Kriz-hub/Holiday-Dialysis/blob/master/NewWireframes/section%203%2C%20contact.jpg
* Tablet: The tablet views the same in panorama view.
          when it is on "selfie view" section3 is ordered on a slightly different way with google maps on top:
          https://github.com/Kriz-hub/Holiday-Dialysis/blob/master/NewWireframes/tablet%20section%203%2C%20dif%20layout%20as%20desktop.jpg
* Smartphone:
  All is showing below each other, Top bar is split in 2 parts:
  https://github.com/Kriz-hub/Holiday-Dialysis/blob/master/NewWireframes/smartphone%2C%20a%20%26%20b.jpg
  https://github.com/Kriz-hub/Holiday-Dialysis/blob/master/NewWireframes/smartphone%2C%20c%20%26%20d.jpg
  https://github.com/Kriz-hub/Holiday-Dialysis/blob/master/NewWireframes/smartphone%2C%20e%20%26%20f.jpg

##Technologies
1. HTML
2. CSS
3. Bootstrap version 4.0.0
4. Javascript

##Features
There is some Javascript added for using GetelementbyID to use display=none and display=inline to hide language when is is not chosen.

##Features left to implement
The behaviour of the scroll-spy is somewhat pour, I was forced to add some empty text to get it right on the pages. With a little bit more knowlegde of Javascript I could make a custom scroll-spy myself. I think I would use "100vh", because that's alway the screensize vertically. Then use a way to get the current screenposition relatively to "100vh", then give a command to make some lines of scrolling.

##Testing


## Deployment
This site is hosted using GitHub pages, deployed directly from the master branch. The deployed site will update automatically upon new commits to the master branch. In order for the site to deploy correctly on GitHub pages, the landing page must be named `index.html`.

To run locally, you can clone this repository directly into the editor of your choice by pasting `git clone https://github.com/` into your terminal. To cut ties with this GitHub repository, type `git remote rm origin` into the terminal.


## Credits

### Content
All content in the 

### Media
Some were taken from [Pexels](https://www.pexels.com/), a stock image library, with the exception of the photo of myself in the background of the 'about me/À Propos' section in the desktop view. A greyscale filter was applied to each one prior to upload to preserve the greyscale theme. 

### Acknowledgements

To get af flag image into a button and customizing it: https://stackoverflow.com/questions/49184471/how-to-change-bootstrap-version-4-button-color 
Creating a feading carousel on section1:  https://silvawebdesigns.com/how-to-change-the-bootstrap-4-carousel-to-a-fade-transition-instead-of-slide/
To get a normal carousel on section2:  https://getbootstrap.com/docs/4.0/components/carousel/ 

To get a responsive google maps thanks to: https://blog.duda.co/responsive-google-maps-for-your-website 
Form, thanks to bootstrap: https://getbootstrap.com/docs/4.1/components/forms/

Inspiration to get a multi language page working:
https://stackoverflow.com/questions/46008760/how-to-build-multiple-language-website-using-pure-html-js-jquery
I read about "display:none". That reminded me to my own litle project "5 days of coding challenge", where I used it to hide pictures. Now I used that idea to make a multi
language site without the need to load the whole website again when changing language. (And to prevent coding from repeating because the other way is make 2 different pages.)

Shadow on Carousel and images:  https://www.w3schools.com/css/css3_shadows_box.asp*/

Youtube of Kevin Powel: https://www.youtube.com/watch?v=u6Rur7G8HNY&t=408s
Animate shadow opacity instead of animating shadow size.

Twitter and Facobook icons, thanks to www.fontawesome.com

Pictures of city Harderwijk and biking in forest area: https://biketourharderwijk.nl/
Pictures of dears and horses: www.pexels.com
Picture for dialysys center: https://www.dialysecentrumravenstein.nl/
Pictures of nurse and patient:
Picture of 2 working dialyse machines:























