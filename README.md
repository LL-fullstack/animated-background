# Animated-background
Tutorial for an animated background

In order to make an animated background for your website, you can follow these
few steps below:

Step 1
1. Create a folder called 'Animated-background';
2. Create a subfolder called 'assets';
3. In 'assets' folder, create 2 subfolders named 'style' and 'images';
4. In 'style' folder, create a css file with name 'index.css';
5. In 'images' folder, put all the images you need to use for this project;
6. In 'Animated-background' folder, create a html file with name 'index.html'.

Step 2

In 'index.html' file, create <body>, navbar, content, sidebar and <button>. Use
<img> to link your pictures from 'images' folder.
Don't forget to link your 'index.css' file correctly here.

Step 3

In 'index.css' file, style hero section, navbar, button, content, side-bar, 
images, and links.
Use @keyframes to define the steps of an animation sequence. Each keyframe 
describes how the animated element should look at a particular time. The time is 
expressed as a percentage, with 0% representing the start of the animation and 
100% the end.

Syntax:

@keyframes slidein {
  from {
    transform: translateX(0%);
  }

  to {
    transform: translateX(100%);
  }
}

Example from the project:

@keyframes bubble {
    0% {
        transform: translateY(0);
        opacity: 0;
    }
    50% {
        opacity: 1;
    }
    70% {
        opacity: 1;
    }
    100% {
        transform: translateY(-80vh);
        opacity: 0;
    }
}

'animation-delay' allows to control when an animation should begin, after a 
specified time has elapsed. For example, animation-delay: 2s; means the animation 
will start 2 seconds after the element is loaded on the page.

Syntax:

/* Single animation */
animation-delay: 3s;

/* Multiple animations */
animation-delay: 2.1s, 480ms;

Example from the project:

.bubbles img:nth-child(1) {
    animation-delay: 2s;
}

.bubbles img:nth-child(2) {
    animation-delay: 1s;
}

.bubbles img:nth-child(3) {
    animation-delay: 3s;
}

.bubbles img:nth-child(4) {
    animation-delay: 4.5s;
}

.bubbles img:nth-child(5) {
    animation-delay: 3.5s;
}

.bubbles img:nth-child(6) {
    animation-delay: 6s;
}

.bubbles img:nth-child(7) {
    animation-delay: 7s;
}

'.bubbles img:nth-child()' is pseudo-class selects the 'img' element within the 
'.bubbles' container that is the 'n-th child' of its parent.

With 'animation-delay', it creates a visual effect, where each bubble begins 
its animation at different times, rather than all at once. 

Step 4

After adding all your content and styling, review your website in a web browser. 
Adjust the positions, sizes, and timings of the animations as needed to fit your 
design vision.


References

[@keyframes](https://developer.mozilla.org/en-US/docs/Web/CSS/@keyframes)
[animation-delay](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-delay)
[:nth-child()](https://developer.mozilla.org/en-US/docs/Web/CSS/:nth-child)
