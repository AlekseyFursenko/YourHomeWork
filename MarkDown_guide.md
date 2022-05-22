# Marcdown Syntax
To create a heading, add number signs (#) in front of a word or phrase. The number of number signs you use should correspond to the heading level.


# Heading level 1


## Heading level 2


### Heading level 3


#### Heading level 4


Alternatively, on the line below the text, add any number of == characters for heading level 1 or -- characters for heading level 2.

Heading level 1
===============

Heading level 2
---------------

Paragraphs
---

To create paragraphs, use a blank line to separate one or more lines of text.

Don't put tabs or spaces in front of your paragraphs.

Keep lines left-aligned like this.

Line Breaks
--------

To create a line break or new line, end a line with two or more spaces, and then type return.

This is the first line.  
And this is the second line.

For compatibility, use trailing white space or the <br> HTML tag at the end of the line.

First line with the HTML tag after.<br>
And the next line.

Bold
---

To bold text, add two asterisks or underscores before and after a word or phrase. To bold the middle of a word for emphasis, add two asterisks without spaces around the letters.

I just love **bold text**.

I just love __bold text__.

Love**is**bold

Italic
---

To italicize text, add one asterisk or underscore before and after a word or phrase. To italicize the middle of a word for emphasis, add one asterisk without spaces around the letters.

Italicized text is the *cat's meow*.

Italicized text is the _cat's meow_.

A*cat*meow

Markdown applications don’t agree on how to handle underscores in the middle of a word.


### Bold and Italic

To emphasize text with bold and italics at the same time, add three asterisks or underscores before and after a word or phrase. To bold and italicize the middle of a word for emphasis, add three asterisks without spaces around the letters.

This text is ***really important***.

This text is ___really important___.

This text is __*really important*__.

This text is **_really important_**.

This is really***very***important text.


Blockquotes
---

To create a blockquote, add a > in front of a paragraph.

> Dorothy followed her through many of the beautiful rooms in her castle.

Blockquotes can contain multiple paragraphs. Add a > on the blank lines between the paragraphs.

> Dorothy followed her through many of the beautiful rooms in her castle.
>
> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

Blockquotes can be nested. Add a >> in front of the paragraph you want to nest.

> Dorothy followed her through many of the beautiful rooms in her castle.
>
>> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

Blockquotes can contain other Markdown formatted elements. Not all elements can be used

> ### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
>  *Everything* is going according to **plan**.

## Ordered Lists

To create an ordered list, add line items with numbers followed by periods. The numbers don’t have to be in numerical order, but the list should start with the number one.

1. First item
2. Second item
3. Third item
4. Fourth item

####

1. First item
8. Second item
3. Third item
5. Fourth item

####

1. First item
2. Second item
3. Third item
    1. Indented item
    2. Indented item
4. Fourth item

## Unordered Lists

To create an unordered list, add dashes (-), asterisks (*), or plus signs (+) in front of line items. Indent one or more items to create a nested list.


- First item
- Second item
- Third item
- Fourth item

- First item
- Second item
    - Intendent item
    - Intendent item
- Third item
- Fourth item

If you need to start an unordered list item with a number followed by a period, you can use a backslash (\) to escape the period.

- 1968\.  A great year!
- I think 1969 was second best.

### Adding Elements in Lists

To add another element in a list while preserving the continuity of the list, indent the element four spaces or one tab, as shown in the following examples.

* This is the first list item.
* Here's the second list item.

    I need to add another paragraph below the second list item.

* And here's the third list item.

### Blockquotes

* This is the first list item.
* Here's the second list item.

    > A blockquote would look great below the second list item.

* And here's the third list item.

## Horizontal Rules

To create a horizontal rule, use three or more asterisks (***), dashes (---), or underscores (___) on a line by themselves.

***

---

_________________

## Strikethrough

~~This was mistaken text~~

## Subscript

<sub>This is a subscript text</sub>

## Superscript

<sup>This is a superscript text</sup>

## Quoting code

Use `git status` to list all new or modified files that haven't yet been committed.

To format code or text into its own distinct block, use triple backticks.

Some basic Git commands are:
```
git status
git add
git commit
```


