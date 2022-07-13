# CSS_File

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

<div id = "first" class  = "c1 c2 c3" >
</div>

<div id = "second">
</div>

<section class = "red bg-blue">

</section>

here "first" is a unique id
and c1,c2,c3 are multiple classes followed by spaces.
* multiple elemet can have one class.
* One element can have multiple classes.

-> There are 3 ways to add CSS to HTML.
<!-- 1. <style> tag-> Adding <style> </style> to HTML-->


1) By using <style> tag in HTML between <head> tag and <title> tag we can use id which we give and open curlie brackets and give contents and agaian we close it by curlie brackets.

WE use " # " for targetting(calling elements) " id " and we use " . " for targetting(means calling class) class 
Syntax:-

#id_name{
    background-color: white:
}

.class_name{
    backgroud-color: white;
    color: white; means whatever we wrote inside that background we got that text in white color.
}

<!-- 2. Inline CSS-> Adding CSS using style attribute. -->

where we can write <style> tag inside our <div> tag folowed by background color(check index2.html file)


<!-- 3. External CSS -> Adding a style(.css) to HTML using <link> tag.  --> 

we add <link> tag between the <tittle> tag and <head> and we work according to that.

<!-- #CSS selectors:- -->

A CSS selectors is used to select an HTML elements for styling.

where body { 
    color : red; --> declaration(property:value)

    background:pink --> declaration}

  #here "body" is known as selectors.




