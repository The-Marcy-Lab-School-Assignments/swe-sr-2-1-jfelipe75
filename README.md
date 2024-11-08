# Technical Writing Assignment

For guidance on setting up and submitting this assignment, refer to the Marcy lab School Docs How-To guide for [Working with Short Response and Coding Assignments](https://marcylabschool.gitbook.io/marcy-lab-school-docs/fullstack-curriculum/how-tos/working-with-assignments#how-to-work-on-assignments).

## Prompt 1

Do some research on semantic and non-semantic elements and share your findings. Your response should include:
* Examples of semantic and non-semantic tags
* The differences between semantic and non-semantic tags
* The benefits of using semantic tags (when possible)

### Response 1
* Semantic Tags
- header
- main
- nav
 * Non-Semantic tags
- div
- span

* The key differences between semantic and non-semantic tags are that while semantic tags provide descriptive names which give us information about its contents, non-semantic tags are not descriptive at all but are great for styling and layout purposes.

* The benefits of using semantic tags are that it's easier to manipulate its contents using JavaScript code since readibility is easier for other developers and also that it's more concise and easier to use to structure our html file.
## Prompt 2

Do some research on accessibility. What are some ways to make your website more accessible? Explain why it is important for developers to create websites that meet accessibility standards.

### Response 2
Some ways to make our website more accessible are by including images and alt descriptions, having functional websites that can be navigated using keyboard if user does not have a mouse, the content should be clear and make use of straighforward language and the website should work well (be compatible) with other assistive technologies. 

It's important for developers to create websites that meet accessibility standards because at the end of the day a website it's a commercial product and we want as many people as possible to be able to use this product in a functional way that adds value to them.
## Prompt 3

It is possible to add "inline" CSS styles to our html elements using the `style` attribute like so:

```html
<p style="color: red;" >hello world</p>
```

While this is possible, it is a best practice to instead write styles in a separate CSS file. Provide at least one argument for why it _might_ be considered useful to write inline styles, and then provide a more compelling argument for writing styles in a separate CSS file.

### Response 3
The only reason I can think of when it comes to styling html elements inline is if you have minimal amount of content and want to avoid having two separate files.

And I believe developers should definitly keep a separate CSS file because that way we first of all improve the readability of our HTML file which should mainly serve as a structure and because we save ourselves tons of time by using selectors and giving them properties in our css that allow us to make custom designs for certain parts, and also the fact that we can use assign styles to our semantic and non semantic tags directly by stating so in our CSS file.

## Prompt 4

Imagine you are teaching a brand new programmer a brief lesson about the `class` and `id` attributes in HTML as well as how to use them to style elements using CSS. Your lesson should have the following components:

* An explanation of the concept of "classes" and "ids" with an analogy.
* An example of the usage using an HTML code block and a CSS code block.
* An explanation of the syntax using the terms: **attribute**, **selector** 

### Response 4

 Think of the major phone manufacturer in the world currently, No one but apple comes to mind. Now to dive in deeper into the topic of what is a class let's think in terms of apple's phone models, we got iPhone 4, iPhone5, iPhone14 pro etc... We know by common sense that there are millions of these operating systems that share the same model floating around the world but we still can identify them by their class which in this case will be their model series, but an Id is something unique, something no more than one person can share so now let's think of "iPhone 15" that belongs to my friend Alex, while there are many other iPhone 15s floating around, your friends phone is only his and is unique in the sense that it's affiliated to a phone number that anyone can use to contact him, his phone also contains information specific to him like pictures, apps, settings, etc... The point is that if I refer to an iPhone 15, there's many out there while if I specify alex's iphone 15 I mean specifically the phone he owns.

 
 ```html
 <h1 id="main-header">Main Title</h1>
 <p class="normal">Normal text</p>
 ```
 Here we have two examples of semantic tags, one refers to the maing heading of the file(h1) and the other one refers to a paragraph element(p). In 'h1' we make sure to speficy that we're working with a unique element by giving it an Id 'id="main-header" and in 'p' we make sure to give it a class that we can pass on to other elements to style them in the same format. class="normal".
 ```css
 #main-header {
    background-color: #4CAF50;
    color: red;
    text-align: center;
    padding: 20x
 }

 .normal {
    color: blue;
 }
 ```
 Here we have a CSS file that refers to the HTML in the previous block. we are refering h1 by calling its Id '#main-header', when calling an id in CSS we must always include a '#' at the beggining of the id. inside of the curly braces that follow after we have all of the styles we wish to apply to our h1. on the left the type of style and separated by a ':' on  the right the values of each style.

 then we have our class '.normal' which we know its a class since it starts with a '.' . Now we know that ids start with a '#' and classes with a '.', we style them in the same way, open curly braces and styles and values on the inside.
 
## Prompt 5

The Document Object Model (DOM) API provides functions for manipulating HTML documents. It is possible to build an entire website using only JavaScript and the DOM API, however is that the best practice?

When building a website, how can I decide which content I should write using HTML/CSS and which content I should create using the JavaScript and the DOM API?

### Response 5

Websites are a combination of text, image, and video content plus functionality, the way users interact with the website is extremely important nowdays since to stay relevant we want non-static websites, the main advantages of reading from the internet rather than reading a document are navigation tools which make it easy to find the content we're looking for and the way it handles user-input giving the illusion of abstraction. When building a website we want to create our main structure using HTML and CSS since it's an straighforward and visual process and makes it easier to read for other developers. We want to reserve the use of JavaScript and the DOM API for when we want to generate dynamic content based on user's interaction with the page, This makes the experience of each user more personal and facilitates the navigation of our website, specially when we're building a big website with many pages and data.