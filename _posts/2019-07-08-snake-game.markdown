---
layout: home
title:  "Deep Q Network in Non-Deterministic Simulation"
date:   2019-07-08 06:44:31
categories: blog
permalink: blog/:title
intro: "This is a snake agent based simulation, trying to avoid the dangers of colliding into itself or the walls while trying to get the highest possible score from eating apples."
---
<div class="centered-content">
  <h1>{{page.title }}</h1>
  <div class="blog-metadata">
    <div class="portrait">
      <img id="min-portrait" src="../IMG_1193.png" alt="">
    </div>
    <div class="blog-metadata-text">
      <i>by Jostein Dyrseth</i><br>
      <i>{{page.date | date_to_long_string}}</i><br>
    </div>
  </div>
  <br>
  <div class="text-content">
    This is a snake agent based simulation, trying to avoid the dangers of colliding into itself or the walls while trying to get the highest possible score from eating apples.<br><br>

    Attaking machine learning and reinforcement learning like never before, I decided to take on a broad and challenging project into my own hands.<br><br>

    I decided that I wanted to try to start small and build from there, so I came up with the simplest scenario possible - a snake game. I this classic archade game play all by itself and make the highest score possible. To do this I needed an agent to act as the snake and make the action decisions, depending on the perception.<br><br>

    In classical AI, one of the first things we learn is the agents’ preceptors and actuators. The preceptors are the agents’ vision and sensory system, to let it perceive and collect data from the outside world and bring it internally to possibly process, memorise and train for later.<br><br>

    <img src="../snake_img.png" alt="snake img" style="display: block;margin: 0 auto;max-width: 55%;"><br><br>

    The actuators on the other hand are things like its limbs or wheels, motors, speakers and other means of affecting the environment. Over time, the agent will often build a set of if-then rules from its collected data, so that it knows for instance where it is, how the environment seem to behave and what to do in the future - normally to achieve a specific task. The task is normally to change the environment’s state - the end goal. So for instance to hover all dust particles, remove all space junk or sort recycled waste.<br><br>
  </div>
  <br>
</div>
