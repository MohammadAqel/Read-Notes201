# Images

*There are many reasons why you might want to add an image to a web page: you might want to include a logo, photograph, illustration, diagram, or chart.*

*There are several things to consider when selecting and preparing images for your site, but taking time to get them right will make it look more attractive and professional.*

### In this chapter you will learn how to:

1. Include an image in your web pages using HTML
2. Pick which image format to use
3. Show an image at the right size
4. Optimize an image for use on the web to make pages load faster

## Choosing Images for Your Site

*A picture can say a thousand words, and great images help make the difference between an average-looking site and a really engaging one.*

*Images can be used to set the tone for a site in less time than 
it takes to read a description. If you do not have photographs to use on your website, there are companies who sell stock images; these are images you pay to use (there is a list of stock photography websites below).*

*Remember that all images are subject to copyright, and you can get in trouble for simply taking photographs from another website.*

*If you have a page that shows several images (such as product photographs or members of a team) then putting them on a simple, consistent background helps them look better as a group.*

## Storing Images on Your Site

*If you are building a site from scratch, it is good practice to create a folder for all of the images the site uses.*

*As a website grows, keeping images in a separate folder helps you understand how the site is organized. Here you can see an example of the files for a website; all of the images are stored in a folder called images.*

*On a big site you might like to add subfolders inside the imagesfolder. For example, images such as logos and buttons might sit in a folder called interface, product photographs might sit in a page called products, and images related to news might live in a folder called news.*

*If you are using a content management system or blogging platform, there are usually tools built into the admin site that allow you to upload images, and the program will probably already have a separate folder for image files and any other uploads.*

## Adding Images

*To add an image into the page you need to use an <img>element. This is an empty element (which means there is no closing tag). It must carry the following two attributes:*

1. src

*This tells the browser where it can find the image file. This will usually be a relative URL pointing to an image on your own site. (Here you can see that the images are in a child folder called images — relative URLs were covered on pages 83-84).*


2. alt

*This provides a text description of the image which describes the image if you cannot see it.*

#### title

*You can also use the titleattribute with the <img> element to provide additional information about the image. Most browsers will display the content of this attribute in a tootip when the user hovers over the image.*

*The text used in the alt attribute is often referred to as alt text. It should give an accurate description of the image content so it can be understood by screen reader software (used by people with visual impairments) and search engines.*

*If the image is just to make a page look more attractive (and it has no meaning, such as a graphic dividing line), then the alt attribute should still be used but the quotes should be left empty.*

# Color

*Color can really bring your pages to life.*

*In this chapter we will look at:*

1. How to specify colors, as there are three common ways in which you can indicate your choice of colors (plus extra ways made available in CSS3)

2. Color terminology, as there are some terms that are very helpful to understand when it comes to picking colors.

3. Contrast, and ensuring that your text is readable.

4. Background colors for behind either your entire page or parts of a page.

*What you will learn about colors in this chapter will then be used in subsequent chapters when it comes to looking at colors of text and boxes in CSS.*

### Background Color

*CSS treats each HTML element as if it appears in a box, and the background-color property sets the color of the background for that box.*

*You can specify your choice of background color in the same three ways you can specify foreground colors: RGB values, hex codes, and color names (covered on the next page).*

*If you do not specify a background color, then the background is transparent.*

*By default, most browser windows have a white background, but browser users can set a background color for their windows, so if you want to be sure that the background is white you can use the background-color property on the <body> element.*

# Text

*The properties that allow you to control the appearance of text can be split into two groups:*

1. Those that directly affect the font and its appearance (including the typeface, whether it is regular, bold or italic, 
and the size of the text)

2. Those that would have the same effect on text no matter what font you were using (including the color of text and the spacing between words and letters) The formatting of your text can have a significant effect on how readable your pages are. As we look through these properties I will also give you some design tips on how to display your type.

### Specifying Typefaces

*The font-family property allows you to specify the typeface that should be used for any text inside the element(s) to 
which a CSS rule applies.*

*The value of this property is the name of the typeface you want to use.*

*The people who are visiting your site need the typeface you have specified installed on their computer in order for it to be displayed.* 

*You can specify a list of fonts separated by commas so that, if the user does not have your first choice of typeface installed, the browser can try to use an alternative font from the list.*

*It is also common to end with a generic font name for that type of font (which you saw on pages 269-270).*

*If a font name is made up of more than one word, it should be put in double quotes.*

### Size of Type

*The font-size property enables you to specify a size for the font. There are several ways to specify the size of a font. The most common are:*

1. pixels

*Pixels are commonly used because they allow web designers very precise control over how much space their text takes up. The number of pixels is followed by the letters px.*

2. percentages

*The default size of text in browsers is 16px. So a size of 75% would be the equivalent of 12px, and 200% would be 32px.If you create a rule to make all text inside the <body> element to be 75% of the default size (to make it 12px), and then specify another rule that indicates the content of an element inside the <body> element should be 75% size, it will be 9px (75% of the 12px font size).*

3. EmsAn

*em is equivalent to the width of a letter m.*

### Type Scales

*You may have noticed that programs such as Word, Photoshop and InDesign offer the same sizes of text.*

*Type Scales:*

1. 8pt
2. 9pt
3. 10pt
4. 11pt
5. 12pt
6. 14pt
7. 18pt
8. 24pt
9. 36pt
10. 48pt
11. 60pt
12. 72pt

*This is because they are set according to a scale or ratio that was developed by European typographers in the sixteenth 
century.*

*It is considered that this scale for type is pleasing to the eye and it has therefore changed little in the last 400 years.*

*For this reason, when you are designing pages, using sizes from this scale will help them look more attractive.*

*On the next page, you can see how to achieve this scale using pixels, percentages, and ems.Print designers often refer to the size of text in terms of points rather than pixels (hence the use of pt in the scale on the right). A pixel roughly equates to a point because a point corresponds to 1/72 of an inch, and most computer displays have a resolution of 72 dots per inch.*

*The default size of text in a browser is 16 pixels. So if you use percentages or ems, you calculate the size of text you 
want based on the default size of the text used in browsers. For example, you could scale down to 12 pixels for body copy and scale up to 24 pixels for headings.*

*Recently, some web designers have started to leave the body text at the default size of 16 pixels and adjust the other font sizes using a scale that keeps the relative proportions of this one.*

*When you first see body text at 16 pixels, it might seem quite large. Once you get used to the larger type, however, most people find it far easier to read; and going back to a page where main type is 12 pixels will often then look quite small.*

## @font-face

*@font-face allows you to use a font, even if it is not installed on the computer of the person browsing, by allowing you to specify a path to a copy of the font, which will be downloaded if it is not on the user's machine.*

*Because this technique allows a version of the font to be downloaded to the user's computer, it is important that the license for the font permits it to be used in this way.*

### font-family

*This specifies the name of the font. This name can then be used as a value of the font-familyproperty in the rest of the style sheet (as shown in the rule for the <h1> and <h2> elements).*

### src

*This specifies the path to the font. In order for this technique to work in all browsers, you will probably need to specify paths to a few different versions of the font, as shown on the next page.*

### format

*This specifies the format that the font is supplied in. (It's discussed in detail on the next page.)*

## font-weight

*The font-weight property allows you to create bold text. There are two values that this property commonly takes:*

### normal

*This causes text to appear at a normal weight.*

### bold

*This causes text to appear bold*

## font-style

*If you want to create italic text, you can use the font-styleproperty. There are three values this property can take:*

### normal

*This causes text to appear in a normal style (as opposed to italic or oblique).*

### italic

*This causes text to appear italic.*

### oblique

*This causes text to appear oblique.*

for more information: https://en.wikipedia.org/wiki/Help:Advanced_text_formatting
