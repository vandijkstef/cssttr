# CSS To the rescue
This repo contains everything regarding CSS to the rescue.
[Styleguide All components](https://vandijkstef.github.io/cssttr/styleguide.html)
[Site with stuff](https://vandijkstef.github.io/cssttr/site/index.html)
[Styleguide w/ site CSS](https://vandijkstef.github.io/cssttr/site/styleguide.html)(Not optimised)

## Usage
If you are on OSX and use Firefox, note you might need to change a keyboard settings. See the know issues for more information.
Any changed HTML will have a class 'changed' attached to it. It will either be explained in a comment or this readme file.

# Issues list
* Only Firefox accepts a fieldset being displayed as flexbox or grid. 
    * Chrome will render the content as being default divs, possible workarounds:
        * Change the fieldset into a regular div. "Fake" the legend
        * Use floats instead
        * Add an extra div in the fieldset to use grid after all [IMPLEMENTED OPTION]
* Firefox on OSX is respecting the system setting under "keyboard -> combinations" and will by default only tab through input fields. Changing this setting will allow to tab through link elements as well
* Checkboxes are not listening to :focus outline and/or border styles, both in Firefox and Chrome, and will render their focus with a default blue outline color

# Process

## Tuesday 6th of February 2018
Placed all components in the styleguide.html. Created basic focus CSS for most of the components.
Explored CSS grid with CSSGridGarden, tried basic use of CSS variables with the colors.

## Thursday 8th of February 2018
Decided to add a div to the fieldset to support grid styling. Discovered that checkboxes are not listening to styles as they should be. Also, input fields are not accepting ::after styles since they are not real 'containers'. Read and used quantity selector (styling by sibling count).

## Tuesday 13th of February 2018
Implemented Fancy ampersands. Implemented De-emphasize by dimming (ratings). Created de-emphasize by blurring, used a small piece of JS for this. Updated the chat and removed a previously added class. Background are now based on the ::before. Extended the clickable area of the button, but cannot downsize focus afterwards since the focus event is fired before any click event has a chance to fire. Played a little bit with the random background pattern, don't fully understand just yet, to be continued...

## Thursday 15th of February 2018
Added custom checkbox. Added loading spinner using the PNG sprite technique, but also using an animated SVG. Played a little more with the random background pattern. Added skip to content link on top of the page. Used a CSS grid to style the chat form, found that textareas dont like to be directly in a grid. Started work on form states, mainly for the input fields. Empty fields shouldn't be invalid, and can be styled using :placeholder-shown, if there is an actual placeholder set, at minumum with a space.

## Tuesday 20th of February 2018
Moving everything over to a site that makes sense, instead of a blob of styleguide.

# Future/Planning/Todo
This section will be updated throughout the process. Items will move over to the Process chapter when completed.
- [ ] Everything hover/focus?
- [ ] Picture with subtitle: Make max 100vh/100vw + caption text
- [ ] Media item as hero banner
- [ ] Extra interaction on the rating
- [ ] Show submenu affordance on nav
- [ ] Create better responsive nav
- [ ] How-to step indicator: Look up examples
- [ ] 
- [ ] Validation formulier (voor <form> zelf)
- [ ] Rework the components into a site that makes sense


# Side-ish
- [ ] What did I learn (doc)
- [ ] Vertical centering (7.40)
- [ ] Intrinsic sizing (7.36)

# Sources

Rating example makes use of Emoji from: http://emojione.com


# Page
Pages:
* Home
	* Media item
* Products
	* Grid layout
	* Product Detail
		* Ratings
* Order
	* Login
	* Progress
* Contact us
	* Chat
	* Form

All pages:
* Nav