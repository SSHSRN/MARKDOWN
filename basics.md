# Markdown

Hello World!
This document contains the basics of writing a markdown file (md).

## Bold and Italic

_This text is italic._
<!-- Note that empty lines doesn't matter (do not affect the preview) in markdown. -->


**This text is bold.**

**_This text is bold and italic!_**

## Headers

# This is Header one
## This is Header two
### This is Header three
#### This is Header four
##### This is Header five
###### This is Header six
<!-- In general, headers one and six should be used sparingly. -->

## Links

There are two different link types in Markdown, but both of them render the exact same way. <br>
The first link style is called an inline link. <br>
To create an inline link, you wrap the link text in brackets ( [ ] ), and then you wrap the link in parenthesis ( ( ) ). <br>
For example, to create a hyperlink to www.github.com, with a link text that says, Visit GitHub!, you'd write this in Markdown: <br>
[Visit GitHub!](www.github.com).

[Click here to _**google**_](www.google.com)

Headings can also have links

For example,

#### [This is a link to the top](#Markdown)

The other link type is called a reference link. <br>
As the name implies, the link is actually a reference to another place in the document. <br>

Here's [a link to github][github].<br>
Here's [yet another link][google].

[github]: https://www.github.com
[google]: https://www.google.com

Reference links don't appear in the rendered Markdown. <br>
You define them by providing the same tag name wrapped in brackets, followed by a colon, followed by the link.

## Images

The syntax for creating links and images is nearly the same.<br>
Images also have two styles, just like links, and both of them render the exact same way. <br>
The difference between links and images is that images are prefaced with an exclamation point ( ! ).

The first image style is called an inline image link.<br>
To create an inline image link, enter an exclamation point ( ! ), wrap the alt text in brackets ( [ ] ), and then wrap the link in parenthesis ( ( ) ). (Alt text is a phrase or sentence that describes the image when the image is not loaded.)

![Github Cat](https://octodex.github.com/images/Fintechtocat.png)

<!-- The below image url is invalid, so the alt(alternative) text is displayed -->
![Github Cat](https://octodex.github.com/images/Fintechtocat123.png)
<br>
For a reference image, the pattern is same as a reference link.<br>
Precede the Markdown with an exclamation point, then provide two brackets for the alt text, and then two more for the image tag, like this: ![The master][yoga] At the bottom of your Markdown page, you'll define an image for the tag, like this: [yoga]: https://octodex.github.com/images/yogitocat.png.<br>

![The master][yoga]

[yoga]: https://octodex.github.com/images/yogitocat.png