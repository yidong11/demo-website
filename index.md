---
---

# yidong11's Website

An engaging 1-3 sentence description of your lab.

{% include section.html %}

## Highlights

<div class="glider-container">
  <div class="glide">
    <div class="glide__track" data-glide-el="track">
      <div class="glide__slides">

        <div class="glide__slide">
          {% capture text %}
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

          {%
            include button.html
            link="research"
            text="See our publications"
            icon="fa-solid fa-arrow-right"
            flip=true
            style="bare"
          %}
          {% endcapture %}

          {%
            include feature.html
            image="images/photo.jpg"
            link="research"
            title="Our Research"
            text=text
          %}
        </div>

        <div class="glide__slide">
          {% capture text %}
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

          {%
            include button.html
            link="projects"
            text="Browse our projects"
            icon="fa-solid fa-arrow-right"
            flip=true
            style="bare"
          %}
          {% endcapture %}

          {%
            include feature.html
            image="images/photo.jpg"
            link="projects"
            title="Our Projects"
            flip=true
            style="bare"
            text=text
          %}
        </div>

        <div class="glide__slide">
          {% capture text %}
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

          {%
            include button.html
            link="team"
            text="Meet our team"
            icon="fa-solid fa-arrow-right"
            flip=true
            style="bare"
          %}
          {% endcapture %}

          {%
            include feature.html
            image="images/photo.jpg"
            link="team"
            title="Our Team"
            text=text
          %}
        </div>

      </div>
    </div>
    
    <div class="glide__arrows" data-glide-el="controls">
      <button class="glide__arrow glide__arrow--left" data-glide-dir="<">{% include icon.html icon="fa-solid fa-arrow-left" %}</button>
      <button class="glide__arrow glide__arrow--right" data-glide-dir=">">{% include icon.html icon="fa-solid fa-arrow-right" %}</button>
    </div>
  </div>
</div>

<script src="https://cdn.jsdelivr.net/npm/@glidejs/glide"></script>
<script>
  const glide = new Glide('.glide', {
    type: "carousel",
    perView: 2,
    breakpoints: {
      600: { perView: 1 },
      1200: { perView: 2 }
    },
    autoplay: 2000,
    hoverpause: true,
    focusAt: "center"
  }).mount()
</script>
