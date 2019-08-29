---
layout: home
title:  "Redlab CMS"
date:   2019-07-10 06:44:31
categories: blog
permalink: blog/:title
intro: "Redlab is a community for IoT enthusiasts. This was developed as a content management system with admin and user features."
published: true
---
<div class="container">
  <div class="blog-entry">
    <div id="jumbotrone-two">
      <h1>{{ page.title }}</h1>
      <div class="blog-metadata">
        <div class="portrait">
          <img id="min-portrait" src="../IMG_0657_5.png" alt="">
        </div>
        <div class="blog-metadata-text">
          <i>by Jostein Dyrseth</i><br>
          <i>{{page.date | date_to_long_string}}</i>
          <i>{{ page.length }}</i>
        </div>
      </div>
    </div>

    <p>Check out the actual site in a new tab here: <a class="yellow-inline-link" target="_blank" href="http://redlab-dev.napier.ac.uk">here</a><p>
    <img src="../redlab_demo.png" width="100%" style="border-radius: 8px;">

    <p>Redlab is a community for IoT enthusiasts. The site was made to let anyone create an account to login at any time, upload their own projects as blog articles or tutorials with steps, or just to learn more from others' posts.</p>

    <p>Any user can create their own blog articles. They can also like, comment and follow the articles themselves.</p>

    <p>The site uses the Django CMS Framework and stores the data about the users and all uploaded articles in a PostrgreSQL database. The content is readable by everyone as long as the Root User wishes so. The Root User has access to everything, however Django let's you create user-groups too. This makes it easy to give different user-groups different responsibilities that matches their role in for instance maintaining the site. Some users can remove comments or delete other users that don't follow the site's policy.</p>
  </div>
</div>
