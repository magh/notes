# Markdown - Lightweight Markup Language

# Applications
- markdown
- pandoc
- Retext

# Headings

    # Heading 1

    ## Heading 2

    First-level heading
    ===================

    Second-level heading
    --------------------

# Quote

> This is a quote
> How does it look on this line?

# Lists
## Basic `+ - *`
-   Red
-   Green
-   Blue

## Numbered 1,2,3
1.  Red
2.  Green
3.  Blue

## HTML list
<ol>
<li>Bird</li>
<li>McHale</li>
<li>Parish</li>
</ol>

## Numbered 1,1,1
1.  Bird
1.  McHale
1.  Parish

## Numbered 3,1,8
3. Bird
1. McHale
8. Parish

## List text indented
*   Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
    Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi,
    viverra nec, fringilla in, laoreet vitae, risus.
*   Donec sit amet nisl. Aliquam semper ipsum sit amet velit.
    Suspendisse id sem consectetuer libero luctus adipiscing.

## List text unindented
*   Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi,
viverra nec, fringilla in, laoreet vitae, risus.
*   Donec sit amet nisl. Aliquam semper ipsum sit amet velit.
Suspendisse id sem consectetuer libero luctus adipiscing.

## Escaped numbered list
1986\. What a great season.

## blockquote within a list item
the blockquote\’s \> delimiters need to be indented:

*   A list item with a blockquote:

    > This is a blockquote
    > inside a list item.

## code block within a list item
the code block needs to be indented twice — 8 spaces or two tabs:

*   A list item with a code block:

        <code goes here>

# Code Blocks

## html tag `<pre>`

<pre>
             ,-. 
    ,     ,-.   ,-. 
   / \   (   )-(   ) 
   \ |  ,.>-(   )-< 
    \|,' (   )-(   ) 
     Y ___`-'   `-' 
     |/__/   `-' 
     | 
     | 
     |    -hrr- 
  ___|_____________ 
</pre>

## Indent
Simply indent every line of the block by at least 4 spaces or 1 tab.

    This is a code block.

## Here is an example of AppleScript:

    tell application "Foo"
        beep
    end tell

## Here is an example of HTML code:
    <div class="footer">
        &copy; 2004 Foo Corporation
    </div>

## Use the `printf()` function.
Use the `printf()` function.

## ``There is a literal backtick (`) here.``
``There is a literal backtick (`) here.``

## Please don't use any `<blink>` tags.
Please don't use any `<blink>` tags.

## `&#8212;` is the decimal-encoded equivalent of `&mdash;`.
`&#8212;` is the decimal-encoded equivalent of `&mdash;`.

# Links

Markdown supports two style of links: inline and reference.

## `This is [an example](http://example.com/ "Title") inline link with a popup/title.`
This is [an example](http://example.com/ "Title") inline link with a popup/title.

## `[This link](http://example.net/) has no title attribute.`
[This link](http://example.net/) has no title attribute.

## `<http://example.com/>`
<http://example.com/>

# Images

## `![Alt text](/path/to/img.jpg)`
![Alt text](/path/to/img.jpg)

## `![Alt text](/path/to/img.jpg "Optional title")`
![Alt text](/path/to/img.jpg "Optional title")

# Emphasis

`*single asterisks*`
*single asterisks*

`_single underscores_`
_single underscores_

`**double asterisks**`
**double asterisks**

`__double underscores__`
__double underscores__

`un*frigging*believable`
un*frigging*believable

# Horizontal Rules

`* * *`

* * *

`***`

***

`*****`

*****

`- - -`

- - -

`---------------------------------------`

---------------------------------------

# Escaping

```
\   backslash  
`   backtick  
*   asterisk  
_   underscore  
{}  curly braces  
[]  square brackets  
()  parentheses  
#   hash mark  
+   plus sign  
-   minus sign (hyphen)  
.   dot  
!   exclamation mark  
```

# Paragraphs and line breaks

- `<br/>`  
- Two spaces at eol  
- Empty line  

Fin

