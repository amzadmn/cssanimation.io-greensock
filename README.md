# How to use cssanimation.io's GSAP version
This library is not only built for CSS, it supports Greensock as well. Greensock is the standard JavaScript Animation framework in the world. It can help you to animate your HTML elements.

This is absolutely easy to have your HTML elements animated by our Greensock version. After include all the files just add your desired class name. 
So why worried?

please follow the instruction below

First, you download or grab the CDN URL of TweenMax.js plugin from GreenSock and download cssanimation.io's GSAP script cssanimation-gsap.js from `cssanimation.io`

1. Now include the TweenMax.min.js and cssanimation-gsap.js before the body tag like below:
```
<!DOCTYPE html>
<html lang="en">
<head> 
    <meta charset="UTF-8">
    <title>CSS Animation Library for Developers and Ninjas</title> 
</head> 
<body> 

   <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/1.19.1/TweenMax.min.js"></script> 
   <script type="text/javascript" src="cssanimation-gsap.js"></script>
</body>
</html>

```

2. Now add the class `cssanimation` and class of animation name like `fadeIn` for fade in animation to the element that you want to animate.
```
<!DOCTYPE html>
<html lang="en">
<head> 
    <meta charset="UTF-8">
    <title>CSS Animation Library for Developers and Ninjas</title> 
</head> 
<body> 

   <h1 class="cssanimation fadeIn"> Example </h1> 

   <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/1.19.0/TweenMax.min.js"></script> 
   <script type="text/javascript" src="cssanimation-gsap.js"></script>
</body>
</html>
```
### FadeIn Animation(greensock):
```
TweenMax.from(".fadeIn", 1, {alpha:0});
```
### FadeOut Animation(greensock):
```
TweenMax.to(".fadeOut", 1, {alpha:0});
```
### Move From Left Animation(greensock):
```
TweenMax.from(".moveFromLeft", 1, {x:"-100%"});
```
### Move From Right Animation(greensock):
```
TweenMax.from(".moveFromRight", 1, {x:"100%"});
```
### Hu...Hu...  Animation(greensock):
```
TweenMax.to(".hu__hu__", 1.5, {y:30, yoyo: true, repeat:-1, ease: Sine.easeInOut});
```
### Heartbeat Animation(greensock):
```
heartbeat = new TimelineMax({repeat:-1});
heartbeat
  .to(".heartbeat", 0.2, {css:{scale:1.3}})
  .to(".heartbeat", 0.16, {css:{scale:1.3}})
  .to(".heartbeat", 0.2, {css:{scale:1}})
```
