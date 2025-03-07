---
layout: post
hide: false
title: Tri 2 final add-ons
---


<h2>Additional things I did to improve (after my retrospective)</h2>

- Video of feature demo
- FRQ review
- Complete self assesment


<br>


<h3>Video Demo</h3>
<p>My feature is the recipe posting system where users can post comments from recipies from other sites. It serves similar to a social media aspect where users can read each other's posts.</p>

<video controls autoplay loop muted width="600">
    <source src="{{site.baseurl}}/images/tri2final/videodemoreal.mp4" type="video/mp4">
</video>



<h3>FRQ practice </h3>

<h5>Screenshot of CB FRQ:</h5>
<img src="{{site.baseurl}}/images/tri2final/Screenshot 2025-03-04 141327.png" alt="pic" width="500">

I'll provide code from my feature + explaination for each component of the FRQ below (scroll!):



<head>
    <title>Horizontal Scroll Section</title>
    <style>
        /* Centering wrapper */
        .horizontal-scroll-wrapper {
            width: 100%;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh; /* Centers vertically */
            overflow: hidden;
        }
        .scroll-container {
            display: flex;
            gap: 15px;
            padding: 20px;
            scroll-snap-type: x mandatory;
            width: max-content;
            overflow-x: auto;
            padding: 20px;
        }
        .section {
            flex: 0 0 70vw; /* Adjusted width */
            max-width: 600px; /* Limits section size */
            min-height: 40vh; /* Allows content to expand */
            background: white;
            border-radius: 10px;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1);
            padding: 15px;
            scroll-snap-align: start;
            text-align: center;
            word-wrap: break-word; /* Ensures text wraps properly */
        }
        .section img {
            max-width: 100%;
            height: 40vh;
            border-radius: 10px;
            object-fit: contain;
        }
        h2 {
            margin-bottom: 8px;
            font-size: 22px;
        }
        p {
            font-size: 16px;
            color: #333;
        }
    </style>
</head>
<body>
    <div class="horizontal-scroll-wrapper">
        <div class="scroll-container">
            <div class="section">
                <h2>List</h2>
                    <img src="{{site.baseurl}}/images/sprint_5/Screenshot 2025-02-04 070520.png" alt="pic" width="500">
                    <p>In model, data is retrieved in lists/rows. Each object under posting (like name, dish, cuisine, etc.) is converted into a dictionary so it can store the user's input data</p>
            </div> 
            <div class="section">
                <h2>Procedure - read</h2>
                   <img src="{{site.baseurl}}/images/sprint_5/Screenshot 2025-02-04 073034.png" alt="pic" width="500">
                    <p>This is the "update" procedure where an API endpoint updates an exisitng "posting" that's already in the db on the specific name. Then it retrieves JSON body requests, checks if the name exisits, then finds it in the db to update the rest of the information if it has been edited (dish, cuisine, link, comments). And lastly it saves the changes to display for the user.</p>
            </div>           
            <div class="section">
                <h2>Algorithm</h2>
                    <img src="{{site.baseurl}}/images/sprint_5/Screenshot 2025-02-04 073513.png" alt="pic of postman" width="500">
                    <p>1. sequencing: ordered steps. First step is when "name" is checked to see if it exists. Then, it fetches data. Last step here is to return a response in the table.</p>
                    <p>2. selection: using if else statments, the methods checks for name. If it's provided, it queries the specific post, if not, it retrieves all posts.</p>
                    <p>3. Iteration: looping of data. Line 112, retrieves all rows from table. Line 113, loops through the rows and converts them into JSON dictionaries</p>
            </div>          
            <div class="section">
                <h2>Output</h2>
                    <img src="{{site.baseurl}}/images/tri2final/Screenshot 2025-03-07 085654.png" alt="pic of frontend" width="200">
                    <img src="{{site.baseurl}}/images/tri2final/Screenshot 2025-03-07 085703.png" alt="pic of frontend" width="200">
                    <p>The input from the user is text entry, then they press a tactile button "submit recipe" which saves their data into the db. If successful, visual text pop up will output "recipe posted successfully". This same message will appear when the user edits and deletes. Edit and delete are also tactile buttons, then to edit, the user can type their changes (textual) and save them. </p>
            </div>
        </div>
    </div>

</body>







<h3>Self assesment for the retrospective</h3>
<br>

|       | points |Self Grade | Reflection |
|-------|--------|------------|-----------|
|   5 accomplishments    | .5 |   .48   |   <small>Distinct 5 accomplishments, covering multiple aspects of the class, that go in detail (db storage, postman, CPT, CRUD, Kanban). Have supporting code/ vocab/ pictures when appropriate. </small>
|   Project demo, CPT, n@tm    |  .2 |   .18   |  <small> Full stack for my feature working and deployed! Demo in person good but didn't have video of demo. CPT discussed in 5 accomplishments in detail (with vocab and code), lots of n@tm pictures and throrough reflection on the experience. </small> |     
|   Project feature blog w CPT lang   |  .1  |  .1  | <small> Complete blog starting with explaining frontend of feature, then backend. Explain success and failure and how I managed problems. Use of CPT language and supporting examples </small>      
|   MCQ    |  .1  |  .08  | <small> Complete MCQ on time, reflection on strengths + weaknesses included and also compared to last tri to see improvement in areas I used to struggle in. </small>  |
|   ability to impress    | .1  |  0.08  | <small> Reached out before the retrospective, asked someone new (my mom) for help for review, mentioned overall goals/ future plans, took extreme interest at N@tm. Added a time on my blog to practice on my own (thanks chat). Self assesment done late though...</small>  
|total| 1 | 0.90 (original) | 0.94 (updated/ after revisions) | 



