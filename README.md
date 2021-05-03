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

But the real inspiration came when I saw this bike site:(https://biketourharderwijk.nl/) (not even a dialysis site)
The pictures of the carousel blowed me away, I decided from that moment my front page of the project must be a carousel in a rectangle format.

## The start
On start I thought to make a website based on one big background picture of the rural area with a big title and subtitle, all to create that holiday dialyse feeling.
With scrolling the information moves over te background picture. The technique was inspired from this idea: (https://valentina-b.github.io/par-excellance-restaurant/). 
Than other pictures of specific dialyse treatment should appear in a carousel after some scrolling.
In that first stage the mentor advised to use smaller pictures and add more text, because the purpose of the website (atract guests who wants to book dialyse treatments) wasn't clear enough. Also he advised to use a Google Map image for a better understanding where the center is situated.

Then after research I knew that I wanted a rectangular carousel with a fading effect in it, with a text column on the left with a little bit tourist information of the area "The Veluwe" and with a text that guests are welcome to come. The right column is the intro part for the center.
The About section gives more information about he center. De contact page gives information to get into contact.

## Structure
###Section1
* The homepage features a responsive navigationbar on the right and a logo on the left top, this bar is fixed. On mobile screens left en right side will split en become centered   in top of each order.
  The navigationbar has also a language button. With javascript and display=none and display=inline, the right language appear in front without loading the whole page.
* Below that is a fading carousel as the hero image. I didn't want to add control buttons to swap the images by hand, just images with a fading effect to each, for designing purposes.
  In that fading carousel a title "Holiday Dialysis" appears with a linear-gradient background directly under that text.
  In smaller devices the title becomes too big according to the pictures of the carousel, therefore the title emerges down the pictures in mobiles.
* Below are 2 columns of text. They appear down each other on a mobile device.

###Section2
* In section 2 a second, normal carousel appears with some dialyse pictures. It is attached to the text column underneath. On the right there is a picture of the fantasy dialyse   center, also attached to the unordered list underneath. 
* On mobile devices it wil appear below each other.

###Section3
* In desktop-devices section 3 appears as 3 column area. On the left side there's Google Map Iframe, the middle a form, and to the right a picture with adress.
* On tablet devices it breaks into a googlemap area with underneath a form and picture with adress on the left and right side. It is made possible by using a nested bootstrap Col element
* On a mobile device everything appears below each other.

### Shadow, hover and transition effect after hover
To give this webpage a finishing feel, I have put a shadoweffect on the images, carousels and google map. Then I added a transition effect after hovering as wel, but only for laptop en desktop devices because it appears not realy to be cool for a small device. I discovered that the fading carousel didn't want to hover. The reason must have been it's relative position, because of the title "Holiday Dialysis" absolute position in it. I saw it wasn't really necaserry for the title's position, so I removed the "relative position line", that works because the body itself is also relative. All titles have also some transition on it. For alle devices icons and navigation have a hovering effect. 

###footer
* On the left 2 icons appear with Facebook and Twitter, on the right a copyright mark appears. 2 Social media links are enough for this site. A hospital isn't that much into social media.

##Technologies
1. HTML
2. CSS
3. Bootstrap
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


The media query for the collapsed navbar regardless of viewport width was taken from this [site](https://www.codeply.com/go/iaM1zcNsQB/bootstrap-navbar-always-collapsed).










