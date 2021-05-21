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


## Animation Name
Once the keyframes for an animation have been declared they need to be assigned to an element. To do so, the animation-name property is used with the animation name, identified from the @keyframes rule

## Animation Duration, Timing Function,Iteration & Delay
```
.stage:hover .ball {
  animation-name: slide;
  animation-duration: 2s;
  animation-timing-function: ease-in-out;
  animation-delay: .5s;
  animation-iteration-count: infinite;
}
```
## Animation Play State
The `animation-play-state` property allows an animation to be played or paused using the `running` and `paused` keyword values respectively.
### Example
```
.stage:active .ball {
  animation-play-state: paused;
}
```
## Animation Fill Mode
The animation-fill-mode property identifies how an element should be styled either before, after, or before and after an animation is run. The animation-fill-mode property accepts four keyword values, including none, forwards, backwards, and both.

## Shorthand Animations
Fortunately animations, just like transitions, can be written out in a shorthand format.

### Example
```
.stage:hover .ball {
  animation: slide 2s ease-in-out .5s infinite alternate;
}
```

## CSS3 has introduced countless possibilities for UX designers, and the best thing about them is that the coolest parts are really simple to implement.

### Just a couple of lines of code will give you an awesome transition effect that will excite your users, increase engagement and ultimately, when used well, increase your conversions. What’s more, these effects are hardware accelerated, and a progressive enhancement that you can use right now.

### Here are 8 really simple effects that will add life to your UI and smiles to your users’ faces.

### 1. Fade in
##### Having things fade in is a fairly common request from clients. It’s a great way to emphasize functionality or draw attention to a call to action.

##### Fade in effects are coded in two steps: first, you set the initial state; next, you set the change, for example on hover:

                .fade
                {
                        opacity:0.5;
                }
                .fade:hover
                {
                        opacity:1;
                }

### 2. Change color
##### Animating a change of color used to be unbelievably complex, with all kinds of math involved in calculating separate RGB values and then recombining them. Now, we just set the div’s class to “color” and specify the color we want in our CSS:

                .color:hover
                {
                        background:#53a7ea;
                }

### 3. Grow & Shrink
##### To grow an element, you used to have to use its width and height, or its padding. But now we can use CSS3’s transform to enlarge.

##### Set your div’s class to “grow” and then add this code to your style block:

                .grow:hover
                {
                        -webkit-transform: scale(1.3);
                        -ms-transform: scale(1.3);
                        transform: scale(1.3);
                }

##### Shrinking an element is as simple as growing it. To enlarge an element we specify a value greater than 1, to shrink it, we specify a value less than 1:

                .shrink:hover
                {
                        -webkit-transform: scale(0.8);
                        -ms-transform: scale(0.8);
                        transform: scale(0.8);
                }


### 4. Rotate elements
##### CSS transforms have a number of different uses, and one of the best is transforming the rotation of an element. Give your div the class “rotate” and add the following to your CSS:

                .rotate:hover
                {
                        -webkit-transform: rotateZ(-30deg);
                        -ms-transform: rotateZ(-30deg);
                        transform: rotateZ(-30deg);
                }

### 5. Square to circle
##### A really popular effect at the moment is transitioning a square element into a round one, and vice versa. With CSS, it’s a simple effect to achieve, we just transition the border-radius property.

##### Give your div the class “circle” and add this CSS to your styles:

                .circle:hover
                {
                        border-radius:50%;
                }


### 6. 3D shadow
##### 3D shadows were frowned upon for a year or so, because they weren’t seen as compatible with flat design, which is of course nonsense, they work fantastically well to give a user feedback on their interactions and work with flat, or fake 3D interfaces.

##### This effect is achieved by adding a box shadow, and then moving the element on the x axis using the transform and translate properties so that it appears to grow out of the screen.

##### Give your div the class “threed” and then add the following code to your CSS:

                .threed:hover
                {
                        box-shadow:
                                1px 1px #53a7ea,
                                2px 2px #53a7ea,
                                3px 3px #53a7ea;
                        -webkit-transform: translateX(-3px);
                        transform: translateX(-3px);
                }

### 7. Swing
##### Not all elements use the transition property. We can also create highly complex animations using @keyframes, animation and animation-iteration.

##### In this case, we’ll first define a CSS animation in your styles. You’ll notice that due to implementation issues, we need to use @-webkit-keyframes as well as @keyframes (yes, Internet Explorer really is better than Chrome, in this respect at least).

                @-webkit-keyframes swing
                {
                15%
                {
                        -webkit-transform: translateX(5px);
                        transform: translateX(5px);
                }
                30%
                {
                        -webkit-transform: translateX(-5px);
                transform: translateX(-5px);
                } 
                50%
                {
                        -webkit-transform: translateX(3px);
                        transform: translateX(3px);
                }
                65%
                {
                        -webkit-transform: translateX(-3px);
                        transform: translateX(-3px);
                }
                80%
                {
                        -webkit-transform: translateX(2px);
                        transform: translateX(2px);
                }
                100%
                {
                        -webkit-transform: translateX(0);
                        transform: translateX(0);
                }
                }
                @keyframes swing
                {
                15%
                {
                        -webkit-transform: translateX(5px);
                        transform: translateX(5px);
                }
                30%
                {
                        -webkit-transform: translateX(-5px);
                        transform: translateX(-5px);
                }
                50%
                {
                        -webkit-transform: translateX(3px);
                        transform: translateX(3px);
                }
                65%
                {
                        -webkit-transform: translateX(-3px);
                        transform: translateX(-3px);
                }
                80%
                {
                        -webkit-transform: translateX(2px);
                        transform: translateX(2px);
                }
                100%
                {
                        -webkit-transform: translateX(0);
                        transform: translateX(0);
                }
                }

##### This animation simply moves the element left and right, now all we need to do is apply it:

                .swing:hover
                {
                        -webkit-animation: swing 1s ease;
                        animation: swing 1s ease;
                        -webkit-animation-iteration-count: 1;
                        animation-iteration-count: 1;
                }

### 8. Inset border
##### One of the hottest button styles right now is the ghost button; a button with no background and a heavy border. We can of course add a border to an element simply, but that will change the element’s position. We could fix that problem using box sizing, but a far simpler solution is the transition in a border using an inset box shadow.

##### Give your div the class “border” and add the following CSS to your styles:

                .border:hover
                {
                        box-shadow: inset 0 0 0 25px #53a7ea;
                }


You can see the all result from her: [RESULT](https://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users)


---
---


# 6 Buttons animated
You can see the 6 button from her: [RESULT](https://codepen.io/retyui/pen/ByoaXV?editors=1111)


---
---
# CSS3 Keyframes Animation
You can see the CSS3 Keyframes Animation from her: [RESULT](https://codepen.io/akshaychauhan/pen/oAfae)


---
---
# 404
You can see the **404** from her: [RESULT](https://codepen.io/kieranfivestars/pen/MYdQxX)


---
---
# Pure CSS Bounce Animation
You can see the **Pure CSS Bounce Animation** from her: [RESULT](https://codepen.io/dp_lewis/pen/gCfBv)



