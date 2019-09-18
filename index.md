---
layout: default
home: true
color: gray
---

{%- capture expert_content -%}

### Was ich für Sie tun kann?

Zuverlässiges und aktuelles Know-how rund um Amerikanische Chiropraktik und Nutrition Concepts zeichnen mich aus. Hier bin ich Experte. In meiner Praxis biete ich seit 1991 Amerikanische Chiropraktik und Nutrition Concepts an, denn Nervensystem und Verdauung hängen unmittelbar voneinander ab. Funktioniert beides im Einklang miteinander, können wir rundherum gesund sein.

{% endcapture %}
{%- include expert_box.html content=expert_content -%}

{% capture kontakt %}

#### Kontakt

Thomas Grossmann  
Hallerplatz 4  
20146 Hamburg  
Telefon: [+49 (0) 40 85 37 33 95](tel:00494085373395)  
E-Mail: [info@institut-grossmann.com](mailto:info@institut-grossmann.com)

{% endcapture %}
{% capture oeffnungszeiten %}

#### Öffnungszeiten

| Montag	   | 09:00–13:00 <br /> 15:00–18:00 |
| Dienstag	 | 15:00–19:00                 |
| Mittwoch	 | 08:00–13:00|
| Donnerstag | 15:00–19:00|
| Freitag	   | 08:00–13:00|

{% endcapture %}
{% include columns.html col1=kontakt col2=oeffnungszeiten %}

{% capture tile_cols_1 %}
{% include tile.html
  image="assets/images/banner.jpg"
  title="Amerik. Chiropraktik"
  href="./amerikanische-chiropraktik"
  text="„Ziel der Amerikanischen Chiropraktik ist es, diese Blockaden zu lösen und auf diese Weise die Selbstheilungskräfte des Menschen zu aktivieren.“"
%}
{% endcapture %}
{% capture tile_cols_2 %}
{% include tile.html
  image="/assets/images/empfang.png"
  title="Nutrition Concepts"
  href="./nutrition-concepts"
  text="„Wichtig ist, was Sie brauchen – <br />was Ihr Darm und Ihr Körper benötigen –, damit Sie Ihr Leben voller Energie leben können.“"
%}
{% endcapture %}
{% include columns.html noSpace=true col1=tile_cols_1 col2=tile_cols_2 %}
