---
layout: home
title:  "C# Checkers Game"
date:   2019-04-20 21:09:45 +0100
categories: blog
permalink: blog/:title
intro: "C# Checkers Game."
---
<!DOCTYPE html>
<html lang="en-us">
  <head>
    <meta charset="utf-8">
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
    <title>Unity WebGL Player | Checkers</title>
    <link rel="shortcut icon" href="../Checkers_WebGL/TemplateData/favicon.ico">
    <link rel="stylesheet" href="../Checkers_WebGL/TemplateData/style.css">
    <script src="../Checkers_WebGL/TemplateData/UnityProgress.js"></script>
    <script src="../Checkers_WebGL/Build/UnityLoader.js"></script>
    <script>
      var unityInstance = UnityLoader.instantiate("unityContainer", "../Checkers_WebGL/Build/Checkers_WebGL.json", {onProgress: UnityProgress});
    </script>
  </head>
  <body>
    <div class="webgl-content">
      <div id="unityContainer" style="width: 960px; height: 600px"></div>
      <div class="footer">
        <div class="webgl-logo"></div>
        <div class="fullscreen" onclick="unityInstance.SetFullscreen(1)"></div>
        <div class="title">Checkers</div>
      </div>
    </div>
  </body>
</html>
