---
layout: home
title:  "Deep Q Network in Non-Deterministic Simulation 🐍"
date:   2019-08-25 06:44:31
length: ", 3 min read"
categories: blog
permalink: blog/:title
comments: true
intro: "This is a snake agent based simulation, trying to avoid the dangers of colliding into itself or the walls while trying to get the highest possible score from eating apples."
---
<div class="container">
  <div class="blog-entry">
    <div id="jumbotrone">
      <h1>{{page.title}}</h1>
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
    <p>Attacking machine learning and reinforcement learning like never before, it was decided to take on a broad and challenging project.</p>

    <p>A small project were made and built from scratch. The simplest scenario possible - a snake simulation! I wanted to use the basic principles from the classic arcade game. The goal is for the snake agent to play all by itself and make all decisions (moves) by itself to optimise the score and eat as many 🍎s as it can. Is it possible to make the snake fill the whole board? This is what I ideally want to achieve. But How?</p>

    <p>To start off, we need to properly understand how we even can build a system that learns from its own experience. We want a system that can learn from its mistakes and get rewarded from its positive actions. In other words, to train the agent to optimally play the game. This is referred to as reinforcement learning within the machine learning and AI world.</p>

    <p>To teach the agent, we need a teacher. The teacher in this case will be the environment - or game - which it is inside of!</p>

    <img src="../markov.png" alt="markov decision process" style="display: block; margin: 0 auto; max-width: 60%; border-radius: 7px;"><br>
    <div class="gh-card">
      <div class="gh-card-footer">
        <p>source: https://deepai.org/machine-learning-glossary-and-terms/markov-model</p>
      </div>
    </div>

    <p>So by now we have introduced two components. And in its simplest form that’s it! The agent and the environment! The agent is the learner and the environment is its teacher.</p>

    <p>The only thing we will do is model the game, simulation and agent with it’s neural network. The neural network will act as the snake’s brain and the network will eventually adapt and get tweaked based on the feedback the snake gets from it’s environment as rewards or penalties.</p>

    <p>There are generally three types of Artificial Intelligence. I want to emphasise first that this is neither supervised- nor unsupervised learning, which are the other two common types of AI. This system is indeed utilizing the more sophisticated reinforcement learning technique. This means that the agent not only have to train itself, but also collect data on the go. It will collect surrounding data so that it can save all action-reward pairs in a database to later mine patterns and informations which then will produce a dynamic algorithm to be tweaked during training. It really sounds magical and a bit crazy, but most of all fun! So let's build it!</p>

    <p>To do this I needed an agent to act as the snake and make the action decisions, depending on the perception.</p>

    <p>In classical AI, one of the first things we learn is the agents’ preceptors and actuators. The preceptors are the agents’ vision and sensory system, to let it perceive and collect data from the outside world and bring it internally to possibly process, memorise and train for later.</p>

    <img src="../snake_img.png" alt="snake img" style="display: block;margin: 0 auto;max-width: 55%;"><br>
    <div class="gh-card">
      <div class="gh-card-footer">
        <p>Illustration of the snake.</p>
      </div>
    </div>

    <p>The actuators on the other hand are things like its limbs or wheels, motors, speakers and other means of affecting the environment. Over time, the agent will often build a set of if-then rules from its collected data, so that it knows for instance where it is, how the environment seem to behave and what to do in the future - normally to achieve a specific task. The task is normally to change the environment’s state - the end goal. So for instance to hover all dust particles, remove all space junk or sort recycled waste.</p>

    <p>In our case though, the snake only have a very basic set of preceptors and actuators. These needs to be defined in a way that is fair and practical. The thing here is that, since our goal is to make a simulation and a snake-like agent as opposed to a human-player agent, we will try to limit the perception that the snake has over the environment or the board. If a human plays snake, the human will have vision over the whole board, but if we program it from the snake's perspective, it will basically only "see" what is in front of him and arguably to the sides. The snake obviously lives in a 2D world only seeing in 1 Dimention. Just like humans - living in 3 Dimentions - only sees in 2 dimensions. This is exactly how we will try to implement it.</p>

    <p>If you want to read the full white paper that I have published, you can do so <a class="yellow-inline-link" href="/jostein_dyrseth_dissertation_2019.pdf">here</a>.</p>

    <div class="gh-card">
      <div class="github-card" data-github="josdyr/Snake_Game" data-width="400" data-height="153" data-theme="default"></div>
      <script src="//cdn.jsdelivr.net/github-cards/latest/widget.js"></script>
      <div class="gh-card-footer">
        <p>Follow me on GitHub and  the repo to play around with it, or follow the instructions to build it from sctratch, yourself! 🤓</p>
      </div>
    </div>

    {% if page.comments %}
    <div id="disqus_thread"></div>
    <script>
    /**
    *  RECOMMENDED CONFIGURATION VARIABLES: EDIT AND UNCOMMENT THE SECTION BELOW TO INSERT DYNAMIC VALUES FROM YOUR PLATFORM OR CMS.
    *  LEARN WHY DEFINING THESE VARIABLES IS IMPORTANT: https://disqus.com/admin/universalcode/#configuration-variables*/
    /*
    var disqus_config = function () {
    this.page.url = PAGE_URL;  // Replace PAGE_URL with your page's canonical URL variable
    this.page.identifier = PAGE_IDENTIFIER; // Replace PAGE_IDENTIFIER with your page's unique identifier variable
    };
    */
    (function() { // DON'T EDIT BELOW THIS LINE
    var d = document, s = d.createElement('script');
    s.src = 'https://josdyr.disqus.com/embed.js';
    s.setAttribute('data-timestamp', +new Date());
    (d.head || d.body).appendChild(s);
    })();
    </script>
    <noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>
    {% endif %}
  </div>
</div>
