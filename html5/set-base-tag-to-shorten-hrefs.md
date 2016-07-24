# Set the `<base>` tag to shorten `href` values (carefully)

Within the `<head>` tag in your HTML document, you can set a base url for all subsequent `href` attributes.

## It looks like this

In your `<head>` tag:

`<base href="http://exampleurl.com/topics/language/">`

All further links can be simplified like so:

`<a href="french">` becomes `<a href="http://exampleurl.com/topics/language/french">`
`<a href="spanish">` becomes `<a href="http://exampleurl.com/topics/language/spanish">`

## Be careful

It's best to think of the `<base>` element as *entirely replacing* the default URL. This can lead to unexpected behavior when using `#` anchors or `?` queries on the `<base>` tag's `href`— since it always ends with a slash by default.

[Read more](https://stackoverflow.com/questions/1889076/is-it-recommended-to-use-the-base-html-tag) at this StackOverflow thread.
