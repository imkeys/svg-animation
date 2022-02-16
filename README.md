```css

.rect {
  position: absolute;
  top: 0;
  left: 0;
  width: 10px;
  height: 10px;
  background: darkred;
  /* -- */
  offset-path: path("M10 180 C 40 10, 65 10, 95 180 S 150 150, 280 80");
  offset-distance: 0%;
  animation: svg-path-animation 3s ease-in-out 0s infinite normal;
}

@keyframes svg-path-animation {
  from {
    offset-distance: 0%;
  }

  to {
    offset-distance: 100%;
  }
}


```


```html

<svg width="300" height="300">
  <path d="M10 180 C 40 10, 65 10, 95 180 S 150 150, 280 80" />
</svg>
<div class="rect"></div>

```