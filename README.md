# css-layout-basics
TeamTreehouse/Tracks/Web Design


::::::::::::::::::::::About this Course::::::::::::::::::::::::::::::::
Learn to work with common layout and positioning methods used in web design. In this course, you'll get hands-on practice with basic CSS layout techniques like display modes and floats. You'll use your new CSS layout skills to build the layout for a simple web page. Then learn to enhance the layout using relative, absolute and fixed positioning.

>>>>>>>>>>>>>>>>>>>>>>Getting Started with CSS Layout<<<<<<<<<<<<<<<<<<<<<<
This stage covers layout tips and techniques used by web designers. You'll learn about CSS resets, layout wrappers, creating a sticky footer, and more.

->>>>>>>>>>>What to Expect:
Good use of CSS layout is important when building a website or app. No matter what type of site or app you want to build, you will use one -- or several -- CSS layout methods to arrange the content on the page.

->>>>>>>>>>>CSS Reset with Normalize:
A CSS reset removes the subtle browser inconsistencies in margins, padding, line-height and font sizes to ensure that your layout displays as consistently as possible across all browsers.

Resources:
1. https://necolas.github.io/normalize.css/
2. http://nicolasgallagher.com/about-normalize-css/

Other CSS reset methods:
1. https://meyerweb.com/eric/tools/css/reset/
2. https://cssreset.com/

->>>>>>>>>>>>>>>>Creating a Layout Wrapper:
A wrapper is commonly used to center a layout on the page. The wrapper keeps a layout from looking too wide or too narrow depending on the device or viewport width. This video covers two common ways to create a wrapper in your layout.

Video review:
1. Giving the wrapper a width prevents the layout from stretching too wide.
2. Setting the left and right margins to the value auto centers the wrapper in the browser.
3. One advantage to using <body> as the wrapper is that you don’t have to add an extra <div> in your markup to contain your layout.
4. If you want to give your page a full background color or image, you'll need to apply it to the <html> element, and you can't place any elements outside of the <body>.
5. Using a wrapper <div> is more appropriate if your site has elements that need to be placed outside the wrapper.

->>>>>>>>>>>>>>>>>>>Why Vertical Margins Collapse:
In this video, you'll learn why vertical margins collapse and how to prevent them from collapsing.

Resources:
1. https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Box_Model/Mastering_margin_collapsing

Video review:
1. If there is no content, padding, or border area to interrupt two touching margins, the margins collapse to the largest of the two margin values.
2. You may experience margins collapsing in adjacent elements like paragraphs and divs.
3. If a div's bottom margin is larger than the top margin of the div below it, the margin area between the divs collapses to the largest of the two margin values.
 
->>>>>>>>>>>>>>>>>>>>>Centering Page Content and Creating a Full-width Header:
A common layout structure in web design involves a centered content area with a header and footer that take up the full width of the page.

Video review:
1. Depending on your design, you may want the header and footer in your layout to stretch from edge to edge of the browser so the left and right sides won't appear cut off.
2. This approach makes the layout feel open and less constrained.
3. One approach is to create a wrapper the main content and an inner wrapper for the content inside the header and footer.
4. You can leave 'outer' elements like the header and footer at their default 100% width.
5. It's common to have more than one wrapper on a page and even to have containers inside of containers.

->Using a Mobile First Approach:
When you use a mobile-first layout approach with CSS, you serve the basic layout styles and minimal amount of code to style a page for a small, mobile device first. Then, using media queries, you add breakpoints which adjust the layout for wider screens and devices.

Resources: 
1. https://zurb.com/word/mobile-first
2. http://bradfrost.com/blog/web/mobile-first-responsive-web-design/
3. http://blog.teamtreehouse.com/box-sizing-secret-simple-css-layouts
4. http://blog.teamtreehouse.com/take-control-of-the-box-model-with-box-sizing

Video review:
1. It's easier to build a mobile layout when you're first starting out because you don't have to worry about any of the complex features of wider, desktop layouts.
2. Mobile layouts are usually simple one column layouts
3. When you use a mobile-first layout approach, you define all the common layout styles before adding any media queries.
4. box-sizing: border-box; forces any padding and borders into the width and height of an element instead of expanding it.

>>>>>>>>>>>>>>>>>>>>>>Controlling Layout with CSS Display Modes<<<<<<<<<<<<
Learn to control elements in your layout using common CSS display modes like block, inline, and inline-block. Understanding the differences between these display settings will help take your CSS layouts to the next level.

->Positioning Elements Side-By-Side with Inline Display:
In this video, you'll learn how changing element display values from block to inline affects surrounding elements and the space they take up on a page. For instance, you can make list items, which normally appear stacked on top of each other, appear side by side to form a navigation bar.

Resources:
1. https://developer.mozilla.org/en-US/docs/Web/CSS/display

Video review:
1. Inline elements, like images, links and span tags, do not create line breaks in a layout; they appear on the same line as the content and elements beside them.
2. Block-level elements, like divs, paragraphs and headings, stack on top of each other and expand to fill their parent.
3. The browser does not apply width and height properties, or top and bottom margin settings to inline elements.
4. An inline element will only accept left/right margins and any padding value.

->Using Inline-Block to Set Width, Height, Top and Bottom Margin and Padding:
The advantage to using inline-block over inline display is that you can style inline-block elements as you would block-level elements. You can apply a width, height, and top/bottom margins and padding.

Video review:
1. The display value inline-block generates an element that's like a block element but it's also flowed with surroundings as if it were an inline element.
2. Setting an <a> element's display value to block lets you apply top and bottom padding values.

->Removing Gaps Between Inline and Inline-Block Elements:
You'll usually see default whitespace between elements when you set their display value to inline or inline-block. If you don't want the spaces in your design, there are several ways you can remove them.

Other methods for removing the default white space:
1. Setfont-size: 0; on the parent element. The space is a character space, so setting the font-size to zero makes the size of the space zero as well. But, you'll need to set the font size of the inline-block child elements back to your desired size.
2. Adding an HTML comment between the inline-block elements will also remove the space

Resources: 
1. https://www.webdesignerdepot.com/2014/07/the-secret-to-designing-website-layouts-without-css-floats/
2. https://developer.mozilla.org/en-US/docs/Web/CSS/display

Video review:
1. The browser interprets the line breaks and spaces in the HTML as content.
2. The browser adds spaces between elements displayed inline and inline-block, just like it adds spaces between words.
3. You can remove the gaps by applying a small, negative right margin to the elements.
4. The element's font-size value affects the size of the gaps between inline and inline-block elements. The larger the font size, the more you'll need to compensate with margins, so you'll need to experiment with negative margin values.

->The Column Layout Challenge:
You've learned a lot about layout and the differences between block, inline, and inline-block display. Now it's time to lay out a section of the page on your own, using CSS display settings.

Resources:
1. https://developer.mozilla.org/en-US/docs/Web/CSS/display
2. https://developer.mozilla.org/en-US/docs/Web/CSS/vertical-align

Challenge instructions:
1. Target the two columns inside the main container to display two equal-width columns.
2. Display both columns horizontally so that they appear side by side on the same line.
3. You're building the column layout using a mobile first approach, so the layout styles should apply to large screens only.

->The Column Layout Challenge Solution:
This video covers the solution to the Column Layout Challenge.

Resources:
1. https://developer.mozilla.org/en-US/docs/Web/CSS/display
2. https://developer.mozilla.org/en-US/docs/Web/CSS/vertical-align
3. https://www.webdesignerdepot.com/2014/07/the-secret-to-designing-website-layouts-without-css-floats/


>>>>>>>>>>>>>>>>>>>>>>Page Layout with the Float Property<<<<<<<<<<<<<<<<<<<
Learn how to use the float property for positioning and layout. You'll also learn about the default browser quirks you'll face when using floats and how to prevent them.

->How Floats Work?
Floats are similar to the inline-block method you learned in the previous section. You can layout elements side by side to create horizontal navigation menus and columns. The biggest difference between floats and inline-block is that floated elements are taken out of the normal document flow and content flows, or wraps, alongside them.

Resources:
1. http://alistapart.com/article/css-floats-101
2. https://developer.mozilla.org/en-US/docs/Web/CSS/float

Video review:
1. By default, browsers display elements in the order they appear in the HTML source code. This order is called the normal document flow.
2. Elements in the normal document flow are either block or inline; they appear stacked on top of each other or on the same line as the content and elements beside them.
3. When you apply a float to an element, the element gets taken out of the normal document flow and shifted to the left or right side of its container.
4. Any content next to the float flows -- or wraps -- around its left or right side.

->Wrapping Text Around Images with Floats:
One of the easiest ways to use floats is with an image. Text will wrap around an image with the float property applied to it, like in a magazine layout.

Resources:
1. https://developer.mozilla.org/en-US/docs/Web/CSS/float
2. https://www.w3.org/TR/CSS21/visuren.html#float-position

Video review:
1. The float property accepts the values left, right, and none.
2. A floated element is technically a block-level element (it accepts any width, height, padding or margins values), but it behaves like an inline element because it doesn't exist on a line of its own, and surrounding content flows around it.
3. If you’re ever curious about how your floated layout actually works, apply a dark border or background to the elements to see what’s going on behind the scenes.

->Creating a Horizontal Navigation with Floats:
Besides wrapping text around images, you can use floats to create entire web layouts. For example, you can float the links in a navigation, or content columns in a container.

Video review:
1. With floats, we don't have to worry about the the extra whitespace that can appear when using inline or inline-block display.
2. Floated elements will sit adjacent to each other regardless of the HTML whitespace between them.
3. If a block-level element contains floated elements, its height collapses.

->Clearing and Containing Floats:
The floats in the header caused a common, undesirable layout behavior you'll likely face when using floats. When you float elements, the parent container no longer honors the space of the floated elements inside it, so its height collapses.

Video review:
1. A parent container with floated elements may not always collapse to no height at all; if the container includes a padding or height value, it'll have some visible height.
2. There are a two common ways to force a collapsed element to expand to the full height of its floated child elements:
A.Setting the parent element's overflow value to hidden or auto
B.Clearing the floats with a CSS pseudo-element
3. A clearfix fixes the collapsing issue by forcing a container to expand and contain the floated elements.

Resources:
1. http://nicolasgallagher.com/micro-clearfix-hack/
2. https://developer.mozilla.org/en-US/docs/Web/CSS/clear
3. https://developer.mozilla.org/en-US/docs/Web/CSS/overflow
4. https://developer.mozilla.org/en-US/docs/Web/CSS/%3A%3Aafter
5. https://benfrain.com/easier-user-interface-and-responsive-layouts-using-css-tables/

->The Float Challenge:
You've learned a lot about CSS floats in this section of course. Now it's your turn to lay out parts of the design using floats.

Resources:
1. http://nicolasgallagher.com/micro-clearfix-hack/
2. https://developer.mozilla.org/en-US/docs/Web/CSS/float
3. https://www.w3.org/TR/CSS21/visuren.html#float-position

Video review:
1. Give each column inside the main container a fluid width.
2. The 'primary' column can be 60% wide and the 'secondary' column can be 40% -- it's up to you.
3. Use floats to display both columns horizontally so that they appear on the same line.
4. You're building the column layout using a mobile first approach, so the horizontal layout should apply to large screens only.
5. Be aware of collapsing containers caused by floats.
6. Use inline-block to lay out navigation items side by side or create a simple two-column layout
7. Use inline-block when you need control over center and vertical alignment
8. Use floats to flow content along the left or right side of an element
9. Floats do not create default horizontal white space between elements
10. Be aware of collapsing containers

>>>>>>>>>>>>>>>>>>>>>>CSS Layout Project<<<<<<<<<<<<<<<<<<<<<<<<<
Now it's time to challenge your new layout skills and put them to use by completing a CSS layout project.


->Introducing the Project:
You've done a great job learning about inline, inline-block, and floats. At this point in the course you know enough about CSS layout to build a layout on your own! Now it's time to challenge your new skills and put them to use by completing a CSS layout project.


>>>>>>>>>>>>>>>>>>>>>>>Positioning Page Content<<<<<<<<<<<<<<<<<<<<
Now that you know the basics of CSS layout, it's time to learn another important CSS layout technique. In this stage, you'll learn to position elements anywhere on the page with relative, absolute, and fixed positioning.

->How Absolute Positioning Works:
The CSS position property gives you precise control over your page layout. CSS positioning makes it easy to place elements, like a menu or an icon, anywhere on the page. This video covers a simple example of how absolute positioning works.

Resources:
1. https://developer.mozilla.org/en-US/docs/Web/CSS/position
2. http://alistapart.com/article/css-positioning-101
3. https://css-tricks.com/almanac/properties/p/position/

Positioning offsets:
1. https://developer.mozilla.org/en-US/docs/Web/CSS/top
2. https://developer.mozilla.org/en-US/docs/Web/CSS/right
3. https://developer.mozilla.org/en-US/docs/Web/CSS/bottom
4. https://developer.mozilla.org/en-US/docs/Web/CSS/left

Video review:
1. Elements with absolute positioning are neither affected by or do not affect other elements in the normal flow of the page.
2. They are like layers in Photoshop or Illustrator; you're free to place them anywhere you wish on the page.
3. Positioned elements rely on you telling the browser where to place them, using values called positioning offsets, for the element's top, right, bottom or left position.
4. When you use absolute positioning, you place the absolutely positioned elements in relation to a parent container; the parent container is the positioning context.
5. You can change the positioning context to other containing elements; this lets us position elements precisely where we want them.

->Positioning Elements Relative to Other Elements:
Absolute positioning has certain limitations by itself because the positioning is often in relation to the browser viewport. Sometimes you want to place an element in relation to another element and even have it stick with that element if it moves in the design. That's when relative positioning comes in handy.

Video review:
1. Absolute and relative positioning work hand in hand.
2. An element with relative positioning gives you the control to absolutely position elements anywhere inside it.
3. An element with absolute positioning is always relative to the first parent that has a relative position.
4. If no parent element has a relative position, the browser viewport is the positioning context by default.

->Create an Image Caption with Absolute Positioning:
Learn to use CSS positioning to place a caption and icon over the "Best City Guide" featured image.

Video review:
1. When you position elements with offset values, a negative offset value moves the element in the opposite direction.
2. Instead of moving the positioned element away from the top, right, bottom or left edges of its relative container, a negative value it moves it towards the top, right, bottom or left edges.
3. It's best to practice using different positioning offsets and relative containers to see how it affects your layout.

->Fixed Positioning:
Fixed positioning is a form of absolute positioning that positions elements in relation to the browser window instead of its containing element. In this video, you'll learn how to add a fixed navigation to your website.

Video review:
1. Unlike absolute positioning, an element with fixed positioning stays fixed to one spot on the page, regardless of the size of the browser window.
2. Fixed headers and navigation bars are common in web design. For example, the navigation bar on Twitter.
3. Fixed positioning is always relative to the browser's viewport. Like absolute positioning, you determine the fixed spot using offset values.
4. When you use relative, absolute or fixed positioning on elements, you may end up with several elements occupying the same space. This can make elements overlap or completely cover up other elements from view.

->How Z-index Works:
When you use relative, absolute or fixed positioning on elements, you may end up with several elements occupying the same space. This can make elements overlap or completely cover up other elements from view. In this video, you'll learn to use the z-index property to determine which elements display above or below other elements.

Resources:
1. https://w.trhou.se/o4yzwtxrz7
2. https://developer.mozilla.org/en-US/docs/Web/CSS/z-index
3. https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Positioning/Understanding_z_index/The_stacking_context
4. https://philipwalton.com/articles/what-no-one-told-you-about-z-index/
5. https://css-tricks.com/almanac/properties/z/z-index/

Video review:
1. Positioned elements follow a stacking order that determines which elements display above or below other elements.
2. By default, the stacking order of positioned elements is the order they appear in the source code.
3. Elements appearing later in the code sit on top on elements appearing earlier in the code.
4. The z-index property is directly related to stacking order and it's what prevents elements from overlapping other elements.
5. An element with a higher z-index value overlaps an element with a lower z-index value.
6. Positioned elements have a z-index of 0 by default.
7. z-index works only on elements with a position property set to absolute, fixed, or relative.
8. If you set a z-index on an element with no position, it will do nothing.

Stacking contexts:
When you give a positioned element a z-index, you establish a new stacking context for any descendants -- or children -- of that element. It's possible to have a higher z-index element that's underneath another element with a lower z-index. Learn more about stacking contexts here.

















