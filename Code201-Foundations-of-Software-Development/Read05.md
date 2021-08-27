   Sometimes, it is required to fit an image into a certain given dimension. We can resize the image by specifying the width and height of an image. A common solution is to use the max-width: 100%; and height: auto; so that large images do not exceed the width of their container. The max-width and max-height properties of CSS works better, but they are not supported in many browsers.

Another way of resizing the image is by using the object-fit property, which fits the image. This CSS property specifies how a video or an image is resized to fit its content box. It defines how an element fits into the container with an established width and height.

The object-fit property is generally applied to image or video. This property defines how an element responds to the width and height of its container. Mainly there are five values of object-fit property such as fill, contain, cover, none, scale-down, initial, and inherit. The default value of this property is "fill".

Example
In this example, we are resizing the image by using the max-width: 100%; and height: auto; properties.

-------
<!DOCTYPE html>  
<html>  
<head>  
<title>cell padding</title>  
<style>  
div {  
width: auto;  
text-align: center;  
padding: 15px;  
border: 3px solid red;  
}  
img {  
max-width: 100%;  
height: auto;  
}  
</style>  
</head>  
<body>  
<div>  

</div>  
</body>  
</html>  

-------

![Output](https://static.javatpoint.com/csspages/images/how-to-change-image-size-in-css1.png)
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   JPG, PNG or GIF? Which image format should you be using in your digital design?

As government communicators, often we have to work with design in all formats, especially digital design. But when you need to throw a picture up on your website, into an email, or send out in a social media post, is it a quick and easy process? Do you know the different effects something as simple as a file format can have on the look and feel of your communications?

We’ve compiled some background on the ins and outs of the three major image formats for Web design to help you do your job quicker and easier.

When dealing with digital design, there are only a handful of file formats we have to concern ourselves with. The three main file types used for digital use are .PNG, .JPG, and .GIF. There are some pretty big differences as to which file type would be appropriate for your current project, and choosing the right one can make all the difference in the world. Knowing which format to use can save a lot of time and prevent you from having to make any changes after the file is sent or uploaded.


![JPG](https://granicus.com/wp-content/uploads/image/png/blog_jpg.png)

The standard “go to” file format at the moment is .JPG. However, the uses in which .JPG would be preferable over a .PNG are a lot more limited. The .JPG format is best used in the case of complex images with no text. By its nature, .JPG reduces loading times by selectively deleting elements of a photo. This is great for large detailed photographs that would otherwise take very long to load. When done to an image with elements that utilize sharp and straight edges, pixilation around these areas become very apparent, making text range from unpleasant to unreadable depending on the size. To avoid this, stick to using .JPG for very detailed images that don’t feature text or other hard-edged graphics.

![PNG](https://granicus.com/wp-content/uploads/image/png/blog_png.png)

The .PNG file format is what we would most often use in digital design projects. The .PNG, or Portable Network Graphic, tends to have a larger file size than the other two formats, but it also preserves hard edges and can handle a high amount of colors while keeping the load time fast enough to use online. Another interesting capability is that it can be saved on a transparency. This means we can utilize the important elements of an image without needing to change things like a background color if we placed it on transparency. This is a big reason why most major sites create their logo as a .PNG, so it doesn’t need to change whenever their site is updated. Best uses for .PNG include images that contain text, graphics with hard edges, and elements that require transparent backgrounds like logos.


![GIF](https://granicus.com/wp-content/uploads/image/png/blog_gif.png)

The .GIF file format is essentially the faster loading cousin of .PNG with one catch—the image needs to be under exactly 256 colors. This limits designers a lot more than you’d think. You should only use this file format for low-resolution images. So elements like photographs or graphics that use gradients would immediately be out of the question for the .GIF format. But elements like solid color buttons or banners are ideal as these will (usually) load faster than the .PNG version, while keeping all the cool features like transparencies and preserving hard edges. Another awesome feature that only .GIFs can utilize is animation. So you can create a graphic that utilizes a short looping or single play animation, which does not require any plug-ins since it’s only an image file.




-----


## Stylesheets cascade —
at a very simple level, this means that the order of CSS rules matter; when two rules apply that have equal specificity the one that comes last in the CSS is the one that will be used.

In the below example, we have two rules that could apply to the h1. The h1 ends up being colored blue — these rules have an identical selector and therefore carry the same specificity, so the last one in the source order wins.

 

**Specificity**
Specificity is how the browser decides which rule applies if multiple rules have different selectors, but could still apply to the same element. It is basically a measure of how specific a selector's selection will be:

- An element selector is less specific — it will select all elements of that type that appear on a page — so will get a lower score.
- A class selector is more specific — it will select only the elements on a page that have a specific class attribute value — so will get a higher score.
Example time! Below we again have two rules that could apply to the h1. The below h1 ends up being colored red — the class selector gives its rule a higher specificity, and so it will be applied even though the rule with the element selector appears further down in the source order.

