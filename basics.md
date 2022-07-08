# Markdown

Hello World!
This document contains the basics of writing a markdown file (md).

### Why MarkDown?  
Markdown is a fast and easy way to take notes, create content for a website, and produce print-ready documents.  
It doesn’t take long to learn the Markdown syntax, and once you know how to use it, you can write using Markdown just about everywhere. Most people use Markdown to create content for the web, but Markdown is good for formatting everything from email messages to grocery lists.

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
Precede the Markdown with an exclamation point, then provide two brackets for the alt text, and then two more for the image tag, like this: ![The master][yogaCat] At the bottom of your Markdown page, you'll define an image for the tag, like this: [yoga]: https://octodex.github.com/images/yogitocat.png.<br>

![The master][yoga]

[yoga]: https://octodex.github.com/images/yogitocat.png

## BlockQuotes

A blockquote is a sentence or paragraph that's been specially formatted to draw attention to the reader. 

To create a block quote, preface a line with the "greater than" caret (>).

>This is a BlockQuote!

Block quotes can contain other Markdown elements, such as italics, images, or links.

>This is a BlockQuote having link to [google](https://www.google.com)!

## Lists

There are two types of lists: unordered and ordered. <br>
To create an unordered list, preface each item in the list with an asterisk ( * ). <br>
Each list item also gets its own line.

* List-item1
* List-item2
* List-item3
* List-item4
* List-item5

An ordered list is prefaced with numbers, instead of asterisks.

1. List-item1
2. List-item2
3. List-item3
4. List-item4
5. List-item5

To nest one list within another, the Markdown syntax is exactly the same. Just indent each asterisk one space more than the preceding item.

* Animals
    * Herbivores
        * Deer
        * Elephant
    * Carnivores
        * Lion
        * Tiger

## Task Lists

To create a task list, preface list items with a hyphen and space followed by [ ].  
To mark a task as complete, use [x].  
- [ ] Task A  
- [x] Task B

## Paragraphs

Markdown has several ways of formatting paragraphs.

Using an empty line in between two lines to create a linebreak in the rendered markdown is called _hard break_.

Using two spaces at the end if a line to create a linebreak in the rendered markdown is called _soft break_.

## Emojis

Emojis can be added to by typing :EMOJICODE:  

@sshsrn Good work :+1: 

## Footnotes

Footnotes can be added to the content by using this bracket syntax:

This is a simple footnote[^1].

A footnote can also have multiple lines[^2].  

You can also use words, to fit your writing style more closely[^note].
<!-- The below three lines will be at the bottom of the document. -->
[^1]: simple footnote.
[^2]: Every new line should be prefixed with 2 spaces.  
  This allows you to have a footnote with multiple lines.
[^note]:
    Named footnotes will still render with numbers instead of the text but allow easier identification and linking.  
    This footnote also has been made with a different syntax using 4 spaces for new lines.

## Ignore Markdown formatting

Markdown formatting can be ignored by using \ before the Markdown character.

Let's rename \*our-new-project\* to \*our-old-project\*.

## Tables

Tables are used for organising the data in rows and columns.  

| Column1 | Column2 |
| --- | --- |
| Row1-Column1 | Row1-Column2 |
| Row2-Column1 | Row2-Column2 |

The pipes on either end of the table are optional.

There must be at least three hyphens in each column of the header row.

### Formatting in table

Formattings like links, inline code blocks, and text styling can be used within a table.

| Command | Description |
| --- | --- |
| `print("Hello world")` | Python code to *print Hello world*  |

Text alignmments can also be done.

| Left-aligned | Center-aligned | Right-aligned |
| :---         |     :---:      |          ---: |
| left   | center     | right    |

## Collapsed sections

Any Markdown within the \<details> block will be collapsed until the reader clicks > to expand the details. Within the \<details> block, use the \<summary> tag to create a label to the right of >.

<details><summary>Do not Click</summary>
<p>

#### I did warn you!

```python
print("You shouldn't have clicked it.")
```

```python
    print("You should now face the consequences.")
```

</p>
</details>

## Diagrams

Markdown can also be used to create diagrams to convey information through charts and graphs.  

Mermaid is a Markdown-inspired tool that renders text into diagrams.  
For example, Mermaid can render flow charts, sequence diagrams, pie charts and more. 

Mermaid documentation => https://mermaid-js.github.io/mermaid/#/

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```