# Introduction to HTML, CSS

## Topics of the day.

1. Introduction to the web(languages on which mostly all website rely on).
2. Difference between HTML, CSS & JavaScript.
3. Introduction to HTML.
4. Elements, Tags, Attributes.
5. Setting up standard HTML Document structure(doctype, html, head, body).
6. Self Closing Elements
7. Nesting and Indentation
8. Introduction to CSS.
9. Selectors, Properties, Values
10. Types of Selectors(Type, Class, ID).
11. Referencing CSS.
12. Semantic overview
13. Non Semantic tags
14. Block vs Inline (div, span)
15. Text-based elements.
16. Creating hyperlinks (Relative & Absolute Paths, Linking to an Email Address, Opening Links in a New Window, Linking to Parts of the Same Page)
17. Building structure with semantic tags (header, nav, article, section, aside, footer, etc.)

## 1. Introduction to the web.

Let's get started with how does a website is built? Most of the websites are run by only three languages(HTML, CSS & JavaScript). It can be said that these three are building blocks of any website. Okay, let's see practically, just open any website of your choice, and right click on a page you will find an inspect option, click it. Once it is clicked you will find some piece of code is open in an inspector window.

Mostly all the websites rely on these three languages. At the time of developing it can be written in any languages, but when it comes to the browser you will find these three languages.

Now let's see the role of these languages one by one and how they are being used to build a website. We will see how they are related to each other and what's the difference between them.

## 2. Difference between HTML, CSS & JavaScript.

These languages are closely related to each other but entirely different from each other. Each of them is designed for a specific task. And our goal is to understand their interaction with each other and how they work individually.

Now let's see them individually. But yeah before going one by one let's make a note of an important point i.e. HTML & CSS are not considered as a programming language. HTML is considered as a markup language, which is solely responsible for the content part in a page. CSS is just the styling information of the content. But yeah JavaScript is considered as a true programming language.

HTML(Hyper Text Markup Language) marks up the raw content with an exact meaning and provide a simple structure to a website.

CSS(Cascading Style Sheet) styles or format those marked up content.

JavaScript provides interaction to those styled and marked up content.

That's the real difference between HTML, CSS & JavaScript. And it should always remain like that only.

With the understanding of the difference between them, its time dig more about them. Of course, we will get started with HTML & CSS part. Once the HTML & CSS part is done then the time will come to start the JavaScript part. Okay then let's get started with HTML.

## 3. Introduction to HTML

As of now, we have a little bit idea of the role of HTML. We also know it is a markup language. But the question is why it is considered as a markup language, not a programming language? To answer this question, first of all, let me tell you, whatever kind of content we see on a page, it can be anything maybe a paragraph or an image, or a video or a button or anything, to show all these types of content in a browser, HTML is responsible. To see any kind of content in a page we will have to send through HTML only. We need to wrap the content inside HTML, only then the browser will understand what kind of content you are sending. This wrapping the content inside HTML is known as markup. Okay, let's take an example to make it more clear.

Just consider an article in a newspaper. If you have been asked just mark up each and every section in the article. Obviously, you will start from the top, for heading section, you will say it as a heading, then some paragraphs, if there will be any image you will say it as an image, then again maybe few more paragraphs, or maybe some quotes inside the article. I will also do the same thing. That's exactly what HTML does. HTML mark up every type of content with the help of elements, tags, and attributes available inside it. So, whatever kind of content we want in a page, we will mark it up with the help of available elements and tags in HTML.

## 4. Elements, Tags, and Attributes.

Now we all know how the content is displayed in a page. We also saw how the content is marked up in an article. Exactly, to markup different kind of content in HTML we use a different kind of elements. For e.g.: for a paragraph, we have a 'p' element, for an image we have 'img' element, for an article we have 'article' element. We have lots of element based on kind of content, we have div, section, header, nav, button, etc.

### Elements

Elements are the basic building blocks of HTML. Let's see one of the most common element used in HTML

```
  <p>Introduction to HTML & CSS</p>
```

The above code is for a paragraph element, wrapping the content 'Introduction to HTML & CSS'. Let's break it down.

Here 'p', is the element name.

### Tags

Once we wrap the element name in between the less than and greater than, angle bracket then it becomes a tag. Tags mostly appear in a pair of opening and closing tag.

Opening Tag, from where an element begins. It contains element name in between less than and greater than angle bracket. For example, `<p>`
Closing Tag, this is where an element ends. It is similar to opening tag only except it contains forward slash before the element name. For example, `</p>`

In between the opening and closing tags our content comes. For example, 'Introduction to HTML & CSS' is our content.

### Attributes

An element may consist of attribute also. Attributes provide some extra information about the element, which actually doesn't appear as content in a webpage. Let's see an element which always appears with an attribute.

The <a> tag defines a hyperlink. The href attribute specifies the URL of the page the link goes to:

```
<a href="https://google.com/">Google</a>
```

An attribute always comes within the opening tag after the elements name. It has a name and value. Here in this case 'href' is the name and 'https://google.com/' is the value.

Few more common attributes are 'id' attribute, which identifies an element, 'class' attribute which classifies element, 'src' attribute which specifies the source of embedded content.

Example for Elements: div, section, img, span, strong and many more. The list is really long. No worries as we move further will cover everything.

## 5. Set up HTML Document structure(DOCTYPE, HTML, head, body)

Now we got the basics of HTML, like what is element, tags, attributes, and how we markup any content. Let's put the things together and create our first web page. For that, we need to set up an HTML document.
HTML documents are simply a plain text editor saved with a .html file extension. Okay let's create a folder and open it in a text editor, it can be any either sublime or vs code or atom whatever you prefer. Create a file inside the folder and save it with .html extension. Let's start the coding part now

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <title>Hello World</title>
  </head>
  <body>
  </body>
</html>
```

The above line of codes is the standard HTML document structure, which you'll require every time, whenever you'll create a new page or a new document. This is the required structure. Let's break it down

### !DOCTYPE html

This is the document type declaration, which informs the browser which version of HTML being used and it is always placed at the beginning of the HTML document. There are a number of HTML version, for example, HTML, HTML 4.01, XHTML, HTML5, etc. HTML5 is the latest version. Because we are using the latest version so simply we will declare, `<!DOCTYPE html>`. For a different version, there is a different declaration.

### html

It signifies the starting of the document. From here the real html document starts. It is also known as the root element of the document. So whatever things we will need to create a page, everything will be coming inside the html i.e, `<html></html>`. So, inside html tag we have `<head></head>` and `<body></body>` elements.

### head

Head stores the extra information on a page. For example, the title of the page, metadata(another extra information on the page). Here we have 'Hello World' as the title of the page. `<meta charset="utf-8">`, this tells the character encoding of the page. There are many more tags which comes inside the `<head>` element, we will see as we move further. One of the important point to note here is, whatever comes inside `<head>` element won't be visible in the page.

### body

All the visible content will come inside `body` element. So whatever we would like to see on a page, will keep them inside the `<body></body>` tags.

Okay, now it's time to open the HTML document in a browser. Once you open the document, I am sure you won't see anything on the browser. Because there is nothing inside the `<body></body>` tags. Let's write something inside it.

```
  <!DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="utf-8">
      <title>Hello World</title>
    </head>
    <body>
    <h1>Hello World!</h1>
    <p>Our first web page.</p>
    </body>
  </html>
```

Now after saving your document again, if you refresh your page you'll get to see something. Yes! that's exactly how we put content in a page. Here we have, `<h1>Hello World!</h1>`, working as heading element and `<p>Our first web page.</p>` as a paragraph element.

## 6. Self Closing Elements

If you recall, earlier we have discussed that elements always appear in a pair i.e. with an opening tag and closing tags. But, in the previous code snippets have a look of 'meta' tag, you won't find any closing tag. These type of tag is called a self-closing tag. There are some elements which don't require to close. They simply get their content from the attribute within a single tag.

## 7. Nesting and Indentation

When an element is placed inside another element known as nesting. Here if you look closely in the above line of codes, you'll see that the `<head>` and `<body>` elements are in between the opening and closing tag of html elements. This means that the head and body elements are nested inside the html elements. When any elements are nested inside other elements we also say parent and children relationships. In our case head and body are the children of html elements. And to keep the code more organized and legible and also to differentiate between the child and parent we use indentation. Indentation is just placing some amount of space to the children from its parents. It can be 2spaces or 1 tab depending upon programmer to programmer.

## Answer the following question

1. What is the role of HTML?
2. What is CSS?
3. Which one them(HTML, CSS, JavaScript), is really considered as a true programming language?
4. What's the difference between HTML, CSS & JavaScript?
5. What are the building blocks of HTML?
6. What is the role of attributes? Is it necessary to place inside every tag?
7. With the help of an example, describe elements, tags, and attributes.
8. All the visible contents should go inside which tag?
9. What is the self-closing tag? Explain with an example.
10. Why do we indent tags? Is it a good practice?

## Do the exercise 1.

## 8. Intro to CSS

Now that we know how to put content in a page, means we have the basic idea of HTML. Like, what are elements, tags, attributes, how to set up an HTML document? Mostly what happens, when we start putting out the contents on a page, automatically our content gets layered out one by one from top to bottom. But the question is do we really want to see our page in that way? Do we really want to keep the structure of the page that much simple? Obviously not, there must be some style to the page, maybe different background color for different sections, different font-size for heading and paragraph. Let's take an example, suppose you build a house, there are different rooms. But, do you leave the walls simply without coloring it, no. It's just you created the simple structure and now for styling, you apply different colors on different walls.

To create the simple structure of the page, we use HTML and in a similary way for styling purpose, we use CSS(Cascading Style Sheet). It can be said that if HTML is drywall then CSS is beautiful paint on the walls.
So to style any element in CSS we need to target that particular element and define what property of the element need to be styled. And for this purpose, we have, selectors, properties and values in CSS. Let's see how all these things work.

## 9. Selectors, Properties, and Values.

For example, suppose we want to change the color of the heading and the size of the font, of the page we have created just a few minutes ago. How we will target the heading in CSS and define styles within it? Let's have a look

```
 h1 {
	color: red;
	font-size: 34px;
}
```

### Selectors:

Here 'h1' is working as a selector. In this way, we target an element within a CSS. There are different ways to target any element but yeah first let understand the above code snippet fully then we will move further. So, once an element is selected then its style can be defined inside the curly braces i.e. `{.......}`.

### Properties & Values:

Here 'color' & 'font-size' are the properties of the element we targeted and 'red' & '34px' are the values. Property determines the style that needs to be applied and value determines the behavior of the property. It can be any property & value of the element. for example, `background-color: blue, width: 300px, height: 300px, position: fixed`, etc. It depends on what we want to style.

## 10. Types of Selectors(Type, Class, ID)

Now that we know how to target any element and style it according to the need. Let's see what are the different ways to target any element.

## Type Selector:

The above way we have seen just now is the type selector. In this, we target an element with the element name or type. For example,

```
  h1 {
    color: red;
    font-size: 34px;
  }
  p {
    background-color: green;
    color: red;
  }
  div {
    width: 400px;
    height: 300px;
  }
```

Here `h1 , p, div` are the name or type of element that we use in HTML. There is a reason why we call it a type selector. We have different types of elements based on the types of contents. We will be using a various number of `ps or divs` depending upon the layout. It can be other elements also. The thing is if we target using element's name, then whatever the number of that particular element has been used in HTML, all the elements of that type will get selected. For example, if we targeted the `p` element using its name, so all the `ps` in the page will be styled. That's why we call it as a type selector.

But, suppose if we want to target just one `p` at a time, not all, so for that purpose we have `class and id` selector.

### Class Selector:

Class Selector allows us to target an element with the class attribute defines inside the tag. For example,

```
  <div class="box">........</div>

  .box {
    height: 150px;
    width: 150px;
    background-color: red;
  }
```

To represent a class selector in CSS we denote it with `.` followed with the value we define inside the class attribute. Here, `box` is our class selector and it will select the element containing the class attribute value of `box`. We are free to choose any class name. And also at one time, we can provide the same class name to different elements. For example,

```
  <div class="perfect">.........</div>

  <p class="perfect">.........</p>

  .perfect {
    text-align: center;
  }
```

Here, the `perfect` class selector will select both `div and p` elements. The class selector is more specific than the type selector. Because with class selector we can target some particular group of elements instead of all the elements of one type.

### ID Selectors:

An ID selector is even more specific than class and type selector. Because we can target only one unique element at a time. As we define a class attribute in a similar way we define ID attribute also inside a tag. But to target an element using an ID selector in CSS we use `#` followed by the value defined inside the ID attribute. For example,

```
  <div id="select"></div>

  #select {
    background-color: green;
  }
```

Here, `select` is the ID selector and it will only select the element containing the id attribute value of `select`. Here one thing is to be noted that ID attribute value can be used once per page. It has to be unique. We can't reuse the same ID attribute value for other elements on the same page.

## 11. Referencing CSS

It's time to connect the dots. We have the basic idea of HTML & CSS. We also know how to target any element and style according to our need. So, let's connect them.

We can create an external stylesheet file and connect it to HTML. We have internal and inline styling option also. In the internal and inline styling, we can write our CSS inside the HTML file also.

In inline styling, we write our style inside the tag only. For example,

```
  <div style="background-color: red; color:blue; ">.......</div>
```

In internal styling, we define a style tag inside the head element and then we write our CSS. for example,

```
  <!DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="utf-8">
      <title>Hello World</title>
      <style>
        body {
          background-color: green;
        }
        .heading {
          color: black;
          font-size: 36px;
        }
      </style>
    </head>
    <body>
      <h1 class="heading">Hello World!</h1>
      <p>Our first web page.</p>
    </body>
  </html>
```

But the best practice is to have one separate stylesheet to write our CSS and then connect it with `link` tag inside the head elements.

```
  <!DOCTYPE html>
  <html lang="en">
      <head>
          <meta charset="utf-8">
          <title>.......</title>
            <link rel="stylesheet" href="style.css">
      </head>
      <body>
          ..........
      </body>
  </html>
```

It helps us in organizing both HTML & CSS code separately. And it also helps us in styling the entire website using just single stylesheet. For separate pages, we won't have to write CSS separately. With just single stylesheet we can style all the pages in a website.

To create an external stylesheet, let's just open the same folder we have created earlier in our text editor. Now create a new file with extension `.css` in the same folder. After that connect the CSS file to HTML document in a similar way we have done in the about code snippet. And in the CSS file, we can normally target any element and style according to the need.

## Answer the following questions

1. How do we target any element and style it in CSS?
2. What are the types of selectors? And which one is more specific?
3. How can we select any element with a class name?
4. How many ways are there to reference CSS in HTML? And which one is the best?
5. Wich tag is used to reference external stylesheet?

## Do the exercise 2.

# Getting to Know more about HTML

Mostly we have seen everything about the basics of HTML & CSS. But in order to start building even a simple website, we need to know more about HTML in detail. We will have to understand which element should be used to display different type of contents. HTML elements are used to provide meaning to the content so that the browser can understand what type of content you want to display. Different element has different semantic meaning so we will have to understand how to use elements semantically.

## 12. Semantic Overview

Here, the meaning of semantic is using a proper element for appropriate content. It's not just that we have to display the content on the page but it is also necessary to provide the exact meaning to the content on a page. Anyone can display the element and style according to the design, but the important part is how semantically you are using the tags.
Let's see a few semantic tags and how it is different from non-semantic tags.

`<section>, <header>, <nav>, <footer>, <article>`, etc are few example of semantic tags. If you see these semantic tags closely you can easily find the meaning from its name only.

Let's take `<header>`, from this tag anyone can easily understand that, this tag must be used to wrap the heading content of any website or any section or any article. In a similar way `<nav>`, must be responsible for wrapping the navigation content. Exactly this is how a semantic tag works.

There are several advantages of semantic elements. For example, search engine optimization(SE0), screen readers, and other devices to read and understand the content on a web page.

## 13. Non-semantic tag

Obviously, there are a lot more semantic elements, as we move forward we will get to know about them. But there are few which does not have any semantic meaning in a page. For example `<div> and <span>` which are solely used for styling purpose as containers. `<div> and <span>` are the generic elements, they do not have any semantic value. But off course, we will be using these two elements number of times while building a website.

## 14. Block Vs Inline

While working with different elements most of the time you'll encounter two types of elements i.e. Block and Inline. Based on the display properties, most of the elements are either block or inline-level elements.

Block-Level elements are those, which always begins from a new line, stacking on top of each other and always takes the available width. For example, `<p>, <div>, <header>` etc. Most of the block level elements are used to wrap the larger piece of contents. Block-level elements may wrap another block elements or inline-level elements.

Inline-Level elements are different from block-levels. Unlike the block level elements, inline-level elements do not take the whole available width, instead, it always takes the space according to the content it wraps inside and line up one after another. They can only wrap inline-level elements, not the block level. Inline-level elements are used to wrap the small piece of contents. For example, `<span>, <strong>, <br>` etc.

## 15. Text Based Elements

As we all know there are different kind of content. For example, text, images, video, forms, map, etc. But among them one of the most and predominant content is text. There a number of elements to display to text. The most commonly used text-based elements are heading elements`h1 to h6` and paragraph `p` elements.

### Heading Elements

We have six levels of heading elements i.e., `h1, h2, h3, h4, h5, h6`. Heading elements are used to provide to a heading of any section or any article. As there are six levels of heading elements, and each level has some semantic meaning, so accordingly it should be used where they are semantically correct. The primary heading should always come in H1 tag and subsequently, other levels should be used.

### Paragraph Elements

We have been seeing this element since the beginning. Mostly all the long paragraph should be wrap inside the paragraph element, `<p>`. It's a block level element.

Apart from heading and paragraph, we have a few more elements which are also text-based elements.

`<strong> and <b>` tag which are used to make any text bold. Again here both `<strong> and <b>` are semantically different from each other. `<strong>` is more semantically used than `<b>`. `<b>` is mostly used for styling purpose but it has no semantic meaning. `<strong>` has semantic meaning and it is used to provide strong importance to any text.

Similarly `strong and b` elements we also have `em and i` elements to make italicize any text. Again here `<em>` is more semantically correct than `<i>`.

## 16. Hyperlinks

We are almost set to build a simple structure of a website, just we need to learn, how do we create a hyperlink in a page and connect them to different pages or external website. Links are one of the core components in a web page. To create a link we use an anchor tag `<a>`, and inside the tag, we define href attribute, also known as hyperlink reference. For example,

```
  <a href="https://webwurx.in/">Webwurx</a>
```

This is how we create links in a page. Once we click on Webwurx in the page it will redirect us to Webwurx website. Here the `href` attribute accepts the destination link which will take us to the page or resources that has been defined the attribute.

It is most common to see that few links in a page connect to the other page of the same website as well as few links connect to a different website. For example,

```
  <a href="about.html">About</a>
  <a href="https://webwurx.in/">Webwurx</a>
```

Based on the link provided inside the href attribute of an anchor link, a link can have two types of path `Relative path` and `Absolute path`.

### Relative Path:

If the link connects to the other pages of the same website then it is considered as a relative path. A relative path will have the name of the file being linked to the page. It won't have any domain like `.com, .io, .org` etc in the attribute value. From the above code snippets, the first link has a relative path. If you click on `About` it will take to he about page of the same website.

### Absolute Path:

If the link connects to another website which is entirely different from the current one, then it is known to have an absolute path. An absolute path will always have a domain name like `.com, .org, .io` etc. The second link in the above snippets has an absolute path, once you click the Webwurx, it will take you to Webwurx's website.

### Opening links in a new window:

Most of the time absolute path is open in a new window or new tab not on the same tab. By default, all links open on the same tab. To open the link on a new window or tab we use target attribute with value `_blank`.

```
  <a href="https://webwurx.in/" target"_blank">Webwurx</a>
```

### Linking to email address:

```
  <a href="mailto:xyz@example.com">Mail me</a>
```

Here if you click the mail me, it will open dialogue box of default email client of the user. This is how we create an email link.

To create an email link we say `mailto:` followed by the email address to which the email has to be sent. Similarly as in the above code.

Additionally, we can also add subject and body text of the email. For example,

```
  <a href="mailto:xyz@example.com?subject=Reaching%20Out&body=How%20are%20you?">Mail Me</a>
```

Here `Reaching out` is the subject and `How are you?` is the body text of the email. To provide space we say `%20` between words and to break line we say `%0A`.

### Linking to other parts of the same page.

Sometimes we can also find the links are connected to other section of the same page. The best example for that type of link is, most of the time you may find `back to top` button when clicked it directly take to the top of the page.

To create such link we use `id` attribute and the value of the id attribute is provided in the href attribute of the anchor link.

```
  <body id="top">
    ................
    <a href="#top">Back to top</a>
    .................
  </body>
```

## 17. Building a structure with semantic tags

Now that we have learned something more in detail about HTML. We saw semantic overview, block, and inline level elements, some text-based elements, how to create hyperlinks. With the help of all these, we are good to build a simple structure of any website.

## Answer the following questions.

1. What are semantic tags?
2. Difference between a semantic tag and a normal tag?
3. List a few advantages of semantic tags?
4. With examples explain block-level and inline-level elements?
5. How can we open a link on another tab?
6. What are the types of path a link can have?

## Do the exercise 3

<!-- steps to follow -->

1. Fork the repo from the link
2. clone it
3. Solve the excercises
4. push the code
