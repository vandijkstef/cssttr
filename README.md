# CSS To the rescue
This repo contains everything regarding CSS to the rescue.
[Styleguide All components](https://vandijkstef.github.io/cssttr/styleguide.html)

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
Implemented Fancy ampersands. Implemented De-emphasize by dimming (ratings). Created de-emphasize by blurring, used a small piece of JS for this.

# Future/Planning/Todo
This section will be updated throughout the process. Items will move over to the Process chapter when completed.
- [ ] Chat before background styling
- [ ] Intrinsic sizing (7.36)
- [ ] Vertical centering (7.40)
- [ ] Loading Spinner (8.43)
- [ ] Extending the clickable area (6.30)
- [ ] Custom Checkboxes (6.31)
- [ ] (pseudo) Random background (2.7)
- [ ] Validatie formulier?
- [ ] Provide skip to content link on top of the page (with concern of any autofocus fields on the page)
- [ ] Decide on advanced features

# Sources

Rating example makes use of Emoji from: http://emojione.com
