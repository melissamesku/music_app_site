# music_app_site

Visit the site: [http://selus.bitballoon.com/](http://selus.bitballoon.com/)

**Overview**

This one-page website was built according to the design specs of a given PSD file, [Coeluso landing page](https://www.behance.net/gallery/30778403/Coeluso-Mobile-and-Landing-Page). The mission was to turn the PSD file into a functional website with responsive styling and animations. 

**Features**
- fully responsive layout
- hand-coded column layout that does not require the use of floats
- responsive jQuery content slider ([Slippry](http://slippry.com/)), customized 
- animated hamburger menu link using spans

**Tools used**
- Sublime Text 2
- Photoshop CS6
- Chrome browser
- ([Slippry](http://slippry.com/)) jQuery slider

**Tested on**
- Safari
- Firefox
- Chrome
- iPhone 6

**Process**

Starting with the PSD file, I manually saved all necessary assets for web. I then worked my way down the page, writing desktop-layout HTML and CSS for each section in order, refactoring as I went. Not having specifications outlined for responsive styling, I hand-wrote a series of media queries, eschewing tablet and phone breakpoints and working instead directly off how the design behaves on the page at any screen size. 

**What I dig about it**
- I took some liberties, particularly in the content slider which features five spoof testimonials (guest appearances may or may not include such luminaries as Ned Stark, Pee-wee Herman and others).
- I kept basic on-page SEO in mind in my use of `h` tags, meta tags, descriptive image file names, alt attributes on images, etc.
- Clean, DRY, semantic organized code 
- I seldom use gradient backgrounds but this gave me an excuse to play with them. 
- I used a different method of making a hamburger menu link; while it's not perfect, I was happy to try out a new way, and it's animated which is always fun.
- The slider was a joy to work with. Content sliders are a little 2011 these days, and the main way I've worked with them in the past was with old versions of Twitter Bootstrap, or as clunky out-of-the-box WordPress plugins. I remember sliders being a complete pain in the ass, but the Slippry documentation was excellent and customizing it was a cinch. Also, the author's code cascaded down the page in a way I haven't seen CSS written before (always good to see how other people do things).
- The buttons: I used some gentle transitions upon hover and I think they look great.
- Using floats for columns was an old habit, but now avoiding floats for me is second nature. Now if we could only get rid of floats entirely...

**Known issues**
- The radial gradient (under a mockup of a phone in the features section) I tried wrestling with in CSS but to no avail; I haven't yet figured out how to change the angled view aspect of the gradient. I ended up settling with a .png of the radial from Photoshop. At the 680px breakpoint, I got rid of the radial with `display:none` because it starts to compete with the surrounding text. 
- I made an executive decision to forego the aforementioned phone element at the 510px breakpoint because the layout gets a bit crowded and I felt the image had been represented enough in other places throughout the site. A better solution might be to make the phone element pop out of the columns and appear above instead. 
- Also at the 510px breakpoint, the section I call "sideways" has text on top of a .png. I think it looks cool but it should be adjusted to fix readability issues.
- The hamburger menu link spans are clickable while the space between them is not; this makes the menu totally functional for touch-based interaction but less than ideal for mouse clicks which are more precise.
- The design would be more complete were I to build out a fake menu for that hamburger button to link to. 
