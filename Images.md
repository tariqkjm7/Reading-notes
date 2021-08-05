# There are many reasons why you might want to add an image to a web page: 

you might want to include a logo, photograph, illustration, diagram, or chart.There are several things to consider when selecting and preparing images for your site, but taking time to get them right will make it look more attractive and professional  this page you will learn how to:
Include an image in your web pages using HTML::

* Pick which image format to use.
* Show an image at the right size.
* Optimize an image for use on the web to make pages.      
* load faster.

## ChoosIng Images for Your sIte
A picture can say a thousand words, and great images help make the difference between an average-looking site and a really engaging one.

**Images can be used to set the tone for a site in less time than it takes to read a description. If you do not have photographs to use on your website, there are companies who sell stock images; these are images you pay to use (there is a list of stock photography websites below). Remember that all images are subject to copyright, and you can get in trouble for simply taking photographs from another website.If you have a page that shows several images (such as product photographs or members of a team) then putting them on a simple, consistent background helps them look better as a group.**

Images should Be:
 * relevant
 * Convey information
* Convey the right mood
* Be instantly recognisable
* Fit the color palette

![img](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT7rPp9LU6vlPJjJVZ3qDAdCJr6cYVdoVV4CA&usqp=CAU)

## adding Images

(img)To add an image into the page you need to use an (img)element. This is an empty element (which means there is no closing tag). It must carry the following two attributes:srcThis tells the browser where it can find the image file. This will usually be a relative URL pointing to an image on your own site. (Here you can see that the images are in a child folder called images — relative URLs were covered on pages 83-84). altThis provides a text description of the image which describes the image if you cannot see it.titleYou can also use the titleattribute with the (img) element to provide additional information about the image. Most browsers will display the content of this attribute in a tootip when the user hovers over the image.add Ing ImagesThe text used in the alt attribute is often referred to as alt text. It should give an accurate description of the image content so it can be understood by screen reader software (used by people with visual impairments) 


### heIght & WIdth of Images

You will also often see an (img) element use two other attributes that specify its size:<br>
**height** This specifies the height of the image in pixels.<br>
**width** This specifies the width of the image in pixels.

**Images** often take longer to load than the HTML code that makes up the rest of the page. It is, therefore, a good idea to specify the size of the image so that the browser can render the rest of the text on the page while leaving the right amount of space for the image that is still loading.The size of images is increasingly being specified using CSS rather than HTML — see pages 409-410 for more information about this.