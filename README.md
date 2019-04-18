# Dragon.request(); 

It's like Dragon Quest, but for coding!

## Level 0: Getting Started
Hello adventurer, thank you for choosing this long quest to becoming a front end programmer. We will be coding inside codepen to get started. This has a few caveats:

1. The HTML title attribute `<title></title>` will not show up on the tab or window
2. There is a console button you can use at the bottom of the screen, this will not show any errors, please use the browser's development console instead.

Please sign up for an account at codepen.io and "Create New Pen" 

If at any time your changes are not appearing on screen, please let me know, we'll troubleshoot together.

## Level 1: HTML
### Goal: Create a fan page for your favorite animal.

1. Give your fan page a title
2. Write 3 Headings for your animal
3. Write 2 Paragraphs
4. Add a link to a wikipedia page.
5. Group Headings and paragraphs together in divs
6. Write a list about the best parts of the animal
7. Add 4 images of your animal (for this, please search for the image, right click, copy image address)
8. Emphasize a line of text, and bold another

### HTML Explanation:

#### Level 1 Preface: What is HTML?

HTML (Hyper Text Markup Language) is responsible for the content that is displayed in your browser. HTML is built out of elements that come together to form a page. Each element is created by using tags:

`<tag> </tag>`

Each time you open a tag you must close it. There are some tags that close themselves, but we will talk about those later. To start coding HTML you must tell the browser you are writing HTML. You do this by setting the Document Type, and adding the HTML tag.

` <!DOCTYPE html> <html></html>`

Now you are ready to start!

#### Level 1.1: Give your Fan Page a Title.

HTML pages are separated into two parts, the head and the body, the head is where all the information about the document goes, styling, scripts, title, and metadata (data the that the browser uses to determine the content of the page for search engines). First, add a head to your page by adding that element.

`<head></head>`

Inside the head element, add the title element:

`<head><title>The Very Best Animal Page on the Internet</title></head>`

The content of an element is placed between the opening and closing tags . Always close your tags when you are done putting content in!

Now your page has a title. From now on, all the elements you will be using today will go inside the `<body></body>` tag of your page which goes right after the head, look to the right to see the ideal structure for your page.

#### Level 1.2: Write 3 Headings for your animal

One of the most important content items are headings, these are the large texts that inform the user what the paragraph or content below might be, headings start at 1 (the largest) to 6 (the smallest). 

`<h1></h1>`
`<h2></h2>`
`<h3></h3>`
`<h4></h4>`
`<h5></h5>`
`<h6></h6>`

#### Level 1.3: Write 2 Paragraphs about your animal.

A paragraph tag is just `<p></p>` and you should be a pro at putting content into your elements by now!

#### Level 1.4: Add one link to wikipedia 

A link tag introduces the idea of an "attribute" to the element, specifically the `href` attribute. Attributes tell us extra information about the element and AWAYS go in the starting tag. You must use double quotes around the value (what comes after the equals) of the attribute

` <a href="http://google.com">Go to Google</a>`


#### Level 1.5: Group together the paragraphs and headings into div's

The most useful thing in HTML is the `<div>` tag, short for "division" this is how you can group elements together to later arrange, and style them the same. It helps break the pages into boxes that you see in most modern websites. Put all the content you want together inside a div element.

`<div></div>`

#### Level 1.6:  Write a list about the animal's best features.

We did some nesting earlier, and now we're going to do even more. There are two types of lists that are fairly common: ordered lists, and unordered lists. 

Ordered lists are lists that numerate for each line. The code for an ordered list looks like this:

`<ol><li>Step 1</li><li>Step 2</li></ol>`

Notice that there is an element `<ol>` this element determines what type of list it is ol is short for Ordered List. Inside the list, there is an element for each List Item `<li>` you cannot have list items outside of a list. That would be madness.

The other list type: Unordered list, looks like this.

`<ul><li>Bullet 1</li><li>Bullet 2</li></ul>`

#### Level 1.7: Add 4 Images of your animal

An image tag is a self closing tag. This is rare! Enjoy it for what it is. 

However, an image also has many attributes (do you remember those from links before?). The "source" (src) of the image which is a direct link to that image file, and the alternative (alt) to that image, which is text that will describe the image.

` <img src="http://url-to-image/image.png" alt="image description">`

"Why alt text!" You might ask. There are two reasons:

1. Better Accessibility for the blind (it can read the image out to them)
2. You can put really funny jokes in the alt text and if you mouseover the images it shows it, and that's the only reason I need.

#### Level 1.8: Emphasize some text, bold another.

`<em></em>`  is short for emphasis
`<strong></strong>` is how you get bolded text.

There are a lot more HTML elements out there! If you're curious to see what else you can add before you move onto CSS, read the docs on w3schools.

## Level 2: CSS
### Goal: Make this fan page look readable.

1. Change the background color to your favorite color
2. Change all the paragraphs to Helvetica
3. Change the picture width to 250px
4. Go back to your html and pick a div and add a class
5. Style that class with a background of black and a text color of white
6. Remove the list style
7. Change all links to be a different color than default
8. Target the first li of your list and make the background blue
9. Add percentage padding and margins to all divs.
10. BONUS TIME: Spend however long you want customizing it to look right, you can generate gradients, or pick color palettes, or set the background to be an image.

#### Level 2: Preface.

CSS is what makes the web beautiful. While HTML is how you get content, CSS is what styles the content. In fact, CSS stands for Cascading Style Sheets.

The C in CSS is the most important part. Whatever is defined last in the stylesheet is the style that will be applied. When CSS is parsed it goes down through, like a cascading waterfall, and picks up the last style to apply.

CSS styles are structured all the same

`selector { property: value; }`

Elements like p, h1, and img are all styled this way. Later on, we will get into classes, and IDs which make it possible to style only particular html elements on the page.

#### Level 2.1: Change the background color to your favorite color

Remember the `<body>` tag from the first step of HTML? You can use this to style anything that is enclosed inside the body. This is pretty convenient for setting styles that are on the whole page.

`body { background-color: AliceBlue; }`

This will change the background color. There are two big ways to deal with colors in CSS: color names, and hex codes. Both are acceptable.

#### Level 2.2: Change all the paragraphs to Helvetica

` p { font-family: Helvetica, Arial, sans-serif };`

This CSS element includes fallbacks for different browsers, which is why three fonts are defined. If a user has Helvetica, use it, if they do not, try Arial, if they do not, any sans-serif font will do.  You can try with other fonts in your system as well.

#### Level 2.3: Change the picture width to 250px

`img { width: 250px }`

You can set the height similarly, and there are many different ways to measure the width an height, try with percentages if you're feeling up to it!

`img { width: 50% }`

#### Level 2.4 Adding Classes and IDs

What if we want one paragraph to have green text and another paragraph to have blue text? Introducing Classes and IDs, these are HTML attributes that we can use to differentiate different elements from one another.

Classes can be used multiple times, and can be used in mutiples, an HTML can have multiple classes, just like you can attend multiple classes at a school, and multiple people can attend that class. 

Pick a div and add a class to it.

`<div class="firstClass">`

To add a specific style to this class, we create a CSS selector for that class, like so:

` .firstClass { color: white; background-color: black; }`

Notice the period in front of the selector? This is how CSS knows that you mean a class instead of an element like <div>.

IDs are different than classes, they can only be used once per page. IDs are a way to distinguish elements from one another. They must be unique for purposes later. 

`<div id="firstID">`

To style it:

` #firstID { background-color: red }`

Notice the # sign in front of the selector? This is how CSS knows that you want to style an ID.

An element can have both a class and an ID.

`<div class="firstClass"  id="firstID">`

#### Level 2.5 Remove List Style

￼`ul { list-style:none; }`

#### Level 2.6: Change all link colors to be something other than default

`a { color: pink; }`

#### Level 2.7: Target the first list item in your list and make the background blue.

There are two ways you can handle this: pseudo-classes and classes. We will go over both. 

First, you can add a class to your list item.

`<ul><li class="blueBackground">Item 1</li><li>Item 2</li></ul>`

Then you can use multiple selectors to target only the list item that has the class blueBackground.

`li.blueBackground {background-color: blue;}`

The selector is literally any li element with class (.) blueBackground. 

The second, and more difficult way is to use pseudo classes. These are invisible classes that HTML appends to elements. Here is a list of them, you can get really crazy with them.

`ul li:first-child {background-color: blue}`

This says in the ul element, chose the first-child element (nested element) that is an li, and change the background to be blue.

#### Level 2.8: Add percentage padding and margins to a div.

Let's go back to our style for our "firstClass" with a background of black and first let's add a margin. 

`.firstClass { background: black; color: white; margin: 5%;}`

You may notice we used percentage instead of pixels. In the modern web, we shy away from pixels because every device has a different number of pixels. Your phone has less than your computer, for example, but we don't want a webpage to be broken on one and not the other. So we use percentages to make sure it takes up the same percentage on all screens.

Secondly, there seems to be more space around the black box, but not inside of the black box. This is because margin is outside of the content, like wearing bulky clothing around the element.

Let's add some padding and see what the difference is.

`.firstClass { background: black; color: white; margin: 5%; padding: 5%;}`

You will see now that the black box itself is bigger and has more space around the text. This is because padding adds space inside the element. It may be a good time to review the [CSS Box Model](https://www.w3schools.com/css/css_boxmodel.asp) in order to best understand how css applies to elements.



## Stylish Sidequest: Making Your Site Modern
### Goal: Make it actually look like the ~modern~ web

1. Install [Bootstrap · The most popular HTML, CSS, and JS library in the world.](https://getbootstrap.com/)
2. Add a div with ID of "header" and give it a background image, make it sized to "cover" and a fixed height of 800px
3. Inside this div add an h1 of the site's name
4. Add a bootstrap button and have it jump to the first heading of your site (hint: give the header an ID also, and the link for the button will be `#<<HeaderID>>`)
5. Put all your content in a container
6. Put one heading in a row
7. Put the other two headings and two paragraphs in a different row.
8. Split the two headings and two paragraphs into col-md-6
9. Put your list in another row, with a column offset of 6
10. Add some other bootstrap fanciness, pick some components and drop them in your site where needed.
11. Add a menu on top and have it scroll the same way the button did in step 4.
12. BONUS: Make your site responsive! (Col-md vs col-sm, why px width is bad,  and percentages are in!) 


## Level 3: Javascript
1. Write a console log haiku (3 console logs, one line each, 5, 7, 5:  `Yesterday it worked, Now it is not working, Coding is like that`  ( write your own sweet haiku, don't steal mine)
2. Create a function that takes in a mood, and console.log's the following statement: "Currently Feeling:"  (you can also put, currently listening to, or currently eating, or something similar) 
3. Write an if statement in the feeling function that takes in a mood and outputs a color. (ex. If mad, then return ‘red')
4. Write an array of your favorite animals, bands, or video games, sort this array,
5. Execute a for loop on this array that console.log's each array item out.
6. Create a button on the website that appends the favorite's array to a paragraph
7. ACTUAL BONUS: write a text input that takes in a "mood" and when submitted changes the background color of the website for the color associated with that mood.

#### Level 3 Javascript:

Javascript is very much the language of the web. It is used to make your page become dynamic, it turns static content into computed content, and is what the modern web is built on. 

I have a lot of opinions on javascript, and there's a lot of ways to go about javascript, but for now, please shut out all the noise about javascript and follow my lead. We'll get to the opinions later.

Going into this know the following things: 

1. Javascript takes time to learn
2. Javascript is a real programming language (TM)
3. Javascript can be very finicky, and you will get a lot of errors to start with.

Please do not be discouraged! You can do this!

#### Level 3.1: console.log Haiku.

If you are on chrome you can access the console by going to `View > Developer > Javascript Console`
 
Inside your javascript files write your console.log() function

`console.log(‘hello');`

You should see hello outputted to the console.

Hello must be put inside two single quotes to tell javascript that this is a string of characters and must be used literally. You do not need to do this for a number:

`console.log(4);`

If you do not put single quotes around a word, Javascript thinks that this is a variable. A variable is a reference object that can hold anything else.

`var greeting = 'hello'; console.log(greeting);`

A variable must be prefixed with `var` in order for javascript to know this is a new variable, if you are not making a new variable, but just changing the value (this is called reassignment), it does not need to be prefixed with var.

` var greeting = hello; greeting = hey; console.log(greeting)`

The console will say hey, instead of hello.

Write your haiku by defining three variables, line 1, line 2, and line 3, and console.logging out those variables.

#### Javascript Level 3.3: Create a function that takes in a mood, and console.log's the following statement: "Currently Feeling:"

If you want javascript to do something at a particular time, or if you want javascript to do a few somethings all at once, you must create a function. Just like when defining a variable, you must define a function similarly:

` function feeling() {};`

The feeling function is now defined, go ahead and add a console.log inside this function.

`function feeling()  { console.log('Currenting Feeling:')};`

After the function is defined you have to call a function to execute it

`feeling();`

It should print something out in your console now.

The next step is to pass a variable into the function, let's first create a variable for our mood and then pass it through:

``` javascript
var definedMood = 'happy';
function feeling(mood) {
console.log('Currenting Feeling:')
console.log(mood);
};

function(definedMood);
```

Notice that any variable we want to pass to the function goes between the () in the function, you can pass multiple variables into the function as well by adding a comma

``` javascript
var definedMood = 'happy';
var definedColor = 'green';
function feeling(mood, color) {
console.log('Currently Feeling:');
console.log(mood);
console.log(color);
};

feeling(definedMood, definedColor);
```


#### Level 3.4 Write an if statement in the feeling function that takes in a mood and outputs a color. (ex. If mad, then return ‘red')

If statements are the first logic operators you will have in javascript, and can get complicated very quickly. First, we must understand equality in javascript to move forward. 

*Not All Equals are Equal*

1. Never use a single equals in a logic (if) statement, single equals (=) is used for variable assignment!
2. Double equals is more common (==) when you want to compare values (‘2' == 2)
3. Triple equals is to check memory reference, and is very strict, it is the strictest of all equals! (===) the preference of triple equals is so code doesn't break as often, but you'll find sometimes it's hard to deal with.

We will use double equals for now.

``` javascript
var definedMood = 'happy';
function feeling(mood, color) {
  if (mood == 'happy') {
  console.log('I am happy because this is working');
  }
};

function(definedMood);
```

If the if statement is true, it executes the code.

There are many comparison operators you can use in an if statement (==, !=, <, >, etc).

#### Level 3.5: Write an array of your favorite animals, bands, or video games, get the length of the Array.

An array is just a collection of objects, strings, or other things. You can access any individual item in the collection by it's index, or place in the array. 

`var Array = ['item 1', 1, ['sub-array1', 'sub-array2'], ‘string']`

As you can see, an array can hold anything.

You can access any item in the array by using it's index:

`Array[0]`

This will get the first item in the array. An array has many methods ([JavaScript Array Reference](https://www.w3schools.com/jsref/jsref_obj_array.asp) ) you can use to modify or access the items in an array.

`Array.length()`

Will get the length of the array.

Try a few of the methods and see how it mutates your array!

#### Level 3.6: Execute a for loop on this array that console.log's each array item out.

A loop is a code that runs over and over until it runs out, it can be infinite (unfortunately for your computer) or finite.  There are a few kinds of loops: for and while are the most common types of loops you will see in Javascript.

``` javascript
for (i = 0; i < 5; i++) {
  text += "The number is " + i + "<br>";
}
```


The for loop above takes three statements. The first statement `i = 0` is executed one time before the loop starts. The second statement ` i < 5` is the condition of the for loop, it is how we prevent infinite loops from happening. It says, as long as I is less than 5, go ahead and run. The third statement `i++` is run every time the loop runs, in this case, it add's 1 to i each time. 

Using this knowledge, execute a for loop on your array using the method array.length() to set the second condition, and console.log out every item in the array.

``` javascript
var arrayLength = myStringArray.length;
    for (var i = 0; i < arrayLength; i++) {
        console.log(myStringArray[i]);
    }
```


#### Level 3.7: Create a button on the website that appends the favorite's array to a paragraph

Create a simple function that execute's a console.log first:

`function clickButton() { console.log(‘button clicked')};`

In your HTML you can create a simple button that executes this function when it is pressed: 

` <buttononclick="clickButton()">Click me</button>`

You should be able to see the output in your console every time the button is clicked.

To append this to the HTML you need to start manipulating the DOM, this is what the HTML is called in programming terms, the Document Object Model. Your HTML page, is the document and you can access it in javascript by using the document method.

` var para = document.createElement("p");`

This is the createElement method and will create a new paragraph at the top of your page, but it's empty! We need to put something inside of it. You can extend this method by adding the `innerHTML` method:

` para.innerHTML="This is a paragraph.";`

Lastly, you can stack document methods together with document element methods like so:

` document.getElementById("myDIV").appendChild(para);`

A good look at the document methods will give you the tools needed to do the bonus question!

## Level 4: I want to be a RealDev(TM) and Set up my Environment

In this section we will set up the following tools:

1. Github
2. How tf do I use command line?
3. Choose your text editior (DANGER: OPINIONS AHEAD)
4. The developer console on chrome (what is it?)

### Part 1: Github

Sign up for an account on GitHub, and if you are on windows install the git client (not Github for desktop, please do not cheat).

Create a new repository and write something in the README file in the browser, clone this repository with the command `git clone`  onto your desktop.

Open the readme file in notepad and change one line, go through the basic git workflow

`git add`
`git push`
`git pull`

You can follow this simple guide [git - the simple guide - no deep shit!](http://rogerdudler.github.io/git-guide/) for now.

### Part 2: Command Line
[Bash Cheat sheet](https://learncodethehardway.org/unix/bash_cheat_sheet.pdf) 

You NEED to learn this, I am sorry, you can only dodge it for so long, you don't need to be fluent, but you should learn the basic commands: cd, ls, mkdir, tail, etc. Use a cheatsheet for now if you must, but it is imperative that you become somewhat comfortable opening up your terminal.

### Part 3: Your Text Editor.

I use [Atom](https://atom.io/) because I love Open Source Software, if you don't, you can use [Visual Studio Code](https://code.visualstudio.com/), if  you're stuck in 2014, then you can use [Sublime Text ](https://www.sublimetext.com/).

If you have infinite time on your hands and need something to argue about, go ahead and learn vim (honestly I think everyone should learn a bit of vim to start with, in case you need to get into things hosted on your server).

[VIM Adventures](https://vim-adventures.com/)

If you use emacs, if someone told you to use emacs, exit the guide. The e in emacs stands for ego. 

### Part 4: The Developer Console.

This is your best friend, you can edit css in it, you can diagnose errors in it, you can find hidden things in it. Please get used to it, it will be your only true friend going forward.

## Level 5: JS-Rogue: Writing your first framework based app with Vue.js

#### Level 5: Patterns, and how it factors into your life

Now that you are getting into more complicated Javascript it's time to take a step back and look at architectural patterns. The biggest ones that you will hear about in your time with javascript are: MVC and MVP 

MVC - Model - View - Controller

This is the easiest to understand, because you already have done it! The Model for the data is HTML, the View is CSS, and the Controller is the Browser.

Model - HTML - data that is structured in an easy to manipulate formate

View - CSS - Styling that can easily be swapped in and out without changing the model, but affects how the user sees the data.

Controller - Browser - Renders the HTML and CSS and can manipulate or control the content.

MVP - Model - View - Presenter

The difference between MVP and MVC is where the logic is held. In the Controller, the browser and the user can manipulate and control the rest, in the Presenter, it is a passive component that only displays while the View allows for information to be passed back and forth from the presenter and the model.

Another important pattern is called the State Pattern. The State pattern is an idea that there is a single point for all the important data in the application that affects how the components display or work. When the state is updated, the components change.

You don't have to really "understand" this to work with Javascript, you will see these come naturally out of the frameworks you are using. Keep these ideas in mind as you're coding.

#### Level 5.1: Learning a Framework (Under Construction)

There are a lot of feelings about frameworks, but the only true feeling I have is that I do not want you to learn jQuery. It becomes a crutch for the rest of your time in Javascript and it's hard to break out of it. I've chosen Vue temporarily as the modern framework I would like you to start learning. I will update this in the future to talk about The Big 3(tm) (Angular, Vue, and React) and how they factor into your life:

The “path” you take will determine very little, you can move from framework to framework with ease, so if you get started with one, don’t think that you have to be with that framework forever. Vue is easier to start with but at a later time I will add React (my home framework) as well. It is important though to note that once you start with a framework, learn it all the way through, don’t switch off midway.


#### Level 5.2 - Vue.JS and You.JS

[Build A Movie Player with Vue.js](https://scotch.io/tutorials/build-a-movie-player-with-vuejs-solution-to-code-challenge-5)
 
 [Animated Image Search](https://scotch.io/bar-talk/build-an-animated-image-search-with-vuejs-solution-to-code-challenge-8) 
 
 [Marvel Search Engine](https://codeburst.io/marvel-api-vuepack-vue-vuex-c84067a7f7fc) 


## Level 5: JS-Mage: Getting serious with Canvas
[Getting Started With The Canvas API - Treehouse Blog](https://blog.teamtreehouse.com/getting-started-with-the-canvas-api)

[Making Sprite-based Games with Canvas](https://jlongster.com/Making-Sprite-based-Games-with-Canvas)

## Level 5: CSS-Bard: SASS, Animations, and Variables
[Getting Started with SASS (with Interactive Examples) ― Scotch.io](https://scotch.io/tutorials/getting-started-with-sass)

[Animated Animals in CSS and SVG | Codrops](https://tympanus.net/codrops/2016/03/21/animated-animals-css-svg/)
