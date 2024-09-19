---
layout: page
title: About
permalink: /about/
---

<script>
{% include nav_Jo.html %}
</script>

{% include nav_Jo.html %}



<br>

<h2>My timeline:</h2>


<head>
<style>
/* Container for the horizontal timeline */
.horizontal-timeline {
    display: flex;
    overflow-x:auto;
    padding: 20px;
    white-space: normal;
    background: #2A447F;
    border: 1px #1D1D76;
}
/*the individual items*/
.timeline-item {
    flex: 0 0 auto; /* Prevent items from shrinking or growing */
    width: 350px;
    height: 400px;
    margin-right: 20px;
    background: #C7D8FF;
    border: 2px solid #211051;
    border-radius: 15px;
    padding: 20px;
    box-shadow: 0 0 15px rgba(48,27,107,1);
    box-sizing: border-box; /* prevent expanding past set padding */
    overflow-y: auto;
}
/* Ensure content fits within items */
.timeline-content {
    max-height: 100%;
    overflow-y: auto;
    overflow-x: hidden;
    overflow-wrap: break-word;
}
.timeline-content img {
    max-width: 100%;
    height: auto;
    display: block;
    margin-top: 10px;
}
.timeline-content p {
    margin-bottom: 0;
}
</style>
</head>


<body>
<div class="horizontal-timeline">
    <div class="timeline-item">
        <div class="timeline-content">
            <h2>2007-2009</h2>
            <p>Born in Pennsylvania </p>
            <ul>
                <li>I don't remember anyting from this time</li>
                <li>But I was a really cute baby</li>
            </ul>
            <img src="{{site.baseurl}}/images/baby.png" alt="CA gurl">
            <img src="{{site.baseurl}}/images/wholefamily.png" alt="CA gurl">
        </div>
    </div>
    <div class="timeline-item">
        <div class="timeline-content">
            <h2>2009-2019</h2>
            <p>Lived in Ohio:</p>
            <ul>
                <li>2012: started swimming with the Mason Manta Rays</li>
                <li>Also learned ice skating, tennis, soccer, art, piano, and flute, but stopped these activities after moving to SD</li>
                <li>Went to elementary and Intermediate school</li>
                <li>Favorite place: Kings Island Amusement Park</li>
            </ul>
           <img src="{{site.baseurl}}/images/masonview.png" alt="CA gurl">
           <img src="{{site.baseurl}}/images/snowbear.png" alt="CA gurl">
        </div>
    </div>
    <div class="timeline-item">
        <div class="timeline-content">
            <h2>2019-2024</h2>
            <p>San Diego</p>
            <ul>
                <li>Attend(ed) middle and high school </li>
                <li>Continued swimming at a new club called SDAC</li>
                <li>Learned crochet and made a small business</li>
            </ul>
            <img src="{{site.baseurl}}/images/casunset.png" alt="CA gurl">
            <img src="{{site.baseurl}}/images/At_school.png" alt="CA gurl">
        </div>
    </div>
</div>
</body>

<br>
<br>
<br>



<div style="text-align: center;">
    <img src="{{site.baseurl}}/images/1180w-600h_a-to-z-dumbo.jpg" alt="endless love for dumbo" width="600" height="350">
    <br>
    <h4>Dumbo is my childhood and comfort character</h4>
</div>

<!--utterances-->
<script src="https://utteranc.es/client.js"
        repo="joannahu123/Jo"
        issue-term="pathname"
        theme="github-light"
        crossorigin="anonymous"
        async>
</script>
