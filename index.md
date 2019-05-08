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
        }

        .text {
          font-family: "Inconsolata";
          padding: 10px;
          padding-left: 10px;
        }

        .imgbox {
            display: grid;
            height: 100%;
            padding: 10px;
            display: inline-block;
        }
        .center-fit {
            max-width: 90%;
            max-height: 90vh;
            margin: auto;
        }

        .scrolling-wrapper {
          overflow-x: scroll;
          overflow-y: hidden;
          white-space: nowrap;
        }
    </style>

</head>

<div class="text">
  <h1>matts.pics</h1>
  <p> my name is matt bettinson and i live in ontario</p>
  <a href="mailto:mattbettinson@gmail.com">hire me?</a>
</div>

<div class="scrolling-wrapper">
  {% for image in site.static_files %}
    {% if image.path contains 'images' %}
      <div class="imgbox">
        <img class="center-fit" src="{{ site.baseurl  }}{{ image.path  }}" alt="image"/>
      </div>
    {% endif %}
  {% endfor %}
<div class="scrolling-wrapper">

{:/}

