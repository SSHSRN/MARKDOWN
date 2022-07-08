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

[github]: www.github.com
[google]: www.google.com

Reference links don't appear in the rendered Markdown. <br>
You define them by providing the same tag name wrapped in brackets, followed by a colon, followed by the link.


