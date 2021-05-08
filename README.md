# Holiday Dialysis
### First Milestone Project: User Centric Frontend Development - Code Institute

This project is a one page website about a Dialysis Center in the middle of The Netherlands. They offer a dialysis treatment for people who suffer from kidney failure and are open for guests who are on holiday. This is a made up center in the small city of Harderwijk, but actually I work in a real dialysis center in Harderwijk. It is also a satelite center of the big one in Amersfoort, 30km from Harderwijk. Important: this project is meant for the post-corona era, off course the situation will become better the comming months and certainly in 2022.

For a demo of my Holiday Dialysis Website click [HERE](https://kriz-hub.github.io/Holiday-Dialysis/).

![Desktop Demo](https://github.com/Kriz-hub/Holiday-Dialysis/blob/master/Animatie.gif)

## UX
From a financial point of view it is very interesting for a hospital to add guests to their patient population. A descent website helps to get a good representation.
I know there is a real demand for a good website for the real dialysis center I work in, first one for holiday guests, later for the dialysis center as a whole.
To prevent that the Milestone 1 project will become too big, I am focussed on the part of Holiday Dialysis.

Business goals:
To get guests interested for this center, there are more to choose in a radius of 50 km. It's a tourist area, that also means they can atract the foreign guest.
The website must not be for a too young audience, the population which is interesting for a dialysis center is mainly 40 years and older.
The next goal for a center to have a descent website is simply to create goodwill, be representive.

Customer goals:
The kidney patient needs 3 times a week dialysis in his own center, but also wants to have an opportunity to get on holiday.
He needs to be informed which center he can choose and what they can offer him. So the website must be informing but not too corporate. He is in the mood for holiday and that mood should reflect the website. 

## The start
On start I thought to make a website based on one big background picture of the rural area with a big title and subtitle, all to create that holiday dialyse feeling.
With scrolling the information moves over te background picture. Than other pictures of specific dialyse treatment should appear in a carousel after some scrolling. The technique was inspired from this idea: https://valentina-b.github.io/par-excellance-restaurant/. 

In that first stage the mentor advised me to use smaller pictures and add more text, because the purpose of the website (atract guests who wants to book dialyse treatments) wasn't clear enough. Also he advised to use a Google Maps image for a better understanding where the center is situated. After that my idea at the beginning changed a lot, see also the "Skeleton" section for that change.

## Research

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

## Structure
#### Section 1
* The homepage features a responsive navigationbar on the right and a logo on the left top, this bar is fixed. On mobile screens left en right side of navbar will split and become centered in top of each order. The navigationbar has also a language button. With javascript and display=none and display=inline, the right language appear in front without loading the   whole page.
* Below that is a fading carousel as the hero image. I didn't want to add control buttons to swap the images by hand, just images with a fading effect to each. In that fading carousel a title "Holiday Dialysis" appears with a linear-gradient background directly underneath the text.
  In smaller devices the title becomes too big according to the pictures of the carousel, therefore the title "Holiday Dialysis" emerges down the carousel in smartphones
* Below are 2 columns of text. They appear down each other on a mobile device.

#### Section 2
* In section 2 a second, normal, carousel appears with some dialyse pictures. It is attached to the text column underneath. On the right there is a picture of the fantasy dialyse center, also attached to the unordered list underneath. 
* On mobile devices it wil appear below each other.

#### Section 3
* In desktop-devices section 3 appears as 3 column area. On the left side there's Google Maps Iframe, the middle a form column, and to the right a picture column with adress.
* On tablet devices it breaks into a googlemap area with underneath a form and picture with adress on the left and right side. It is made possible by using a nested bootstrap Col element.
* On a mobile device everything appears below each other.

#### Footer
On the left 2 icons appear with Facebook and Twitter, on the right a copyright mark appears. Facebook and Twitter is enough for this site. Hospitals aren't that much into social media.

#### Shadow, Hover Animation and Shadow Animation Effect during hover
To give this webpage a finishing feel, I have put a shadow effect on the images, carousels and on Google Maps. Then I added a transition effect after hovering as well, but only for laptop en desktop devices because it appears not really to be that cool for a small device. I discovered that the animation effect on the fading carousel didn't work. The reason must have been it's relative position, because of the title "Holiday Dialysis" absolute position in it. I saw it wasn't really necessary for the title's position, so I removed the "relative position line". The title kept on the same place because the body itself is also relative, so that change worked succesfully also with a good hovering now.

To get this project really finished I added shadow animation with the hovering animation, so there is an increase of shadow now during transition animation on image. I saw an interesting youtube to do it in a way to keep the rendering significant lower, which is good for older devices, see Acknowledgements. The trick is to animate opacity instead of animating shadow size.

All titles also have some hover transition on it. For the smaller devices only icons and navigation have a hovering effect. 

## Skeleton
The wireframe was made in [Balsamiq](https://balsamiq.com/). My only thought first was to get it right on my laptop. I hadn't much of an idea how to get it on smaller devices. This were the early wireframes: 
* [Section1: Home](https://github.com/Kriz-hub/Holiday-Dialysis/blob/master/OldWireframes/Wireframe%201.png)
* [Section2: About](https://github.com/Kriz-hub/Holiday-Dialysis/blob/master/OldWireframes/Wireframe%202.png )
* [Section3: Contact](https://github.com/Kriz-hub/Holiday-Dialysis/blob/master/OldWireframes/Wireframe%203.png)

Later it evolved to a responsive idea :
* laptop/desktop:
  * [Section1: Home](https://github.com/Kriz-hub/Holiday-Dialysis/blob/master/NewWireframes/section%201%2C%20home.jpg)
  * [Section2: About](https://github.com/Kriz-hub/Holiday-Dialysis/blob/master/NewWireframes/section%202%2C%20about.jpg)
  * [Section3: Contact](https://github.com/Kriz-hub/Holiday-Dialysis/blob/master/NewWireframes/section%203%2C%20contact.jpg)
* Tablet: The tablet views the same in panorama view.
          when it is on "portrait view" section3 is ordered on a slightly different way with google maps on top:
          [Section3: Contact](https://github.com/Kriz-hub/Holiday-Dialysis/blob/master/NewWireframes/tablet%20section%203%2C%20dif%20layout%20as%20desktop.jpg)
* Smartphone:
  All collumns appear underneath each other and the top bar appearance is a split in 2 parts on top:
  [Image A](https://github.com/Kriz-hub/Holiday-Dialysis/blob/master/NewWireframes/smartphone%2C%20a%20%26%20b.jpg), [Image B](https://github.com/Kriz-hub/Holiday-Dialysis/blob/master/NewWireframes/smartphone%2C%20c%20%26%20d.jpg), [Image C](https://github.com/Kriz-hub/Holiday-Dialysis/blob/master/NewWireframes/smartphone%2C%20e%20%26%20f.jpg). 
  
## Technologies
1. HTML
2. CSS
3. Bootstrap version 4.0.0
4. Javascript

## Features
The user can click on Home, About and Contact for going to Section 1,  Section 2 or Section 3.
By clicking on the flag image he can choose the language he prefers. Also he can navigate to the sections by just scrolling because all is in one page.
At Section 3 the user can fill in a form to send his phone number, email adress or comments, than he can be contacted back.
In the footer section he can click on the icon links.

## Features left to implement
The behaviour of the scroll-spy is somewhat pour, I was forced to add some empty text to get it right on the pages. With a little bit more knowlegde of Javascript I could make a custom scroll-spy myself. I think I would use "100vh", because that's alway the screensize vertically. Then use a way to get the current screenposition relatively to "100vh", then give a command to make some lines of scrolling.

## Testing
* The site is tested on a real Samsung S7, Samsung A32 and Samsung A52, on there own browser.
* also on 2 tablets: Asus Transformer Pad (an old one) and Lenovo TB-X10AF, both on a Chrome browser
* screens: 1366x768, 1920x1080 on Chrome and Edge.

## Bugs
* I found out that the landscape view of a tablet also have shadow hovering. I wanted that only to be for laptop an desktop. It's not that important, I leave it that way.
* I didn't get that shadow hovering working well for Google Maps, but it's initial shadow effect remains as well. Therefore I leave it that way, It don't seems to be that noticable.

## Deployment
This project was developed using GitHub.

I followed the next steps to deploy my page on the GitHub pages:

* Log into GitHub.
* Select krizhub-Holiday-Dialysis in the repository list.
* Go to Settings.
* Scroll down to the GitHub Pages section.
* Select the Master Branch.
* On selecting Master Branch the page is automatically refreshed, the website is deployed.
* The link can be retrieved to the deployed website.

## Credits
* All content in the CSS-section and the index.html is written by myself.
* Twitter and Facebook icons, thanks to www.fontawesome.com
* Pictures of "City Harderwijk" and "Biking in forest area": https://biketourharderwijk.nl/
* Pictures of "Dears" and "Horses": www.pexels.com
* Picture for dialysys center: https://www.dialysecentrumravenstein.nl/
* Pictures of nurse and patient: https://thumbs.dreamstime.com
* Picture of 2 working dialyse machines:  https://thumbs.dreamstime.com

## Acknowledgements

* To get af flag image into a button and customizing it: https://stackoverflow.com/questions/49184471/how-to-change-bootstrap-version-4-button-color 
* Creating a feading carousel on section1:  https://silvawebdesigns.com/how-to-change-the-bootstrap-4-carousel-to-a-fade-transition-instead-of-slide/
* To get a normal carousel on section2:  https://getbootstrap.com/docs/4.0/components/carousel/ 
* To get a responsive Google Maps thanks to: https://blog.duda.co/responsive-google-maps-for-your-website 
* Form class with bootstrap: https://getbootstrap.com/docs/4.1/components/forms/
* Inspiration to get a multi language page working:
  https://stackoverflow.com/questions/46008760/how-to-build-multiple-language-website-using-pure-html-js-jquery
  It's all about the mentioning of "display:none" on that site. That reminded me to my own litle project "5 days of coding challenge", where I used it to hide pictures. Now I used the idea "display:none" and "display:inline" to make a multi language site without the need to load the whole website again when changing language. (And to prevent coding from repeating because the other way is make 2 different pages.)
* Shadow on carousel and images:  https://www.w3schools.com/css/css3_shadows_box.asp
* Youtube of Kevin Powel: https://www.youtube.com/watch?v=u6Rur7G8HNY&t=408s
  Animate shadow opacity instead of animating shadow size to reduce rendering of processor.
* Section 2 "Your stay with us", inspirated by https://www.dialysecentrumravenstein.nl/dialysis-centre-ravenstein/. See paragraph "contact" on that page.
* section 2 the unordered list underneath "Our center offers.. " is inspirated by https://www.roompot.nl/care/behandelingen/vakantiedialyse/banjaard/. See the unordered list on that page.
  
  I want to thank my mentor M for guiding me through the process and keeping me inspirated.

























