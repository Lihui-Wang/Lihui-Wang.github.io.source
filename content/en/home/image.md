---
# An instance of the Blank widget.
# Documentation: https://wowchemy.com/docs/page-builder/

# https://wowchemy.com/docs/content/writing-markdown-latex/#figures
widget: blank

# Activate this widget? true/false
active: false

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 25

title:
# Gallery
subtitle:

design:
  columns: "1"
  background:
    # image: coders.jpg
    image_darken: 0
    image_parallax: false
    image_position: center
    image_size: cover
    # text_color_light: true
  spacing:
    padding: ["20px", "0", "20px", "0"]
advanced:
  # css_class: fullscreen

gallery_item:
  - album: gallery
    image: test1.jpg
    caption: Write your image 1 caption here
  - album: gallery
    image: test2.jpg
    caption: Write your image 2 caption here
---
{{< gallery album="gallery" >}}
