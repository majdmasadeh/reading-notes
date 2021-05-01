# Images, Color, Text

## Image In HTML
![img](https://lh3.googleusercontent.com/proxy/VKMi_dkFswRo4NS7FSsJDr6VLICoEkwqzupNjcGeIfI8gYW68YbczJN9MIzDrixqcEfCka2_SRn8x94tO7ztiZuNu-9SVaLxzutG7YOssEoOSM-9ml4)

There are many reasons why you mightmwant to add an image to a web page: youmight want to include a logo, photograph, illustration, diagram, or chart. so how we can add image ? . 
we use  element ; that mean there is not close tage . and two attributes scr this to tell where the image find and alt to give description of the image if you cannot see it. 
also we can use title attribute to provide additional information for the image.

![img2](https://img.webnots.com/2017/01/Raw-Code-on-Visual-Editor.jpg)

![img2](https://miro.medium.com/max/459/1*Fa1GefqQbmKMOLTRsjMkUQ.png)


### The  element is used to add images to a web page.

You must always specify a src attribute to indicate the source of an image and an alt attribute to describe the content of an image.
You should save images at the size you will be using them on the web page and in the appropriate format.
Photographs are best saved as JPEGs; illustrations or logos that use flat colors are better saved as GIFs.


## Colors

Color not only brings your site to life, but also helps convey the mood and evokes reactions.
There are three ways to specify colors in CSS: RGB values, hex codes, and color names.
- Color pickers can help you find the color you want.
- It is important to ensure that there is enough contrast between any text and the background color (otherwise people will not be able to read your content).
- CSS3 has introduced an extra value for RGB colors to indicate opacity. It is known as RGBA.
- CSS3 also allows you to specify colors as HSL values, with an optional opacity value. It is known as HSLA.

![img3](https://www.w3schools.com/w3css/img_analogous.png)

### HSL Colors

hue Hue is the colloquial idea of color. In HSL colors, hue is often represented as a color circle where the angle represents the color, although it may also be shown as a slider with values from 0 to 360.

saturation Saturation is the amount of gray in a color. Saturation is represented as a percentage. 100% is full saturation and 0% is a shade of gray.

lightness Lightness is the amount of white (lightness) or black (darkness) in a color. Lightness is represented as a percentage. 0% lightness is black, 100% lightness is white, and 50% lightness is normal. Lightness is sometimes referred to as luminosity.

Color not only brings your site to life, but also helps convey the mood and evokes reactions.

![img4](https://i2.wp.com/www.cssscript.com/wp-content/uploads/2018/03/kwulers.png?fit=539%2C412&ssl=1)

### Contrast
When picking foreground and background colors, it is important to ensure that there is enough contrast for the text to be legible:

- low contrast.
- medium contrast.
- high contrast.
The high contrast is better than the low one.

## Text
Typeface Terminology
1- SERIF:used for long passages of text because they were considered easier to read.
2- SANS-SERIF:if the text is small sans-serif fonts can be clearer to read.
3- MONOSPACE:they align nicely, making the text easier to follow.
![img5](https://jetline.co.za/wp-content/uploads/2018/04/typography.png)

### The CSS font-family Property
In CSS, we use the font-family property to specify the font of a text.

The font-family property should hold several font names as a “fallback” system, to ensure maximum compatibility between browsers/operating systems. Start with the font you want, and end with a generic family (to let the browser pick a similar font in the generic family, if no other fonts are available). The font names should be separated with comma.

Note: If the font name is more than one word, it must be in quotation marks, like: “Times New Roman”.
![img6](https://www.whatfontis.com/blog/wp-content/uploads/2018/02/font-infography.jpg)

### Font size
The font-size property enables you to specify a size for the font. There are several ways to specify the size of a font. The most common are: pixels Pixels are commonly used because they allow web designers very precise control over how much space their text takes up. The number of pixels is followed by the letters px. percentages The default size of text in browsers is 16px. So a size of 75% would be the equivalent of 12px, and 200% would be 32px. If you create a rule to make all text inside the body element to be 75% of the default size (to make it 12px), and then specify another rule that indicates the content of an element inside the body element should be 75% size, it will be 9px (75% of the 12px font size). ems An em is equivalent to the width of a letter m.

![img7](https://www.tutorialbrain.com/wp-content/uploads/2019/02/Font-in-HTML.jpg)
![img8](https://i1.wp.com/halfelf.org/wp-content/uploads/sites/2/2013/11/fontsize-accessible-email.jpg?fit=268%2C312&ssl=1)
