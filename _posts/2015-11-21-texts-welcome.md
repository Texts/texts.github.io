---
title: "Welcome to Texts!"
---

Texts is “rich editor for plain text”—you can write documents in visual
interface and they will be saved in plain text format with Markdown markup. This
document shows some styles available in Texts. Please feel free to edit it—a
fresh copy is always available via Help menu.

Inline Formatting
-----------------

To apply *emphasis* or **strong emphasis** press ⌘I or ⌘B and type. Press again
to turn it off.

Footnotes
---------

Notes can be placed anywhere[^1] in the source file (press ⌘R to insert one).
When document is published to paper-oriented format (PDF or Word) footnotes are
displayed at the bottom of the corresponding page. E-book readers usually
display notes in popups.

[^1]: Yes, right here.

Hyperlinks
----------

Press ⌘K to insert a hyperlink. It can be either literal URL (e.g.
<http://www.google.com/>) or have some [text](<http://www.texts.io/>). Click URL
with ⌘ key pressed to open it in web browser.

Images
------

![](<../images/radcliffe-camera.jpg>)

Math
----

Formulas can be placed inline like $$E=mc^2$$ or in a separate paragraph, like
the following one. Standard LaTeX syntax is supported.

$$
\frac{n!}{k!(n-k)!} = \binom{n}{k}
$$

Code
----

Inline `code` gets monospaced font.

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ ruby
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Press “Enter” key inside code block to insert a line break or “Shift+Enter” to
end code block.

Lists
-----

-   First bulleted item.

-   Second bulleted item.

Lists can be styled via menu, keyboard shortcut, or using autoformatting: type
minus and space for bulleted item or “1”, point and space for numbered item.
Press “Tab” to indent paragraph and create subitem, “Shift+Tab” to unindent.

1.  First numbered item.

2.  Second numbered item.

Tables
------

Press **\^⌘L** to create a table, ⌥⌘+arrow keys to add more columns or rows,
\^⌘+arrow keys to move column or row. Here is a sample table.

| **Features** | **Editable in Texts** | **Export to PDF** | **Export to HTML** |
|--------------|-----------------------|-------------------|--------------------|
| Basic Styles | ✓                     | ✓                 | ✓                  |
| Footnotes    | ✓                     | ✓                 | ✓                  |
| Images       | ✓                     | ✓                 | ✓                  |
| Tables       | ✓                     | ✓                 | ✓                  |

Happy writing!
==============

Got a question? Visit <http://www.texts.io/support/>.
