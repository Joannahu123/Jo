---
layout: base
title: Student Home 
description: Home Page
hide: true
---


<!--<head>
  <style>
    .grid-container {
      display: grid;
      grid-template-columns: repeat(3, 1fr); /* make 3 columns */
      gap: 15px; /* put gap between grid items */
      justify-content: center; /*center grid horizontally*/
      text-align: center; /* center text & images */
    }
    .grid-item img {
      width: 100%; /* Make image full width */
      height: auto; /* keep aspect ratio */
    }
    p {text-align: center;}
    .column {
    float: right;
    width: 100%;
    padding: 2px;
    }
    .row {
    display: flex;
    }
    .grid-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(150px, 1fr)); /* Dynamic columns */
            gap: 10px;
        }
        .grid-item {
            text-align: center;
        }
        .grid-item img {
            width: 100%;
            height: 200px;
            max-height: 200px;
            object-fit: contain; /* make image fit with fixed height */
        }
        .grid-item p {
            margin: 5px 0;
        }
        .center {
            display: block;
            margin-left: 0 auto;
            margin-right: auto;
            width: 50%;
}
  </style>
</head>-->


<head>
  <style>
    /* Grid container: Dynamic columns, centered horizontally */
    .grid-container {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(150px, 1fr)); /* Dynamic number of columns */
      gap: 15px; /* Space between grid items */
      justify-content: center; /* Center grid horizontally */
      max-width: 500px; /* Limit grid width */
      margin: 0 auto; /* Center the entire grid container */
      text-align: center; /* Center text inside the grid */
    }
    /* Grid item: Style for individual items */
    .grid-item {
      text-align: center; /* Ensure content is centered inside each grid item */
    }
    /* Image: Ensure images are contained within their grid item */
    .grid-item img {
      width: 100%; /* Make images fully responsive */
      height: auto; /* Maintain aspect ratio */
      max-height: 200px; /* Limit image height */
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
      width: 50%; /* You can adjust this to change how centered elements appear */
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
            <a href="https://www.youtube.com/watch?v=HMTKMWHLbdQ&ab_channel=Crunchycat" target="blank">
                <img src="images/catonly.png" alt="crunch crunch"> 
            </a>
            <p>Crunch along</p>
        </div>
        <div class="grid-item">
            <a href="https://www.youtube.com/watch?v=Gnm3hIcjiCQ&ab_channel=Michi" target="blank">
                <img src="images/catonly.png" alt="happi dance">
            </a>
            <p>Dance along</p>
        </div>
        <div class="grid-item">
            <a href="https://www.youtube.com/watch?v=_fvNuap9l-Y&ab_channel=JamirJessR" target="blank">
                <img src="images/catonly.png" alt="cat cam">
            </a>
            <p>Eat along</p>
        </div>
    <br>
    <br>

</div>
<br>
<br>
<div style="text-align: center;">
    <img src="images/cute_cat.jpg" alt="silly cat with a hat is sad you can't see it" width="600" height="350">
</div>
</body>
