# CSS_File  
               CHAPTER-0 & 1

HTML is just a skeleton layout of a website we need CSS to design a website add styles to it and meake it look bbeautiful.
body {
    background-color:red;

}

CSS- Cascading style sheet which is used for desiging the website and it is very useful skills for making websites as per your likings.

In HTML if we want to write CSS code lines we will write that below title tag and above the head tag or we can say that in between the title tag and head tag.

Syntax:-

<!-- <title> </title>
<style>
    </style>
<head>
</head> -->

Q:- What is DOM?
Ans-> It is document object model. when a page is laoded, the browser creates a DOM of the page which is constructed as a tree of object.

Q:- HTML id & class attributes.

Ans:- When an html elements is given an id, it serves as a unique identifiers for that element.
On the other hand, when an HTML elements is given a class, it now belongs to that class.More than one element can belongs to a single class but every elements must have a unique id(if assigned)
and one elemement can have multiple classes.

Synatx:-

<"div id = "first" class  = "c1 c2 c3" >
<"/div>

<"div id = "second">
<"/div>

<"section class = "red bg-blue">

</"section>

here "first" is a unique id
and c1,c2,c3 are multiple classes followed by spaces.
*multiple elemet can have one class.
*One element can have multiple classes.

-> There are 3 ways to add CSS to HTML.
#"style> tag-> Adding #style> #/style> to HTML-->


1) By using "style" tag in HTML between "head" tag and "title" tag we can use id which we give and open curlie brackets and give contents and agaian we close it by curlie brackets.

WE use " # " for targetting(calling elements) " id " and we use " . " for targetting(means calling class) class 
Syntax:-

#id_name{
    background-color: white:
}

.class_name{
    backgroud-color: white;
    color: white; means whatever we wrote inside that background we got that text in white color.
}

#2. Inline CSS-> Adding CSS using style attribute. -->

where we can write "style" tag inside our "div" tag folowed by background color(check index2.html file)


#3. External CSS -> Adding a style(.css) to HTML using "link" tag.  --> 

we add "link" tag between the "tittle" tag and "head" and we work according to that.

#CSS selectors

#A CSS selectors is used to select an HTML elements for styling.

where 
body { 
    color : red; --> declaration(property:value)

    background:pink --> declaration}

  #here "body" is known as CSS selectors.

  where
  h2{

  }
#Here h2 is an element and if we select this, then this is known as element selectors.

#ID selectors:- suppose we have any id mentioned in our files check index1.html where we define id , if we select that id then 
we called it as id selectors #id_name{} (is the id selectors.)

#class selectors:- chekc index3.html in which we define a class name and synatx of selexting class is .class_name{}.


            IMPORTANT NOTES

#1-> we can group selectors in the way:-
h1,h1,h3,h4,div{
    color: red;

}

#2-> We can use element.class as a selector like this:

p.red{
    color: red # here all the pragraph get red.
}

#(  "*")-> It is used as a universal selectors to select all the elements.
*{
    margin:0
    padding:0
}

an inline style will overdide external and internal styles.

"<#div class="red"></div>
<#div id="red"></div>


                            CHAPTER-2
CSS rule are simple key value pairs with a selectors we can write css rule to change color and set background.
#1-> color property-> color property is used to set the text color inside the element.

p {
    color:red -> this will give the color red to the text. smillalry we can set for the different elements
}

Types of color values:-

1.RGB-> specify color using Red, green, Blue values e.g rgb(200,98,70)
2.HEX code-> Specify using ex code.
           eg. #ff7180

3.HSL--> Specify the color using HSL values (H-Hue, S- Saturation, L-Lightness)
       eg. hsl(8, 90%,63%)
       The values of the color or background color are provided any one of them.

                 For RGB, HEX and HSL write hex color picker on google and you will get the result. from there choose the value of RGB,HEX and HSL and you can apply it.


                 Background Image property
                 .class_name{
                    background: url('location')
                 }
               

               Backgroud repeat property

               1-> repeat-x : repeat in x direction
               2-> repeat-y : repeat in y direction
               3-> no-repeat : image not repeat

               To use the attribute selector to select the <a> element with an href attribute value containing ‘florence’, add the following code to style.css:

                a[href*='florence'] 
                {
                color: lightgreen;
                }
                Notice how only the “Learn More” link in the Florence, Italy paragraph changed to light green.

               Specificity
Specificity is the order by which the browser decides which CSS styles will be displayed. A best practice in CSS is to style elements while using the lowest degree of specificity so that if an element needs a new style, it is easy to override.

IDs are the most specific selector in CSS, followed by classes, and finally, type. For example, consider the following HTML and CSS:


                    Chaining
When writing CSS rules, it’s possible to require an HTML element to have two or more CSS selectors at the same time.

This is done by combining multiple selectors, which we will refer to as chaining. For instance, if there was a special class for <@h1> elements, the CSS would look like below:

h1.special {
 
}
The code above would select only the <@h1> elements with a class of special. If a <@p> element also had a class of special, the rule in the example would not style the paragraph.


                            Descendant Combinator
In addition to chaining selectors to select elements, CSS also supports selecting elements that are nested within other HTML elements, also known as descendants. For instance, consider the following HTML:

<ul class='main-list'>
  <li> ... </li>
  <li> ... </li>
  <li> ... </li>
</ul>
The nested <li> elements are descendants of the <ul> element and can be selected with the descendant combinator like so:

.main-list li {
 
}
In the example above, .main-list selects the element with the.main-list class (the <ul> element). The descendant <li>‘s are selected by adding li to the selector, separated by a space. This results in .main-list li as the final selector.

Selecting elements in this way can make our selectors even more specific by making sure they appear in the context we expect.



                                BACKGROUND SIZE PROPERTY

                        cover-> fits and no empty sapce remains
                        contain-> fits & image is fully visible
                        auto-> display in original size
                        {{width}}-> set width height will be automatically resized according to width.


                        set background position

                        div1{
                            background-position: left top;

                        }

                        The background attached property
                        Defines scrollable and non scroable charater of abackground image

                        div2{
                            background-atachment:fixed;
                        }


                        The background short hand

                        a single property to set multiple background properties

                        div3{
                            background: red url(imag.jpg) no-repeat fixed right top'
                        }


                        Text Align
                    The text-align CSS property can be used to set the text alignment of inline contents. This property can be set to these values: left, right, or center




                    Important
                !important can be applied to specific declarations, instead of full rules. It will override any style no matter how specific it is. As a result, it should almost never be used. Once !important is used, it is very hard to override.

                The syntax of !important in CSS looks like this:

                p {
                color: blue !important;
                }
                
                .main p {
                color: red;
                }
                Since !important is used on the p selector’s color attribute, all p elements will appear blue, even though there is a more specific .main p selector that sets the color attribute to red.

                One justification for using !important is when working with multiple stylesheets. For example, if we are using the Bootstrap CSS framework and want to override the styles for one specific HTML element, we can use the !important property.


                            Review Visual Rules
            Incredible work! You used CSS to alter text and images on a website. Throughout this lesson, you learned concepts including:

            The font-family property defines the typeface of an element.
            font-size controls the size of text displayed.
            font-weight defines how thin or thick text is displayed.
            The text-align property places text in the left, right, or center of its parent container.
            Text can have two different color attributes: color and background-color. color defines the color of the text, while background-color defines the color behind the text.
            CSS can make an element transparent with the opacity property.
            CSS can also set the background of an element to an image with the background-image property.
            The !important flag will override any style, however it should almost never be used, as it is extremely difficult to override.


            Dealing with overflow
If content is too large for its container, the CSS overflow property will determine how the browser handles the problem.

By default, it will be set to visible and the content will take up extra space. It can also be set to hidden, or to scroll, which will make the overflowing content accessible via scroll bars within the original container.



Height and Width Maximums/Minimums
The CSS min-width and min-height properties can be used to set a minimum width and minimum height of an element’s box. CSS max-width and max-height properties can be used to set maximum widths and heights for element boxes.


                                                Borders
A border is a line that surrounds an element, like a frame around a painting. Borders can be set with a specific width, style, and color:

width—The thickness of the border. A border’s thickness can be set in pixels or with one of the following keywords: thin, medium, or thick.
style—The design of the border. Web browsers can render any of 10 different styles. Some of these styles include: none, dotted, and solid.
color—The color of the border. Web browsers can render colors using a few different formats, including 140 built-in color keywords.



Border Radius
Ever since we revealed the borders of boxes, you may have noticed that the borders highlight the true shape of an element’s box: square. Thanks to CSS, a border doesn’t have to be square.

You can modify the corners of an element’s border box with the border-radius property




The code in this example puts 10 pixels of space between the content of the paragraph (the text) and the borders, on all four sides.

The padding property is often used to expand the background color and make the content look less cramped.

If you want to be more specific about the amount of padding on each side of a box’s content, you can use the following properties:

padding-top
padding-right
padding-bottom
padding-left
Each property affects the padding on only one side of the box’s content, giving you more flexibility in customization.


                                    Margin
So far you’ve learned about the following components of the box model: content, borders, and padding. The fourth and final component of the box model is margin.

Margin refers to the space directly outside of the box. The margin property is used to specify the size of this space.

p {
  border: 1px solid aquamarine;
  margin: 20px;
}




div.headline {
  width: 400px;
  margin: 0 auto;
}
In the example above, margin: 0 auto; will center the divs in their containing elements. The 0 sets the top and bottom margins to 0 pixels. The auto value instructs the browser to adjust the left and right margins until the element is centered within its containing element.

In order to center an element, a width must be set for that element. Otherwise, the width of the div will be automatically set to the full width of its containing element, like the <#body>, for example. It’s not possible to center an element that takes up the full width of the page, since the width of the page can change due to display and/or browser window size.

In the example above, the width of the div is set to 400 pixels, which is less than the width of most screens. This will cause the div to center within a containing element that is greater than 400 pixels wide.



                                Margin Collapse
As you have seen, padding is space added inside an element’s border, while margin is space added outside an element’s border. One additional difference is that top and bottom margins, also called vertical margins, collapse, while top and bottom padding does not.

Horizontal margins (left and right), like padding, are always displayed and added together. For example, if two divs with ids #div-one and #div-two, are next to each other, they will be as far apart as the sum of their adjacent margins.

#img-one {
  margin-right: 20px;
}
 
#img-two {
  margin-left: 20px;
}


In this example, the space between the #img-one and #img-two borders is 40 pixels. The right margin of #img-one (20px) and the left margin of #img-two (20px) add to make a total margin of 40 pixels.

Unlike horizontal margins, vertical margins do not add. Instead, the larger of the two vertical margins sets the distance between adjacent elements.

#img-one {
  margin-bottom: 30px;
}
 


#img-two {
  margin-top: 20px;
}
In this example, the vertical margin between the #img-one and #img-two elements is 30 pixels. Although the sum of the margins is 50 pixels, the margin collapses so the spacing is only dependent on the #img-one bottom margin.

It may be helpful to think of collapsing vertical margins as a short person trying to push a taller person. The tall person has longer arms and can easily push the short person, while the person with short arms cannot reach the person with long arms.




                                        Overflow
All of the components of the box model comprise an element’s size. For example, an image that has the following dimensions is 364 pixels wide and 244 pixels tall.

300 pixels wide
200 pixels tall
10 pixels padding on the left and right
10 pixels padding on the top and bottom
2 pixels border on the left and right
2 pixels border on the top and bottom
20 pixels margin on the left and right
10 pixels margin on the top and bottom
The total dimensions (364px by 244px) are calculated by adding all of the vertical dimensions together and all of the horizontal dimensions together. Sometimes, these components result in an element that is larger than the parent’s containing area.

How can we ensure that we can view all of an element that is larger than its parent’s containing area?

The overflow property controls what happens to content that spills, or overflows, outside its box. The most commonly used values are:

hidden—when set to this value, any content that overflows will be hidden from view.
scroll—when set to this value, a scrollbar will be added to the element’s box so that the rest of the content can be viewed by scrolling.
visible—when set to this value, the overflow content will be displayed outside of the containing element. Note, this is the default value.
p {
  overflow: scroll; 
}
In the example above, if any of the paragraph content overflows (perhaps a user resizes their browser window), a scrollbar will appear so that users can view the rest of the content.

The overflow property is set on a parent element to instruct a web browser on how to render child elements. For example, if a div’s overflow property is set to scroll, all children of this div will display overflowing content with a scroll bar.

For a more in-depth look at overflow, including additional properties like overflow-x and overflow-y that separate out the horizontal and vertical values, head over to the MDN documentation.




                            Visibility
Elements can be hidden from view with the visibility property.

The visibility property can be set to one of the following values:

hidden — hides an element.
visible — displays an element.
collapse — collapses an element.


                        <ul>
  <#li>Explore</#li>
  <#li>Connect</#li>
  <#li class="future">Donate</#li>
</#ul>
.future {
  visibility: hidden;
}



Note: What’s the difference between display: none and visibility: hidden? An element with display: none will be completely removed from the web page. An element with visibility: hidden, however, will not be visible on the web page, but the space reserved for it will.


                    Why Change the Box Model?
The last lesson focused on the most important aspects of the box model: box dimensions, borders, padding, and margin.

The box model, however, has an awkward limitation regarding box dimensions. This limitation is best illustrated with an example.

<#h1>Hello World</#h1>
h1 {
  border: 1px solid black;
  height: 200px;
  width: 300px;
  padding: 10px;
}
In the example above, a heading element’s box has solid, black, 1 pixel thick borders. The height of the box is 200 pixels, while the width of the box is 300 pixels. A padding of 10 pixels has also been set on all four sides of the box’s content.

Unfortunately, under the current box model, the border thickness and the padding will affect the dimensions of the box.

The 10 pixels of padding increases the height of the box to 220 pixels and the width to 320 pixels. Next, the 1-pixel thick border increases the height to 222 pixels and the width to 322 pixels.

Under this box model, the border thickness and padding are added to the overall dimensions of the box. This makes it difficult to accurately size a box. Over time, this can also make all of a web page’s content difficult to position and manage.

In this brief lesson, you’ll learn how to use a different technique that avoids this problem altogether.