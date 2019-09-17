---
layout: default
---

# An h1 header

Paragraphs are separated by a blank line.

2nd paragraph. _Italic_, **bold**, and `monospace`. Itemized lists
look like:

{% capture expert_content %}

### Was ich für Sie tun kann?

Zuverlässiges und aktuelles Know-how rund um Amerikanische Chiropraktik und Nutrition Concepts zeichnen mich aus. Hier bin ich Experte. In meiner Praxis biete ich seit 1991 Amerikanische Chiropraktik und Nutrition Concepts an, denn Nervensystem und Verdauung hängen unmittelbar voneinander ab. Funktioniert beides im Einklang miteinander, können wir rundherum gesund sein.

{% endcapture %}
{%- include expert_box.html content=expert_content -%}

- this one
- that one
- the other one

Note that --- not considering the asterisk --- the actual text
content starts at 4-columns in.

> Block quotes are
> written like so.
>
> They can span multiple paragraphs,
> if you like.

Use 3 dashes for an em-dash. Use 2 dashes for ranges (ex., "it's all
in chapters 12--14"). Three dots ... will be converted to an ellipsis.
Unicode is supported. ☺

there are also buttons

{% include button.html cta="Click me" href="#" %}

## An h2 header

Here are some columns:

{% capture colexample1_col1 %}

#### Column Headline

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

{% endcapture %}
{% capture colexample1_col2 %}

#### Column Headline

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

{% endcapture %}
{% include columns.html mobile2=true col1=colexample1_col1 col2=colexample1_col2 %}

Three Columns:  

{% include columns.html col1=colexample1_col1 col2=colexample1_col2 col3=colexample1_col2 %}

Four Columns:

{% include columns.html mobile2=true col1=colexample1_col1 col2=colexample1_col2 col3=colexample1_col2 col4=colexample1_col2 %}

Columns can also contain tiles

{% capture tile_cols_1 %}
{% include tile.html
  image="assets/images/banner.jpg"
  title="Amerik. Chiropraktik"
  href="./amerikanische-chiropraktik"
  text="Das bewährte Behandlungskonzept basiert auf einem der zentralsten Organe: dem Nervensystem."
%}
{% endcapture %}
{% include columns.html noSpace=true col1=tile_cols_1 col2=tile_cols_1 %}


Here are text columns

{% capture text_cols_content %}

Here's a numbered list:

1.  first item
2.  second item
3.  third item

Note again how the actual text starts at 4 columns in (4 characters
from the left side). Here's a code sample:

    # Let me re-iterate ...
    for i in 1 .. 10 { do-something(i) }

As you probably guessed, indented 4 spaces. By the way, instead of
indenting the block, you can use delimited blocks, if you like:

```python
import time
# Quick, count to ten!
for i in range(10):
    # (but not *too* quick)
    time.sleep(0.5)
    print(i)
```

(which makes copying & pasting easier). You can optionally mark the
delimited block for Pandoc to syntax highlight it:

{% endcapture %}
{% include text_columns.html content=text_cols_content %}

### An h3 header

#### h4 header

##### h5 header

###### and h6 header

Now a nested list:

1.  First, get these ingredients:

    - carrots
    - celery
    - lentils

2.  Boil some water.

3.  Dump everything in the pot and follow
    this algorithm:

        find wooden spoon
        uncover pot
        stir
        cover pot
        balance wooden spoon precariously on pot handle
        wait 10 minutes
        goto first step (or shut off burner when done)

    Do not bump wooden spoon or it will fall.

Notice again how text always lines up on 4-space indents (including
that last line which continues item 3 above).

Here's a link to [a website](http://foo.bar), to [google](http://google.com), to a [local
doc](local-doc.html), and to a [section heading in the current
doc](#an-h2-header). Here's a footnote [^1].

[^1]: Some footnote text.

Tables can look like this:

| Name         | Size | Material    | Color       |
| ------------ | ---- | ----------- | ----------- |
| All Business | 9    | leather     | brown       |
| Roundabout   | 10   | hemp canvas | natural     |
| Cinderella   | 11   | glass       | transparent |

---

and images can be specified like so:

![example image](https://placekitten.com/300/300 'An exemplary image')

And note that you can backslash-escape any punctuation characters
which you wish to be displayed literally, ex.: \`foo\`, \*bar\*, etc.
