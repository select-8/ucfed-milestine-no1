# USER CENTRIC FRONT END MILESTONE PROJECT

## STATIC WEBSITE FOR THE FOLK-ROCK BAND _BIG THIEF_

## Project Overview

For this project, I have built a mobile-first responsive website for the rock group Big Thief. It can be viewed [here](https://select-8.github.io/ucfed-milestone-no1/index.html).

Relatively new to the music of Big Thief, from the moment I heard the song _Cattails_ I was drawn in by their sound and aesthetic. My hope is this has somehow seeped into the project presented here.

My primary goal was to make the best site I could, utilising and building upon the processes and technologies outlined throughout the User Centric Front End Development modules and to take the initial steps towards developing my own working method as a web developer. 

For the most part I'm happy I have met these goals, at the very least I now have a much clearer understanding about what I don't know yet!

The site consists of 5 linked pages. It incorporates main navigation, grid layout, display and text utilities, and modal components provided by Bootstrap.

All links have functioning endpoints. The mailing list goes nowhere.

I used Notion as a project management tool. I created a sprint with bite-sized tasks. This can be viewed by anyone with an @codeinstitute.net email [here] (https://www.notion.so/liamucmsp/e0125f6404bb4daaa59b5b10da2a7415?v=04742600702b4e64a04207bb24732246).


### Strategy Plane

#### Owner Stories

The band has a strong brand and aesthetic that suggests the standard indie-music trope of "It's all about the music". The website needs to reflect this while still presenting commercial opportunities outside of music streams. 

To this end, we need a website to:

1. Promote the band's music and brand

2. Target fans with merchandise and tickets to live shows

3. Showcase music

  - audio clips

  - new album just out to promote 

  - rave reviews from the right places

4. Publicise availability (tour)

   - dates, locations, links to buy tickets

   - hero image of a live show atmosphere

4. Show photos of the band members

     - should fit the brand

5. Show videos

     - a mix of staged and live

7. Show social media presence

#### Inspiration - The persona of Big Thief

Inspiration for the site's content as well as the general look and feel came mainly from the band's own website, their music and lyrics, and from various interviews I have read or seen with the group. Their persona, in particular that of the band's leader and songwriter Adrianne Lenker, is one of mystery, darkness, and contrast.

      I'll be your real tough cookie with the whiskey breath
      I'll be a killer and a thriller and the cause of our death

- https://bigthief.net 
- https://www.stereogum.com/2014756/adrianne-lenker-big-thief-interview-abysskiss/franchises/interview/

## UX Process

### Scope Plane

#### User Stories 

As a user I want to be able to:

 1 seamlessly navigate to the content I want.

 2 seamlessly wander the site till I find something that interests me

Two types of users can be defined:

1. I’m already a fan of the band, I have all their albums

    - As a user I expect the site to reflect the persona of the band.
    - As a user, I want easy access to unique content i.e. access to an official store, definitive tour listings.

2. I have just heard of this band and I want to find out more…

    - As a user, I want access to the band's social media.
    - As a user, I want to hear some of this bands music.
    - As a user, I want to see their music videos.
    - As a user, I want to see some live performances.
    - As a user, I want access to biographic information on the group

_In potential conflicts between users requirements, reflecting the band's persona wins out_

### Structure Plane
#### Information Architechture

![](user_experience_assets/Info-arch.png)

### Skeleton Plane
#### Wireframes

Wireframes can be viewed here.

wireframe_1.jpg shows my initial mind dump.

Initially, I planned for the site to scroll vertically, with distinct page blocks for each section. However, I quickly decided to go with single pages. I don't like a sticky navbar and early on couldn't find a simple enough (non-javascript) alternative I liked to do navigation back up and through the pages. I had thought that I might switch back once all the pages were completed but in the end, I prefer the single linked pages layout for this project. Finding a nice way of internal navigation for a vertical scrolling site is a goal I've set myself for future projects.

The idea of pages split into 4 quads in a single view came to me early in the project. I wanted symmetry of content with left/right & top/bottom used to imply levels of importance in the content for the user. On moving from desktop to mobile the bottom right would fall down/off first, then bottom left, top right, top left.

In hindsight, this approach to the UX has not worked as I would have liked, particularly on the music and video pages where I feel the content, between both the titles and iframes and the quad divs themselves, could do with more room to breathe as they react to the responsive design.

I did not wireframe the tour page. I knew I would use a Bootstrap table and that it would mirror the home page.

### Surface Plane
#### Colour 

I wanted to use a high contrasting palette of colors which could portray the sense of mystery and intensity outlined in the user stories. To this end, the site is bookended by the lighter in tone, pink backgrounded, Home & Tour pages, while the core pages of music, videos, and store are dark with high contrast between the blacks, whites, and oranges.

Light home -> darker content pages -> light tour

This is intended to make the user feel like they are going "inside" the site from the home page.

#### Typography

The site makes use of two fonts.

I wanted to use a serif font for banner headings like the band's name on the home page, and sans serif for content paragraphs. 

I choose Cinzal as my serif font. Using a serif gives a sense of grandeur to the title and fits with the band's brand. 

Google fonts suggested Lato as a complimenting font.

The formatting of the text and some decoration on the quotes section of the music page proved to be the most challenging aspect I faced in terms of type.

I would have liked to have been able to do more with the video titles.

The store page makes heavy use of Font Awesome icons. Ideally, I would have custom made some SVGs that better suited the band's persona. Saying that, in general, I think the quad approach to the design works best on this page.

#### Images

The home page image was chosen for its clear and natural portrayal of the group. The tone and form of the image informed the overall aesthetic of the site.
The tour page was chosen to give a sense of the atmosphere a user can expect at one of Big Thief's shows i.e. up close, intense and intimate. 

## FEATURES

#### Navbar
This is a Bootstrap component. Fixed to the top of the screen, it
collapses to dropdown for mobile screens. I choose to justify the link text across the bar to give that sense of symmetry and balance to the site. I did play with the idea of setting the button itself in the centre of the navbar but this just looked a bit weird.
As it is, I feel the navigation allows users to easily jump from one page to another and back without any confusion.

#### Footer

Apart from using W3Schools CSS for the drop up effect and reappropriating some Whiskey Drop code for the modal and using Font Awesome icons, the footer is 100% custom built!
On the right, we have some social icons as block text which collapse to a social button drop-up for mobile. On the left, we have a mailing icon which houses a modal pop-up form. This responsive feature allows users to navigate to the band's social sites in a new tab. 

The block stacking means, for the most part, the icons will not overlay the content on medium to large screens.

The Wikipedia link meets the needs of the new user outlined in the user stories above. It also meets the needs of the owner in keeping content inline with the persona of the band.

Has a mailing icon which has a modal form pop up on click.

Both of these features use colour and hover effects which are responsive to the user being in either one of the light or dark pages

#### Iframes

The music and video pages use Spotify and YouTube embed code respectively. These meet the user and owner needs outlined above.

#### Ticket Links

Every link links to the same Ticketmaster page. I had toyed with the idea of having a single link, sitting in either the banner text, the image or the navbar but in the end, I decided that this would distract from the overall design of the page. For the same reason social and mailing list links do not appear on this page.

#### Left to Implement

- iframes more responsive to media screen size
- floating, down pointer on tour page to disappear on scroll
- make the band's name appear opaque behind the dropdown menu

## Testing

My testing spreadsheet can be found [here](testing/site-tests.xls).

Mostly my breakpoints happen at the mid-size screen level, therefore I tested the responsiveness of content either side of this divide.

Further to this, the site was tested on a variety of devices using Google Chrome Dev Tools and physically using a RedMi Android phone, an iPhone 8 and a Samsung Galaxy Tablet.

####Results

 - Conflict in z-indexing of music/video/store content/links and the mailing/social links that make up the footer. It's a fine margin, but when they overlap only the higher indexed item will work. This does not meet the users need for seamless navigation and control of the content.

 - Scrolling was found to be laggy on the Galaxy Tablet.

 - Spotify iFrames are too wide on iPhone 8

 - Not enough space under the music and video pages.

Through the project I made use of the CSS code snippet below. I found it very useful for finding CSS and HTML gremlins.


     *  {
    background: #000 !important;

    color: #0f0 !important;

    outline: solid #f00 1px !important;
    }


## Deployment

I have used Git for versioning. The site is deployed to GitHub pages at the address given at the top of this readme.

There is no difference between the development and deployed versions of the site.


## Technologies Used

##### LANGUAGES
- HTML
- CSS

##### VERSION CONTROL
- GIT

##### FRAMEWORKS & APIS
- BOOTSTRAP 4
- FONT AWESOME
- GOOGLE FONTS
- JQUERY
- POPPER

##### SOFTWARE AND SERVICES
- AWS Could9 IDE
- VISUAL STUDIO CODE
- GITHUB
- INKSCAPE

##### EDITORS
- Sublime
- Atom

##### VMWARE
- Ubuntu V18.04

##### HARDWARE
- Mac OSX

##### PROJECT MGMT
- SLACK
- Notion

## Credits
I used [this](https://stackoverflow.com/questions/41651612/how-to-align-icon-to-center-inside-div-element) to center some content, turned out to be more hassle than it was worth.

The bones of the modal was taken from Matt's Whiskey Drop walkthrough.

The drop-up CSS came from W3Schools [here](https://www.w3schools.com/howto/howto_css_dropup.asp).

The Home page banner image is by Michael Buishas and was found on NPR's site [here](https://www.npr.org/sections/allsongs/2019/02/26/697748344/big-thief-announces-a-new-album-u-f-o-f-and-releases-its-first-single).

The Tour page image is by Kate Johnston and was found on The Skinny website [here](https://www.theskinny.co.uk/music/live-music/reviews/big-thief-swg3-glasgow-19-may)

