# Images :
In Html we can add images using img tag :

Example :

	<img src="cat.pmg" />

and we can resize the image using css style properties width and height 

Example :

	img
	{
		width:50%;
		height:50%;
	}

we can also add the image as a background for the elements

Example :

	body
	{
		background-image:url("cat.png")
	}

##The background-repeat property can have four values:

1.repeat : The background image is repeated both horizontally and vertically (the default way it is shown if the backgroundrepeat property isn't used).

2.repeat-x : The image is repeated horizontally only (as shown in the first example on the left).

3.repeat-y : The image is repeated vertically only.

4.no-repeat : The image is only shown once.

5.fixed : The background image stays in the same position on the page.

6.scroll : The background image moves up and down as the user scrolls up and down the page.

##Some notes for Images :

Images can be aligned both horizontally and vertically using CSS.

You can use a background image behind the box created by any element on a page.

Background images can appear just once or be repeated across the background of the box.

You can create image rollover effects by moving the background position of an image.

To reduce the number of images your browser has to load, you can create image sprites.


# Search Engine Optimization (SEO) :
Search engine optimization helps visitors find your
sites when using search engines , Analytics tools such as Google Analytics allow you to
see how many people visit your site, how they find it,
and what they do when they get there.To put your site on the web, you will need to obtain a
domain name and web hosting.
FTP programs allow you to transfer files from your
local computer to your web server.
Many companies provide platforms for blogging, email
newsletters, e-commerce and other popular website
tools (to save you writing them from scratch).


### Video and audio 

You can review what all the HTML features do in the article linked above; for our purposes here, the most interesting attribute is controls, which enables the default set of playback controls.

One big issue with the native browser controls is that :
##### 1. they are different in each browser 
##### 2. the native controls in most browsers aren't very keyboard-accessible.

# Video :

To show a video in HTML, use the video element.

Example :

	<video width="320" height="240" controls>
    <source src="movie.mp4" type="video/mp4">
    <source src="movie.ogg" type="video/ogg">
    Your browser does not support the video tag.
    </video>

The controls attribute adds video controls, like play, pause, and volume.

It is a good idea to always include width and height attributes. If height and width are not set, the page might flicker while the video loads.

The <source> element allows you to specify alternative video files which the browser may choose from. The browser will use the first recognized format.

The text between the <video> and </video> tags will only be displayed in browsers that do not support the <video> element.

To start a video automatically, use the autoplay attribute:

	
	<video width="320" height="240" autoplay>
    <source src="movie.mp4" type="video/mp4">
    <source src="movie.ogg" type="video/ogg">
    Your browser does not support the video tag.
     </video>



## Chapter 19: “Practical Information”

## PRACTICAL INFORMATION
 -Search engine optimization helps visitors find your sites when using search engines.
 -Analytics tools such as Google Analytics allow you to see how many people visit your site, how they find it, and what they do when they get there.

![SEO](https://www.loebigink.com/wp-content/uploads/2016/04/Loebigseo.png)

 -To put your site on the web, you will need to obtain a domain name and web hosting.
 -FTP programs allow you to transfer files from your local computer to your web server.
- Many companies provide platforms for blogging, email newsletters, e-commerce and other popular website tools (to save you writing them from scratch).

![FTP](https://th.bing.com/th/id/R49a897ecda8333f2be80e6a93545e362?rik=35O3jJaIAt%2brlA&riu=http%3a%2f%2fwww.highteck.net%2fimages%2f39-FTP.jpg&ehk=8BJttRrR%2fwIbPBfx4puULvRXlw4TCMb3t4bvunFJQ7k%3d&risl=&pid=ImgRaw)
