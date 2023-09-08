# Week 2 - Day 4

## The story so far...

### HTML

HTML is _essentially_ information architecture.

* "Semantic" markup means choosing elements that best represent the content being displayed.
* HTML is where you put the content and control what it _is_, CSS is how you control how it _looks_.
* HTML elements are essentially a bunch of "blocks" on a page (even if they look like other shapes!).

### CSS

CSS is the how a page should _look_, we can use it to enhance the content created by HTML.

* User Agent Stylesheets, aka "Browsers gonna browser..."
* In CSS order matters, recent rules override prior rules.
* However, Specificity can override almost everything!
* CSS Selectors read from left->right.
* The box model
  * Old and busted (ish): `content-box`
    * This is the default behavior, the box grows as you add padding + content)
  * New hotness: `border-box`
    * The width of a box doesn't change if you add padding.
    * Essentially the padding is _contained_ by the box and the content adjusts accordingly
    * This can be applied universally (the `*` selector).
* HTML elements can be displayed a few different ways:
  * Inline: Default behavior for elements (it's usually reset to "block" by browsers*).
    * Doesn't break the flow, stays inline
    * Margin and Padding can be applied
    * Height and Width are ignored
  * Inline-Block
    * Similar to inline but it respects width and height values.
  * Block: Are not inline, more like "stacked."
    * If a width isn't set, they'll take up the full width by default
  * Flex and Grid are newer display types for blocks.
    * Flex allows boxes to be "flexible," think of it almost like a liquid being poured into a container.
    * Grid puts things into a grid of rows and columns. You can assign boxes to specific areas.
* Some elements have default display types, i.e.
  * By default a `span`, or a text modifier like `strong`, are _inline_.
  * By default most images, paragraphs, headings, and `div` elements are _block_.

### Responsive Web Design/Development

* The introduction of Media Queries in CSS has made it possible to use the same code across many different device types/sizes.
* Media Queries are built in to CSS and allow us to "test" if a certain value is true, i.e. "Is this scren 640px or larger?" or "Is this screen in landscape or portrait mode?"
