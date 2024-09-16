---
layout: base
title: Student Home 
description: Home Page
hide: true
---

{% include nav_Jo.html %}
<br>

<head>
  <style>
    .grid-container {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(150px, 1fr)); /* Dynamic number of columns */
      gap: 15px;
      justify-content: center; /* Center horizontally */
      max-width: 500px;
      margin: 0 auto; /* Center entire grid */
      text-align: center;
    }
    .grid-item {
      text-align: center;
    }
    /* Image: Ensure images are contained within their grid item */
    .grid-item img {
      width: 100%; /* Make images fully responsive */
      height: auto; /* Maintain aspect ratio */
      max-height: 200px;
      object-fit: contain; /* Fit images inside the container */
    }
    /* Paragraph styling for grid items */
    .grid-item p {
      margin: 5px 0; /* Space around paragraphs */
    }
    /* Centered block elements */
    .center {
      display: block;
      margin: 0 auto;
      width: 50%;
    }
  </style>
</head>


<body>
    <div style="text-align: center;">
    <h4>⋆ ⭒ ˚ . ⋆  ⋆ ⭒ ⋆🪐˚ . ⋆⋆ ⭒ ˚ .  ⋆ ⭒ ˚ . ⋆⋆ ⋆🪐⭒ ˚ . ⋆⋆ ⭒ ˚ . ⋆. ⋆ ⋆ ⭒⋆ ˚ . ⋆ ⭒ ˚ .  </h4>
    <h1 style="color:dark blue;"> Joanna's page!</h1>
    <h4>˚. ୭ ˚ ○ ◦ ˚.˚ ◦ ○˚ ୧ .˚ₓ ˚. ୭ ˚ ○ ◦ ˚.˚ ◦ ○˚ ୧ .˚ₓ˚. ୭ ˚ ○ ◦ ˚.˚ ◦ ○˚ ୧ .˚ₓ</h4>
    </div>
    <div class="grid-container" id="grid_container">
    </div>
    <div class="grid-container">
        <div class="grid-item">
            <a href="https://www.youtube.com/watch?v=HMTKMWHLbdQ&ab_channel=Crunchycat" target="blank"><p title = "click me">
                <img src="images/catonly.png" alt="crunch crunch"> 
            </p></a>
            <p>Crunch along</p>
        </div>
        <div class="grid-item">
            <a href="https://www.youtube.com/watch?v=Gnm3hIcjiCQ&ab_channel=Michi" target="blank"><p title = "click me too">
                <img src="images/catonly.png" alt="happi dance">
            </p></a>
            <p>Dance along</p>
        </div>
        <div class="grid-item">
            <a href="https://www.youtube.com/watch?v=_fvNuap9l-Y&ab_channel=JamirJessR" target="blank"><p title = "click me three">
                <img src="images/catonly.png" alt="cat cam">
            </p></a>
            <p>Eat along</p>
        </div>
    <br>
    <br>

</div>
<br>
<br>
<div style="text-align: center;">
    <p title = "you can't click me haha"><img src="images/cute_cat.jpg" alt="silly cat with a hat is sad you can't see it" width="600" height="350"></p>
</div>
</body>
