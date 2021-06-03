
### [Table of Contents](https://wondwosentsige.github.io/code-401-reading-notes/Home)

## Read Class 01

### Responsive web design & Floats


- Responsive web design (RWD )is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop.

#### Responsive vs. Adaptive vs. Mobile

- Responsive and adaptive web design are closely related, and often transposed as one in the same. Responsive generally means to react quickly and positively to any change, while adaptive means to be easily modified for a new purpose or situation, such as change. 

- Mobile, on the other hand, generally means to build a separate website commonly on a new domain solely for mobile users


#### Flexible Layouts

- *Responsive web design is broken down into three main components, including flexible layouts, media queries, and flexible media.*

- __Flexible layouts,__ is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width. 

- Flexible layouts do not advocate the use of fixed measurement units, such as pixels or inches. Reason being, the viewport height and width continually change from device to device.


#### Media Queries

- Media queries were built as an extension to media types commonly found when targeting and including styles. *Media queries provide the ability to specify different styles for individual browser and device circumstances*, the width of the viewport or device orientation.

- __Initializing Media Queries__


- Within responsive design the most commonly used features include min-width and max-width. These help build responsive websites on desktops and mobile devices equally, avoiding any confusion with device features. Example:- __@media all and (min-width: 320px) and (max-width: 780px) {...}__

- __Mobile First__:- The mobile first approach includes using styles targeted at smaller viewports as the default styles for a website, then use media queries to add styles as the viewport grows.


- __Viewport Height & Width__:- *Using the viewport meta tag with either the height or width values will define the height or width of the viewport respectively*. Each value accepts either a positive integer or keyword. For the height property the keyword device-height value is accepted, and for the width property the keyword device-width is accepted.

- For the best results, and the best looking website, it is recommend that you use the device defaults by applying the device-height and device-width values.



#### Float

- There are four valid values for the float property. *Left and Right float* elements those directions respectively. *None* (the default) ensures the element will not float and *Inherit* which will assume the float value from that elements parent element.

- Floats can be used to create entire web layouts.











...............................................................................

__Attributions for the following Reference materials and their authors__


[Shay Howe’s intro to RWD](https://learn.shayhowe.com/advanced-html-css/responsive-web-design)

[All about floats](https://css-tricks.com/all-about-floats/)

[SMACSS official documentation](http://smacss.com/)




[>> NEXT (Read-02)](https://wondwosentsige.github.io/code-301-reading-notes/class-02)
