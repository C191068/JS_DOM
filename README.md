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






















