---
layout: home
title:  "C# Tower Defence"
date:   2019-08-23 21:09:45 +0100
categories: blog
permalink: blog/:title
intro: "C# Tower Defence."
---
<!DOCTYPE html>
<html lang="en-us">
  <head>
    <meta charset="utf-8">
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
    <title>Unity WebGL Player | Tower_Defence_Tutorial</title>
    <link rel="shortcut icon" href="..//Tower_Defence_Tutorial/TemplateData/favicon.ico">
    <link rel="stylesheet" href="..//Tower_Defence_Tutorial/TemplateData/style.css">
    <script src="..//Tower_Defence_Tutorial/TemplateData/UnityProgress.js"></script>
    <script src="..//Tower_Defence_Tutorial/Build/UnityLoader.js"></script>
    <script>
      var unityInstance = UnityLoader.instantiate("unityContainer", "..//Tower_Defence_Tutorial/Build/Tower_Defence_Tutorial.json", {onProgress: UnityProgress});
    </script>
  </head>
  <body>
    <div class="webgl-content">
      <div id="unityContainer" style="width: 960px; height: 600px"></div>
      <div class="footer">
        <div class="webgl-logo"></div>
        <div class="fullscreen" onclick="unityInstance.SetFullscreen(1)"></div>
        <div class="title">Tower_Defence_Tutorial</div>
      </div>
    </div>
  </body>
</html>
