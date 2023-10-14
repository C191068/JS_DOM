# Intro(leaning fro freecodecamp)

DOM stands for Document object module <br>

Document object is a built in object that has many properties and methosd that we <br>
can use to manipulate the content <br>
the structure ,the style of the project <br>

this ability to manipulate the DOM or document object model is the most <br>
unique and useful abilities in javascript <br>

so almost anytime a website perfoms an action such as toggling a navigation menu <br>

or rotaing between slide show images or even dispalying an error <br>

when user tends to submit an incomplete form <br>

this is a result of javascript accessing and manipulating the DOM <br>


![image](https://github.com/C191068/JS_DOM/assets/89090776/41547dfc-8b74-43df-a048-33742a9c630e)


now another way of thinking of the DOM is thinking of it as atree of nodes <br>

like the above <br>

DOM object is actually property of window object <br>

which is a global top level object reperesenting a tab in the browser <br>

and this window object has access to information such as toolbars <br>

height and width of the window <br>

most of the node in the above diagram have praent child relationship <br>

the topmost node is the document node here and is the root node of the DOM tree <br>


which we access to DOM and manipulate all the content <br>

now this document node has one child node which is HTML <br>


nad html is the parent to head and body element <br>

now head and body elemts what we called is sibling <br>

since they rae on the same level of the DOM tree <br>

underneath the head elmt is what is the title element <br>

body element is the parent of paragraph and h1 <br>

paragraph and h1 are siblings to each other <br>


text content s inside each of these elemts are child node <br>

to the paragraph and h1 <br>


so my links and my headers are child nodes to h1 <br>

and paragraph element <br>


now we can see by paragraph tag we have class attributes <br>

now html attributes such as ids and classes in this case <br>
styles etc are also considers node in the dom hierarchy <br>

but they actually don't participate in parent child sibling relationship <br>

like othernodes do <br>

the way they are accessed is through the properrties of the element nodes <br>

that they contained in <br>

the way they are accessed is through the properties of the element node <br>
 understing this parent child relationship is crucial to understanding <br>

how javascript works with html <br>


in order to first select an element in the dom tree we have to first select the element <br>

there are five major ways of selecting element <br>

by using the method GetElementId we can select an element by it's unique id <br>


this is the esaiest way to find an html elemnt inside the dom tree <br>

we know from css the id attribute is ussed for something unique <br>

![d1](https://github.com/C191068/JS_DOM/assets/89090776/7584b65a-b156-4814-8b48-43b665c3fca6)

here id of h1 is main heading <br>


![image](https://github.com/C191068/JS_DOM/assets/89090776/b07c158c-6778-4357-992b-846bfd31d741)

when we type the above code <br>

![d2](https://github.com/C191068/JS_DOM/assets/89090776/725fb1d3-1df4-4028-b1b8-534845239f79)

we get the above output in browser <br>

![image](https://github.com/C191068/JS_DOM/assets/89090776/e7af48c5-f815-4e2f-ad1a-d540ba9cfaff)

if we hover over this it is highlighted in the browser <br>

here we have selected that element and now we can do is select that <br>
variable we just created for the element and we can add styles to the element <br>
manipulate it attributes 
































![image](https://github.com/C191068/JS_DOM/assets/89090776/5e2d7006-492d-4ed4-8221-d645ec7aa118)

change browser in vs code <br>

https://stackoverflow.com/questions/49289233/how-to-change-default-browser-with-vs-codes-open-with-live-server








```

<html>
  <head>
    <meta http-equiv="X-UA-Compatible"
    content="IE=edge">
    <meta name="viewport"
    content="width=device-width, initial scale=1.0">
    <title>Movies</title>
  </head>

  <body>
    <div class="container">
      <h1 id="main-heading">My favorite movies</h1>
      <ul>
        <li class="list-items">The Message</li>
        <li class="list-items">Lion of the Desert</li>
        <li class="list-items">The Kingdom of Heaven</li>
      </ul>
    </div>
    <script src="kapp.js"></script>
  </body>
</html>


```





















