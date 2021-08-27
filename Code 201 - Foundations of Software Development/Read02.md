
# intro-html-css-js
Introductory presentation project to learn some Html, CSS, and JavaScript


# Workshop Steps

This workshop is intended to compliment an in-person Nexul Academy mentor demo.

Each step of the workshop is contained in commits to this repository, so you can see the exact lines of code that changed. You can see all the commit steps or follow the links in each step.

[All commits](https://github.com/MasteRminD6666/reading-notes/commits/main)

## Step 1: Starter Html file

Web pages are defined with Html for content and CSS for style.  Start by creating a file with the 'html' extension. Then build the most basic of documents with a single
heading (use the 'h1' tag) and a paragraph element (use the 'p' tag).  Refer to the instructor demo.



## Step 2: Html 'Inline' style

Styles include colors, borders, shadows and much more. The most basic way to add styling to an HTML document is with 'inline' styles, using the 'style' attribute on the element to be styled.  Add a color of red to the paragraph, referring to the instructor demo.


## Step 3: Style in Html 'head'

Style can quickly complicate an Html file if applied on many elements using the Style attribute. Move the style to the 'head' of the document using a 'style' element. The style is similar to the following:

    p {
      //your style here
    }
    otherElement {
      //some other style
    }

Compare your answer to commit 

## Step 4: Narrow style to element 'id' selector

Usually, styling all elements of a specific type in the same way is undesirable. The other extreme is styling a single element by referencing an 'id' attribute on the element.  Add an id attribute to the paragraph.

    <p id="special">
    
Now a #special selector is available for use in your css.  Update the selector and then compare your answer to commit ['Step004'](https://github.com/NexulAcademy/intro-html-

## Step 5: Narrow style to class selector

A balance is needed to target many instances of an element type, but not all of them.  A common way to do this is using the class selector.  First apply a class attribute value to the element (instead of an id).  Then use the class selector syntax to style the paragraph.

    .special {}
    
Compare your answer to commit 

## Step 6: Narrow style to a specific hierarchy

Usually context matters, such as a paragraph in a sidenav area may be treated differently than a paragraph in the main content area of the page.  CSS rules can target specific element hierarchies for custom rules.

Place a paragraph inside of a div element and another leave as a direct child of the body.  A CSS rule targeting a hierarchy contains both parent and descendent selectors with a space between them.

    selector1 selector2 { }

To target only direct children of a parent element, use a greater than sign between the selectors.

    selector1 > directChildSelector { }

Use these rules to style only the paragraph inside of the div. Compare your answer to commit 

Using a combination of these selector types can conflict with one another. If multiple selectors change different attribute values, then all rules win and will be applied. When two styles affect the same attribute of an element, only one can win. 'Specificity' rules determine the winner. Refer to the Specificity diagram in the Resources section below for details.

## Step 7: Style moved to separate file

Adding numerous styles to an html document can lead to harder to maintain code and prevents sharing the same style code between html pages.  Style is preferably defined in separate CSS files and then referenced by the HTML file. Create a file with the '.css' extension in the same folder as the html file.

Import css into an html file using the link tag in the document header.

    <link rel="stylesheet" href="...">

Compare your answer to commit 

## Step 8: Introducing the 'Bootstrap' style framework

You can leverage one of many CSS frameworks in your page by linking to them with a style tag.  Download the Bootstrap library from the references section below, place it into the same folder as the html file and import it similar to the last step.

Compare your answer to commit 
## Step 9: Creating a Bootstrap grid layout

Bootstrap is a CSS framework that includes a grid layout system and numerous widgets, with extensions by the development community. Refer to the Bootstrap grid system documentation to build a row of content containing two equally sized side-by-side sections (columns). You will need to place the header in a row above the content row.

Compare your answer to commit 

## Step 10: Bootstrap 'card' widget

Bootstrap has many widgets, one of which is a card. Refer to the Bootstrap cards documentation in the Resources section below.

Replace the two equally sized side-by-side columns content with a card in each, with each card containing the paragraph that was already in each column.

Compare your answer to commit 

## Step 11: Introducing JavaScript

JavaScript is the logic of the application. JavaScript can be added to the head of a document with the 'script' tag, or it can be referenced from an external file.  Let's begin with some code in the html document. 

The most simple JavaScript code to write shows an alert message on the screen.

    alert('Hello World!');

Compare your answer to commit 

## Step 12: Grabbing elements from JavaScript

A common task in JavaScript is to grab an element and do something with it.  You can do this with the 'document.getElementById()' function.  Create a new element in the html with id of 'dynamic', then using JavaScript grab it and write it the the debug console.

Compare your answer to commit 

## Step 13: Defering execution until Html is loaded

If you run the last step in the browser you will notice no element is written to the console. JavaScript runs immediately when parsed by the browser, even before the entire page has finished loading.  So script at the head of the document runs before the body exists, resulting in no element found.

Moving script to the end of the body could be one solution, but it doesn't necassarily guarantee the browser has finished rendering all that was downloaded before the JavaScript compiles.

A better solution is to still run code immediately, but the code should instead register with the load event of the page to defer execution of the element selection logic until the document is downloaded, parsed and ready to use.  The browser DOM supplied an event called "window.onload" for this purpose.  Implement the event and move the element selection logic inside the event block.

Compare your answer to commit 

## Step 14: JavaScript moved to separate file

You can move JavaScript to an external file, similarly to CSS. However scripts are imported using a different tag, called 'script'

    <script src="..."></script>
    
Move the script into a separate file in the same folder as the html file. Compare your answer to commit 
