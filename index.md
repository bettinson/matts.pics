---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

---


{::nomarkdown}
<head>
    <style>
        * {
            margin: 0;
            padding: 0;
            font-family: "Inconsolata";
        }
        .imgbox {
            display: grid;
            height: 100%;
            padding: 10px;
        }
        .center-fit {
            max-width: 100%;
            max-height: 100vh;
            margin: auto;
        }
    </style>

</head>

<h1>matts.pics</h1>

{% for image in site.static_files %}
  {% if image.path contains 'images' %}
    <div class="imgbox">
      <img class="center-fit" src="{{ site.baseurl  }}{{ image.path  }}" alt="image"/>
    </div>
  {% endif %}
{% endfor %}
{:/}
