# **CSS**

# Transforms
1. **2D Transforms**

  * 2D rotate ,2D Scale,2D Translate 

  ```
  html>>>> <figure class="box-1">Box 1</figure>
  css>>>>>
   .box-1 { 
       transform: rotate(20deg);
       transform: scale(.75);
       transform: translateX(-10px);

       }

  ```

  ![img1](https://image.slidesharecdn.com/css3transforms-110622085054-phpapp01/95/css3-2d3d-transform-4-728.jpg?cb=1308732778)

   and we can specify the scale for x ,y


   * and you can control the skew by `transform: skewX(5deg);` ,combining transform ,transform origin 
   `.box-1 {transform: rotate(15deg); transform-origin: 0 0;}` and Perspective
    `.box { transform: perspective(200px) rotate(45deg);}` you control for it's  depth and origin Value .

    2. **3D Transforms**

it workes as  the same elements of 2D and in the same way but we have to give it value for z-axis dimensional and in addition in transform style On occasion three-dimensional transforms will be applied on an element that is nested within a parent element which is also being transformed and Backface Visibility

 ```
 <div class="rotate three-d">
<figure class="box">Box 1</figure>
css>>>>>>>>>
.rotate {
  transform: perspective(200px) rotateY(45deg);
   }
.three-d {
  transform-style: preserve-3d;
 }
 backface-visibility: hidden;
 ```
![img2](https://tipsmake.com/data/images/3d-transform-in-css-picture-1-jtznOkrOW.jpg)

## CSS Transitions & Animations
### Transitions

![img4](https://stfalcon.com/uploads/images/5881e0b98e717.png)

There are four transition related properties in total, including transition-property, transition-duration, transition-timing-function, and transition-delay
1. The transition-property property determines exactly what properties will be altered in conjunction with the other transitional properties
2. The duration in which a transition takes place is set using the transition-duration property
3. The transition-timing-function property is used to set the speed in which a transition will move
4.  The delay sets a time value, seconds or milliseconds, that determines how long a transition should be stalled before executin

```
.box {
  background: #2db34a;
  border-radius: 6px
  transition-property: background, border-radius;
  transition-duration: .2s, 1s;
  transition-timing-function: linear, ease-in;
  transition-delay: 0s, 1s;
}
.box:hover {
  background: #ff7b29;
  border-radius: 50%;
}

```


*  there is a shorthand property, `transition`, capable of supporting all of these different properties and values. Using the transition value alone, you can set every transition value in the order of transition-property, transition-duration, transition-timing-function, and lastly transition-delay ` transition: background .2s linear, border-radius 1s ease-in 1s`

# Animations

![img3](https://i.ytimg.com/vi/2a2p2FhBgfA/maxresdefault.jpg)

1. To set multiple points at which an element should undergo a transition, use the `@keyframes` rule
2. animations behave similarly to transitions. They include a duration, timing function, and delay if desired
3. On top of being able to set the number of times an animation repeats, you may also declare the direction an animation completes using the animation-direction property. Values for the animation-direction property include normal, reverse, alternate, and alternate-reverse
4. The animation-play-state property allows an animation to be played or paused using the running and paused keyword values respectivel
5. The animation-fill-mode property identifies how an element should be styled either before, after, or before and after an animation is run


```
.stage:hover .ball {
  animation-name: slide;
  animation-duration: 2s;
  animation-timing-function: ease-in-out;
  animation-delay: .5s;
  animation-fill-mode: forwards;
}
.stage:active .ball {
  animation-play-state: paused;
}

```


* shorthand animation can be written out in a shorthand format. This is accomplished with one `animation` property, rather than multiple declarations. The order of values within the animation property should be animation-name, animation-duration, animation-timing-function, animation-delay, animation-iteration-count, animation-direction, animation-fill-mode, and lastly animation-play-state

`  animation: slide 2s ease-in-out .5s infinite alternate;`


1. Fade in `.fade{opacity:0.5;}  .fade:hover{opacity:1;}` 
2. Change color ` .color:hover{background:#53a7ea;} `
3. Grow & Shrink ` .grow:hover{-webkit-transform: scale(1.3);  -ms-transform: scale(1.3); transform: scale(1.3); }`
4. Square to circle `.circle:hover { border-radius:50%;}`
5. and others button style like  3D shadow , Swing, Inset border

## 8 SIMPLE CSS3 TRANSITIONS THAT WILL WOW YOUR USERS

![img4](https://i.pinimg.com/originals/40/c0/a6/40c0a6c04d35246cb84408749fbf7f95.jpg)

![](https://slideplayer.com/slide/3827203/13/images/56/CSS3+Transition+Properties.jpg)

1- Fade in:Having things fade in is a fairly common request from clients. It’s a great way to emphasize functionality or draw attention to a call to action.

2- Change color Animating a change of color used to be unbelievably complex, with all kinds of math involved in calculating separate RGB values and then recombining them. Now, we just set the div’s class to “color” and specify the color we want in our CSS.

3- Grow & Shrink To grow an element, you used to have to use its width and height, or its padding. But now we can use CSS3’s transform to enlarge.

4- Rotate elements CSS transforms have a number of different uses, and one of the best is transforming the rotation of an element. Give your div the class “rotate” and add the following to your CSS

5- Square to circle A really popular effect at the moment is transitioning a square element into a round one, and vice versa. With CSS, it’s a simple effect to achieve, we just transition the border-radius property.

6- 3D shadow 3D shadows were frowned upon for a year or so, because they weren’t seen as compatible with flat design, which is of course nonsense, they work fantastically well to give a user feedback on their interactions and work with flat, or fake 3D interfaces.

