---
layout: home
title:  "Design Principles"
date:   2019-04-20 21:09:45 +0100
categories: blog
permalink: blog/:title
intro: "This is an intro to Design Patterns."
published: false
---
<div class="container">
  <h1>{{page.title }}<br></h1>
  <p><i>{{page.date | date_to_long_string}}<br></i></p>
  <p>Definition: A design pattern is the re-usable form of a solution to a design problem. The idea was introduced by the architect Christopher Alexander[1] and has been adapted for various other disciplines, notably software engineering.</p>

  <h3>The DRY Pattern</h3>
  <p>This pattern or principle sais in short to simply never let a software have redundant code or repeting instructions. If this is the case - which is fine under development - however before deployment this should be strongly avoided and refactored. Changing the repetitive code into a generic function rather. Remeber, all functions you write can always be used again at a later point from different systems.</p>

  <p>This articles is coming.</p>

</div>
