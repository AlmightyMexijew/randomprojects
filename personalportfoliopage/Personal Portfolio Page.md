Personal Portfolio Page
User Stories:
1) Your portfolio should have a welcome section with an id of #welcome-section.
2)The welcome section should have an h1 element that contains text
3)Your portfolio should have a projects section with an id of #projects
4)The projects section should contain at least one element with a class of .project-tile to hold a project.
5)The projects section should contain at least one link to a project.
6)Your portfolio should have a navbar with an id of #navbar.
7)The navbar should contain at least one link that you can click on to navigate to different sections of the page.
8)Your portfolio should have a link with an id of #profile-link, which opens your Github or FCC profile.
9)Your portfolio should have at least one media query
10)The height of the welcome section should be equal to the height of the viewport
11)The navbar should always be at the top of the viewport.
---------------
Their example (https://personal-portfolio.freecodecamp.rocks) 
Navbar on top with 3 links (About, Work, Contact). This is red color. It's a flexbox display with a height of 70.8px and a width of 100%.  Height at minimum size is ~62px.

#welcome is a section. also flexbox. Contains an h1 and a p for it. Flexbox seems to be in use to center either the linear-gradient or the text. If the text it's really weird as a design decision. Width is 100% and height is 100vh. This makes it's height always 100% of the viewport height. It takes up more like 110-130% though because when you scroll it leaves what to see in full-screen for the next section(work -> #projects).

#projects is a section. This incorporates grid. The section has an h2 child "These are some of my projects" and then a div for grid, for the wrapper itself. This grid is filled out with items that are the projects.

Each "tile" of the project grid comprises of a link(<a>) with it's child <img> and then a p.
So layout is:
<div class="grid">
    <a class="tile">
        <img>
    <p>paragraph explanation/title

This repeats as many times as necessary to fill the grid.
At the end is a <a> utilizing a button which may be a bootstrap because of classing style.

All links go out in new pages.  The section is about 1/3 page beyond viewheight from how I experienced it.

#contact is the contacts page. Centered h1+h2 saying "Let's work together" and under that is centered links/icons to FB,github,twitter,email,phone.  This is all in flexbox too...as is child div for the links themselves (which makes sense).

#footer is 65.2px at largest content,+20px padding.. States the details are all just fake.
----------
Things I liked:use of linear-gradient(62deg,#3a3d40 0%,#181719 100%); Perhaps change of color could also work on this.