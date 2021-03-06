---
title: 'Markdown Syntax Guide'
date : 2020-05-15
tags:
- Hugo
categories:
- Skill
- Coding
thumbnailImagePosition: left
thumbnailImage: //document360.com/wp-content/uploads/2020/02/Introductory-Guide-to-Markdown-for-Documentation-Writers-01.jpg
---

This article offers a sample of basic Markdown syntax that can be used in Hugo content files, also it shows whether basic HTML elements are decorated with CSS in a Hugo theme.

<!--more-->

## Headings

To create a heading, add number signs(#) in front of a word or phrase. The
The following HTML `<h1>`—`<h6>` elements represent six levels of section headings. `<h1>` is the highest section level while `<h6>` is the lowest.

![image](https://user-images.githubusercontent.com/65668613/118364986-20378580-b59b-11eb-8272-58d91d2a36d9.png)

For compatibility, always put a ** space** between the number signs and the heading name.

## Paragraph

To create paragraphs, use a **blank line** to separate one or more lines of text.<br>
Unless the paragraph is in a list, don’t indent paragraphs with **spaces or tabs**.

### Line Break Best Practices

Fortunately, there is another option supported by nearly every Markdown application: the <br> HTML tag.

![image](https://user-images.githubusercontent.com/65668613/118365242-2bd77c00-b59c-11eb-854f-8529f3ca8704.png)

## Blockquotes

The blockquote element represents content that is quoted from another source, optionally with a citation which must be within a `footer` or `cite` element, and optionally with in-line changes such as annotations and abbreviations.

#### Blockquote without attribution
To create a blockquote, add a > in front of a paragraph.
> Tiam, ad mint andaepu dandae nostion secatur sequo quae.
> **Note** that you can use *Markdown syntax* within a blockquote.

#### Blockquote with attribution

> Don't communicate by sharing memory, share memory by communicating.<br>
> — <cite>Rob Pike[^1]</cite>

[^1]: The above quote is excerpted from Rob Pike's [talk](https://www.youtube.com/watch?v=PAAkCSZUG1c) during Gopherfest, November 18, 2015.

## List Types

You can organize items into ordered and unordered lists.

#### Ordered List

To create an ordered list, add line items with numbers followed by periods. The numbers don’t have to be in numerical order, but **the list should start with the number one**.

![image](https://user-images.githubusercontent.com/65668613/118365355-b7510d00-b59c-11eb-8c3a-3d8a4deb0fd4.png)
1. xxx
     1. df
     2. df
3. xxx
4. xxx

#### Unordered List

To create an unordered list, add dashes (-), asterisks (*), or plus signs (+) in front of line items. Indent one or more items to create a nested list.
- kjk
- kjl
- nkd

![image](https://user-images.githubusercontent.com/65668613/118365952-08fa9700-b59f-11eb-9f72-a8a253f54a78.png)

### Starting Unordered List Items With Numbers

If you need to start an unordered list item with a number followed by a period, you can use a backslash (\) to escape the period.

![image](https://user-images.githubusercontent.com/65668613/118366223-22e8a980-b5a0-11eb-8fa0-45968012c50d.png)

### Adding Elements in Lists

To add another element in a list while preserving the continuity of the list, blank a line and indent the element four spaces or one tab, as shown in the following examples.

- jdfkjdk
- dfdfdf

    djfkdjfk
- kdjfkdjf

    jdkfjdkjf
- dfdf



## Tables

Tables aren't part of the core Markdown syntax, but Hugo supports them out-of-the-box.

   Name | Age
--------|------
    Bob | 27
  Alice | 23

#### Inline Markdown within tables

| Italics   | Bold     | Code   |
| --------  | -------- | ------ |
| *italics* | **bold** | `code` |

## Code Blocks

#### Code block with backticks(code fences) and Hugo highlight shortcode
**Input:**
````
```
html{linenos=table,hl_lines=[2,"5-8",10],linenostart=1}
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
```
````
**Rendered output:**
```html{linenos=table,hl_lines=[2,"5-8",10],linenostart=1}
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
```
Options:
* `linenos`: configure line numbers. Valid values are `true`, `false`, `table`, or `inline`.`table` will give copy-and-paste friendly code blocks.
* `hl_lines`: lists a set of line numbers or line number ranges to be highlighted.
* `linenostart=199`: starts the line number count from 199.

## Other Elements — abbr, sub, sup, kbd, mark

<abbr title="Graphics Interchange Format">GIF</abbr> is a bitmap image format.

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Press <kbd><kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>Delete</kbd></kbd> to end the session.

Most <mark>salamanders</mark> are nocturnal, and hunt for insects, worms, and other small creatures.
