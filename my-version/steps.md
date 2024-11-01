head of html
meta tags:
utf8
viewport
import google fonts with open sans font
import fontawesome
title of page
link in css stylesheet
link favicon

add base styles:
css reset
body:font, line height
anchor tags: no underline and color of #333
ul: take away bullets
img:max-width

Header and navigation
html:
make tag for the header with a class of header
make a div that's a container for the whole header with classes container and header-flex
add the lumina logo with a class of logo
wrap the ul with a class of main-menu in a nav with the items of home, about, & contact as links

css:
container
give the container a max-width
put it into the center of it's container
give it space inside of 0 top/bottom 1.5rem left/right

make a .container-lg class and give it a max width of 1400px
make a container-sm class with a max-width of 900px

header:
give the header margin of 1.5rem top/bottom leff/right auto

set the image to a width of 130px

now target the header-flex class
make it a flex container
make space between the logo and list
make the image be in the middle of the cross-axis

now target the list:
make it horizontal
give elements 1 rem of space between each other

give the links space inside the element on the top/bottom of 0.5rem and 1rem left/right

give the links a background of #fcf5e9 if hovered

make a .current class give it to the home page element and give it a background of the same as above
and make it bolder with a value of 600

make a media query at 768 for the header-flex item
and make it vertical
add 1.5rem of space between logo and links

HERO TEXT
html
make a section with the class of hero
make a div with the container class and container-sm class
put in the hero text
wrap the first and last words of the text with an element and give it a class of bg-primary

css:
hero section
give height of 500px
make a flex container
align items center on main & cross axis
make sure text is aligned in the middle

hero text:
size of 3rem
space between lines of 1.4
less bold with a setting of normal

make a section for utility classes right above the container section and below the global styles

give it a background of #fcf5e9;

make a media query to make the h2 smaller
give the hero container less height of 300px
size of hero text 1.8rem

CUSTOM PROPERTIES
target the root element :root {}
name it primary color: --primary-color:#fcf5e9
insert it every place it's needed var(--primary-color)
do it for the container width as well:
normal, wide and narrow

GALLERY SECTION
make a section with a class of gallery
div with a class of container container-lg gallery-flex
gallery items:
make a div for each gallery item with a class of gallery-item
make it a link that links to the picture
inside the link put the image (will be the portfolio number)

styles:
targer the gallery-flex
make it a flex container
center items on the main axis
make the items wrap
give 20px of space between each flex item

target the gallery item
make the width so that 3 items can fit into it and account for the 20px of space

target the image
give it a round border 10px

make gallery item transparent wen hovered
opacity 0.9

add media query to make each row of images show 2 images

FOOTER
html
make a footer element with class of footer
make a container with class container and footer-flex
add in our 3 flex items: logo,contact div(class of contact):with h4 and list with contact info social div with:h4 and list of social media items(add fa-2x to the end of each item to make bigger)

styling
footer

add a border to the top color of #aaa really skinny
add space at the top/bottom inside the element of 2rem 1.5rem left/right inside the element
add space above the element at the top of 2 rem

for the h4:
text should be 1rem
space on the bottom outside the element 0.5 rem

for the links:
space outside the element (all sides) 0.2 rem

media query for the footer:
target the footer flex class
make items display vertically
center items on main/cross axis
make text be in center
add 1rem of space between each element

ABOUT PAGE
copy over header/hero/footer from home page
change the home href to /
make the link that's highlighted the about link

services section
html
make a section with the class of services
give it a container
in the container 2 divs
1 div:h2 with a class of section-heading that we'll use as a utility class

CSS
for the services section:
background of #333
white text
space inside the section:3rem top 0left/right 4rem bottom

services flex
make the service items display horizontally
2rem of space between service items

h4's in the service items
text size of 1.1rem
space outside the element on the bottom of 0.7rem

h2 section heading:
text size of 1.6rem
make text be in the center
space below the element on the outside of 2rem

TEAM SECTION
section with class of team
container div with class of container & container-lg
h2 with class of section-heading

team-flex container with class of team-flex
3 team items each one will have
img
h4
paragraph

CSS
the team section will have space inside the element ontop 3rem 0left/right 4rem bottom

team-flex:
make it a flex container
add 1.4rem of space between elements

add rounded corners to the img

CONTACT PAGE
copy header footer and hero text from about page
change the hero text to what it's supposed to be
make sure the proper link at the top has a background

since we are using the same dark background in our about page
for the hero text make a utility class name .bg-dark and make a variable for the dark color #333 since the background is dark we have to change the color of the text

go to our about page and add the bg-dark class to the services section and remove the css so the class is the one determining the background

in our hero section add the bg-dark class to make the background dark and text light

make a utility class that targets the spans inside the hero text
and give space inside the element on left/right of 0.3 rem

make a section for the contact info with the class of contact
make a container with the class of container and container-sm
make an h2 with the class of section-heading
add the paragraph right below the h2
make a form
for each input add a label and give it a class of visually-hidden
cause we're not gonna use the label but we need it for accessibility
also wrap each input/label in a div with the class of form-group

lookup how to do a visually hidden class (there's a good link on a11yproject) and add that to css and add it to the utility classes

Contact styles
give the entire contact section some space inside the element of 3rem on top 0 left/right 4rem below

make the text in the paragraph be centered
add 2 rem of space outside the element below

form group items
add 2rem of space above and below the items on the outside

target the input and the textarea at the same time for this:
give it a bottom border but to do so we have to set a border of none first bottom border 1px solid #333
make the width all of the container
give space on the bottom inside the element

make the textarea taller at a size of 200px

make the textare and inputs when you focus(click on them)
have no outline

style the button make a utility class incase we use elsewhere:
we want it as an inline-block element
add some space on the inside of the element 1rem top/bottom 2rem left/right

border of 1px solid #333
background transparent
make cursor a pointer

on hover: .bg-dark class

target the button that is in this contact form
and make the width 100%

Image lightbox affect
go to cdnjs and search up lightbox
copy the css link and paste it on the index page
copy the js tag and link it at the end of the body but not outside
do the same for jquery cause its a dependency

on the links add data-lightbox="image-1" data-title="image-1"
