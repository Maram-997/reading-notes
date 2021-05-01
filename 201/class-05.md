# Read: 05 - HTML Images; CSS Color & Text
## IMAGES
* We add images to our website by **`<img>`** tag : it's an empty element (which means there is no closing tag). And it has the following attributes :
1. **src** : This tells the browser where it can find the image file. This will usually be a relative URL pointing to an image on your own site.
2. **alt** : This provides a text description of the image which describes the image if you cannot see it.
3. **title** : You can also use the title attribute with the `<img>` element to provide additional information about the image.

### The height and width of images : 
1. **height** : This specifies the height of the image in pixels.
2. **width** : This specifies the width of the image in pixels.
### Where to Place Images in Your Code:
1. **before a paragraph**
The paragraph starts on a new line after the image.
2. **inside the start of a paragraph**
The first row of text aligns with the bottom of the image.
3. **in the middle of a paragraph**
The image is placed between the words of the paragraph that it appears in.
![img](img-placing.png)
### Old Code: Aligning Images Horizontally
**align** The align attribute was commonly used to indicate how the other parts of a page should flow around an image. It has been removed from HTML5 and new websites should use CSS to control the alignment of images.
#### The align attribute can take these horizontal values:
**left**
This aligns the image to the left (allowing text to flow around its right-hand side).
**right**
This aligns the image to the right (allowing text to flow around its left-hand side).
#### Old Code: Aligning Images Vertically
There are three values that the align attribute can take that control how the image should align vertically with the text that surrounds it:
**top**
This aligns the first line of the surrounding text with the top of the image.
**middle**
This aligns the first line of the surrounding text with the middle of the image.
**bottom**
This aligns the first line of the surrounding text with the bottom of the image.
#### Three Rules for Creating Images :
* Save images in the right format.(GIF.PNG)
* Save images at the right size.
* Use the correct resolution.(The higher the resolution of the image, the larger the size of the file.)
#### Vector Images :
Vector images differ from bitmap images and are resolution-independent. Vector images are commonly created in programs such as Adobe Illustrator. Mainly used for logos and diagram.
> Vector images are created by placing points on a grid, and
drawing lines between those points. A color can then be added to "fill in" the lines that have been created.
>> The advantage of creating line drawings in vector format is that you can increase the dimensions of the image without affecting the quality of it.
#### Animated GIFs :
Animated GIFs show several frames of an image in sequence and therefore can be used to create simple animations.
#### Transparency :
Creating an image that is partially transparent for the web involves selecting one of two formats:(GIFs,PNG)
### HTML5: Figure and Figure Caption :
* `<figure>` Images often come with captions. HTML5 has introduced a new `<figure>` element to contain images and their caption so that the two are associated.
* `<figurecaption>` The `<figcaption>` element has been added to HTML5 in order to allow web page authors to add a caption to an image.
![img](caption.png)


## COLOR 
The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways:
* **RGB Values** : These express colors in terms 
of how much red, green and blue are used to make it up.are expressed as numbers between 0 and 255.
* **HEX Codes** : These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign. The value of the red, 102, is expressed as 66 in hexadecimal code.
* **color names** : There are 147 predefined color names that are recognized by browsers.

### Background-color :
CSS treats each HTML element as if it appears in a box, and the background-color property sets the color of the background for that box. And You can specify your choice of background color in the same three ways you can specify foreground colors.
#### understanding color :
Every color on a computer screen is created by mixing amounts of red, green, and blue. To find the color you want, you can use a color picker.
![img](colors.png)

#### Contrast :
When picking foreground and background colors, it is important to ensure that there is enough contrast for the text to be legible.
* Text is harder to read when there is low contrast between background and foreground colors.
* Text is easier to read when there is higher contrast between background and foreground colors.
* For long spans of text, reducing the contrast a little bit improves readability.
![img](contrast.png)
 #### CSS3: Opacity :opacity, rgba
CSS3 has introduced an extra value for RGB colors to indicate opacity. It is known as RGBA.
#### CSS3: HSL & HSLA :hsl, hsla
CSS3 also allows you to specify colors as HSL values, with an optional opacity value. It is known as HSLA.

## TEXT
#### Typeface Terminology :
* **serif** : Serif fonts have extra details on the ends of the main strokes of the letters. These details are known as serifs.`im`
* **sans-serif** :Sans-serif fonts have straight ends to letters, and therefore have a much cleaner design.
* **monospace** : Every letter in a monospace (or fixed-width) font is the same width. (Non-monospace fonts have different widths.)
![img](serif.png)

#### Choosing a Typeface for your Website :
When choosing a typeface, it is important to understand that a browser will usually only display it if it's installed on that user's computer.
![img](serif1.png)

#### Techniques That Offer a Wider Choice of Typefaces :

* font-family: The user's computer needs the typeface installed. CSS is used to specify the typeface.
* font-face: CSS specifies where a font can be downloaded from if it is not installed on the computer.
* Service-based Font-Face: Commercial services give users access to a wider range of fonts using @font-face.
* size of type(font-size): The font-size property enables you to specify a size for the font. There are several ways to specify the size of a font. The most common are:(Pixels,Percentages,EMS)
* Type scale : The default size of text in a browser is 16 pixels. this scale is pleasing to the eye.
* bold(font-weight): The font-weight property allows you to create bold text.
There are two values that this property commonly takes: (normail,bold).
* italic(font-style): If you want to create italic text,you can use the font-style property. There are three values this property can take: (normal,italic,oblique).
* Underline & Strike(text-decoration): The text-decoration property allows you to specify the following values:(none,underline,overline,line-through,blink)
* leading(line-height): is a term typographers use for the vertical space between lines of text. In a typeface, the part of a letter that drops beneath the baseline is called a *descender*, while the highest point of a letter is called the *ascender*.
* Alignment(test-align): The text-align property allows you to control the alignment of text. The property can take one of four values: (left,right,senter,justify).
* Vertical Alignment(vertical-align): The vertical-align property is a common source of confusion. It is not intended to allow you to vertically align text in the middle of block level elements, The Values it can take: (baseline,sub,super,top,text-top,middle
bottom,text-bottom)
* Indenting Text(text-indent): The text-indent property allows you to indent the first line of text within an element. The amount you want the line indented by can be specified in a number of ways but is usually given in pixels or ems. it can take a negative value, which means it can be used to push text off the browser window.
* CSS3: Drop Shadow(text-shadow): It is used to create a drop shadow, which is a dark version of the word just behind it and slightly offset. It can also be used to create an embossed effect by adding a shadow that is slightly lighter than the text.
![img](text-shadow.png)
* First Letter or Line(:first-letter, :first-line): You can specify different values for the first letter or first line of text inside an element using :first-letter and:first-line.
 #### Styling links:(:link, :visited)
 Browsers tend to show links in blue with an underline by default, and they will change the color of links that have been visited to help users know which pages they have been to.
 > there are two *pseudo-classes* that allow you to set different styles for links that have and have not yet been visited:
 >1. `:link`: This allows you to set styles for links that have not yet been visited.
 >2. `:visited`: This allows you to set styles for links that have been clicked on.
 #### UpperCase & LowerCase : (text-transform)
 The text-transform property is used to change the case of text giving it one of the following values: (uppercase,lowercase,capitalize(This causes the first letter of each word to appear capitalized.))
 #### Responding to Users(:hover, :active, :focus)
 it allows to change te appearance of elements when a user iteract with them.
1. :hover : This is applied when a user hovers over an element with a pointing device such as a mouse.
2. :active : This is applied when an element is being activated by a user; for example, when a button is being pressed or a link being clicked.
3. :focus : This is applied when an element has focus. Any element that you can interact with, such as a link you can click on or any form control can have focus.
#### Attributes Selectors:
There are also a set of attribute selectors that allow you to create rules that apply to elements that have an attribute with a specific value.
![img](attributes.png)
