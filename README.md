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
manipulate it attributes <br>

wwe have getelementbyclassname method <br>
this method returns all elements in the document with that <br>
specified class name <br>

![d3](https://github.com/C191068/JS_DOM/assets/89090776/83d8b01a-6e9c-4761-ae76-9388f613d25b)

here we can see in all of our list items with class name list item <br>

![d4](https://github.com/C191068/JS_DOM/assets/89090776/cd6fd88d-9012-405d-b100-a58c7cdb1f42)
thus we can get the above output <br>

now this method returns an array of object of all the child elements <br>


which have all the given class names <br>

![image](https://github.com/C191068/JS_DOM/assets/89090776/01521349-a309-4d53-8bf1-31578ff1c837)

we can see they are index and in order in html file <br>


here getelementbytagname is similiar to getelementbyclassname <br>

it accepts a tag and return all element of that specified tag <br>


it returns an array of object for all child element with the given tag name <br>


![d6](https://github.com/C191068/JS_DOM/assets/89090776/29976af8-c92d-40be-af31-ab0013a0cfd7)

we get the above output which is similiar to getelementbyclassname <br>


the query selected method is used to select one item <br>

or first item that matches the selector <br>

so if we have multiple items with the same class name or with the same id <br>

or even the same tag it will select the first one it come across <br>

so the beauty of this method as you probably just guessed is <br>
that it can accept all css style selectors again allowing <br>
it is selected by tag or it's class or even it's id <br>

so we can actually use this method any element in our html file 

![d7](https://github.com/C191068/JS_DOM/assets/89090776/1ed22bac-00ea-4cba-b400-d4ad7ad376c7)

here we have the div tag <br>

![d8](https://github.com/C191068/JS_DOM/assets/89090776/bf5fe419-c914-480b-b7f5-1bc0ff851cb7)

for that we get the above output <br>



if we have more than one div and if we want to select them all we <br>
use queyselectorall <br>

![d10](https://github.com/C191068/JS_DOM/assets/89090776/51c1199c-0e2d-4cfb-b64d-5aa1ce1b7bb1)

for that we use the above code for below more than one div 


![image](https://github.com/C191068/JS_DOM/assets/89090776/222caad6-cb0a-49f3-8905-fc8baf660010)

for below more than one div <br>

![image](https://github.com/C191068/JS_DOM/assets/89090776/af52a5c4-c43c-42da-b6c0-0cab85f15353)

we get the above output <br>

in getbytagname and getbyclassname where we get html collection <br>
here we get node list <br>


now we will add styling to the elements <br>

we can access css properties in javasxcript <br>





![d11](https://github.com/C191068/JS_DOM/assets/89090776/b43c6ea7-e305-4c34-be36-687dc398f67a)


so first we will select main heading <br>

which is the title of the container <br>


and so we gonna put that in a variable <br>




![d12](https://github.com/C191068/JS_DOM/assets/89090776/04266158-7abc-438b-b8b2-a55b7c8baf74)

now we can see we have selected this elemnt and put inside the variable named title <br>


so what we can actuyally do is manipulate the styling of this elements <br>

and change it around using css properties <br>



![image](https://github.com/C191068/JS_DOM/assets/89090776/bda303f4-48e5-4dfe-8840-dddaab9401c9)



so to access css properties in javascript we just first grab the variable <br>

we want to apply styling to <br>

to which case is the title or main heading and simply type in the style property <br>

and after this style property we just use any css property <br>

you want to apply to this element <br>

and change the color of text <br>



![d13](https://github.com/C191068/JS_DOM/assets/89090776/4c2fb0ae-da06-4005-a2c8-eccc90ee21ee)

so we can see the colior is changed to red <br>


this type of styling is called inline styling <br>

this is probably the direct method <br>

![d14](https://github.com/C191068/JS_DOM/assets/89090776/a1094f14-7289-4cad-a0a7-b7d654e3934c)


now if we look at the console it is actually included style attribute <br>

again because this is dob=ne through inline styling <br>

if it is applied to all list items it will not work <br>

why we are using style property because css properties are written in camel case <br>

not with standard snake case <br>

![d15](https://github.com/C191068/JS_DOM/assets/89090776/361d2440-2b3e-4363-a2c8-28cdd91097e6)

if we try to apply inline css to list <br>

![d16](https://github.com/C191068/JS_DOM/assets/89090776/22952e00-4f6b-4f1d-9ba0-b91173aef2f5)

we get the above error <br>


if we want to apply style to list items we need to loop through all list items first <br>


![image](https://github.com/C191068/JS_DOM/assets/89090776/58b7bc44-a565-4626-aa18-000f9f07a991)

like above 


![image](https://github.com/C191068/JS_DOM/assets/89090776/0befd26a-ded0-48c3-be4d-11a14082a0a5)

output
<br>

another cool thing about DOM manipulation is that we can create elemnts from js file here <br>

![d1](https://github.com/C191068/JS_DOM/assets/89090776/00e9be1c-a201-4f2d-8c09-c36279b5be5b)

by the above line of code we create element <br>

now this is not actually do anything at this moment <br>

we can add element inside our document using append method  <br>

![d3](https://github.com/C191068/JS_DOM/assets/89090776/166be2ae-6cda-43cd-9461-69b2d39b5feb)

we can see a new list item is created <br>

now we gonna modify text in elements <br>

![d4](https://github.com/C191068/JS_DOM/assets/89090776/6665f157-42ee-428d-b5bb-dca03475e20c)

we have created span in the above <br>


![d5](https://github.com/C191068/JS_DOM/assets/89090776/d59d9d95-0e49-466e-b65c-e7748145d542)


now create another varaible to grab that element <br>


![d6](https://github.com/C191068/JS_DOM/assets/89090776/9bed02dd-d2ee-46eb-85a9-7de8c2f5cee1)

if we clearly look at tyhe console we can see the diffrences <br>

it is better to use innerText <br>

![d7](https://github.com/C191068/JS_DOM/assets/89090776/0d7c0080-49ab-49f4-83a4-3a28655a29e7)

so we have created a new list item <br>


![d8](https://github.com/C191068/JS_DOM/assets/89090776/18d4dbfb-16c4-4aba-bedd-e16c091991c9)

![d9](https://github.com/C191068/JS_DOM/assets/89090776/9b2a7c76-3e5c-48ff-a220-9cec614429d6)

the difference of using and and using of the code above which is used to set attribute <br>
 we have given the below list item below same id as our main heading <br>

 it got the same styling <br>

 ![d10](https://github.com/C191068/JS_DOM/assets/89090776/c642c86b-31dd-4d6f-a502-7d5cad5f0b5b)

to remove styling we use the above code <br>





![d11](https://github.com/C191068/JS_DOM/assets/89090776/2eef885d-6fb6-441f-ad67-1ddc93ea686d)



to access attributes in javascript we do the above <br>

to get the attribute of main haeding here we do the above  <br>


now we will see how to add class to our list items <br>

![d12](https://github.com/C191068/JS_DOM/assets/89090776/b62ef3cc-d72f-4d10-b882-e561588df64f)


we can see our last list item has exact the same styling like other list item <br>

![image](https://github.com/C191068/JS_DOM/assets/89090776/ee003881-cdca-4a8e-b63c-2e36876ca83f)

if we remove it we can see it has removed <br>


now we will find whether an element has specific class <br>


![d13](https://github.com/C191068/JS_DOM/assets/89090776/a1cb7854-7dc6-4c96-ba4e-35723b7de920)

so it return false <br>


![d14](https://github.com/C191068/JS_DOM/assets/89090776/8dadf1a5-7aec-4ce4-86fc-876b86d5cc77)
now it returns true <br>


now we will see how to remove an element <br>


![d15](https://github.com/C191068/JS_DOM/assets/89090776/9a722036-5740-47a3-837d-13de8066617d)

thus we have remove the elemnt <br>

![d16](https://github.com/C191068/JS_DOM/assets/89090776/9d960db5-856b-49cf-9218-0232922cdd3b)
thus we have remove the element <br>


DOM object is itself a property of window object <br>

which is a global top level object representing the tab in the browser <br>

the window object has access too much information <br>

the height and the width of the window <br>

![image](https://github.com/C191068/JS_DOM/assets/89090776/41547dfc-8b74-43df-a048-33742a9c630e)
here document node is the topmost node and root of dom tree <br>

it has one child node elemnt i.e html <br>


underneath head node has the child node which is title element <br>

other relations are similiar <br>

html attributes such as id ,class and styles are also considered <br>
nodes in dom tree <br>

but they don't participate in parent child relationship <br>

they accessed as properties of element node that contains them <br>


![d17](https://github.com/C191068/JS_DOM/assets/89090776/84d0b50f-f277-4ec2-91f0-4be559ca8aba)


so now here we will find parent of the ul and the grandparent <br>


![image](https://github.com/C191068/JS_DOM/assets/89090776/df13386a-afbb-4f31-b695-7099049f777e)

we can also see hovers over it <br>


![d18](https://github.com/C191068/JS_DOM/assets/89090776/e1d93604-ce35-4585-8aa6-c9650fe098a4)


we find the parent node in the above way <br>


![image](https://github.com/C191068/JS_DOM/assets/89090776/824c6fad-8b71-4470-b0ba-f8a62622262b)

to find the grandparent we do the above <br>


elemts are atype of node <br>



![d20](https://github.com/C191068/JS_DOM/assets/89090776/95615d5a-56a5-4686-ba56-50788e04dd37)

the above we can see the difference between nodes and elements <br>

here parent element is returning null <br>

because job of parent element is to return html element <br>


parent node is mostly used <br>

now we will take a look how we can navigate downwards in DOM tree <br>

i.e how to traverse child node <br>


![d21](https://github.com/C191068/JS_DOM/assets/89090776/9f64989a-8777-49e5-b4a1-5e29c5a2c054)

we can see in the console it has given us a node list <br>
we can get alist of child node inside the ul <br>

here distinction between between nodes na delements become more evident <br>

here we get three list items and four text nodes <br>

in adduition of three list items we get four text nodes <br>

this is because we wrote our own html this was not generated by javascript <br>

Inside of html here the indentation between element nodes is counted <br>
in the dom tree as text nodes <br>

![d22](https://github.com/C191068/JS_DOM/assets/89090776/b4586377-6265-4e05-a1d6-6fd3777b0a70)

here we remove one of the identataion brought the last list tag with the second at same line <br>

now we can see the node list is showing 6 <br>

again because identation are counted as text nodes <br>

so again distinction betwwen nodes and element nodews becomes more evident <br>

now as well child nodes property we also have first and last child <br>


as we probably guess this selects first and last child of our list <br>


![d23](https://github.com/C191068/JS_DOM/assets/89090776/923e3d88-7bb7-4920-8fba-072519969e33)

this is reeturnining us the text nodex <br>

because first index is a text node and last index is also a text node <br>

now when we are using first child and last child here which is selecting <br>
the first nde and last node we need to be very mindful if we are styling eklement <br>

using this property  <br>

![d24](https://github.com/C191068/JS_DOM/assets/89090776/32a88285-19ef-4b86-a308-8fe0510d0fd5)
 here we get an error here because first child here is actuallly a text node <br>
 it is not an elemnt <br>

 ![d25](https://github.com/C191068/JS_DOM/assets/89090776/625f84e6-5a38-4b7a-a154-bfaed5c6875a)

now by the above code the first list elemnt is colored green background color  <br>


 now unlike the aprent element here we also have in  children elemnt which can <br>

 select only element nodes <br>

 ![d26](https://github.com/C191068/JS_DOM/assets/89090776/576bd645-9da1-4a30-89c6-8e9911468581)

here it returns only html collection instead of node list <br>

![d27](https://github.com/C191068/JS_DOM/assets/89090776/255b3042-b420-485c-86c0-c8f0d69f06e7)

here weget the properties of child node <br>


at last we gonna take a look at sibling node traverssal <br>

siblings nodes are nodes on the same tree  level <br>


![image](https://github.com/C191068/JS_DOM/assets/89090776/9d724190-bd14-4e3a-87ca-d2f08f18c6c0)

in the above html of ours <br>

the ```h1``` and  ```ul``` are sibling to each other because they are on the same level  <br>

it is important to note that sibling do not have to be same typ eof node <br>

they are here as element node <br>

![d30](https://github.com/C191068/JS_DOM/assets/89090776/0dcb1c5b-967f-41c0-a8b4-a38faaf9b9a9)

in the above we get text node before ul and after ul <br>

now we want to find previous and next  element nodes  <br>


![d31](https://github.com/C191068/JS_DOM/assets/89090776/5b2ab34f-3c6d-4c36-9fd7-2f0f5a0789f1)

at console we can see it is the previous elemnt sibling node <br>

next element sibling we get null <br>


now we gonna talk about event listeners <br>

Event listeners are most frequently used javascript structures <br>
they allow us to add interactive functionality to html elements <br>
by listening to different events that take place on page  <br>

such as when users preses a key when elements load or when user clicks <br>
 a button <br>

 the most common event is load event <br>

touch start event , key down event , mouse over event  and of course <br>
click events <br>

![image](https://github.com/C191068/JS_DOM/assets/89090776/4c03f89c-be33-4d20-a327-12590511550b)

we can include events inside of our above index.html and directly one of these elements <br>

this event is global on event attribute <br>

this way of creating an event to an element works preety <br>
much like any attribute we inserted directly in the html element i.e presesnt <br>
 on the page <br>
 and then apply one line script to that particular event <br>
 

 ![d32](https://github.com/C191068/JS_DOM/assets/89090776/2a818f1e-703b-4278-8c1b-142c483ca989)

 we get the above output for the above code <br>

 
this is the direct include of an vent ot html <br>

now we will see about javascript add event listener method <br>



 

 




























![image](https://github.com/C191068/JS_DOM/assets/89090776/5e2d7006-492d-4ed4-8221-d645ec7aa118)

change browser in vs code <br>

https://stackoverflow.com/questions/49289233/how-to-change-default-browser-with-vs-codes-open-with-live-server








```

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
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


<br>


```

//GetElementId

//const title = document.getElementById("main-heading");
//console.log(title);

//GetElementbyclassname

//const listItem = document.getElementsByClassName("list-items");
//console.log(listItem);

//getelementbytagname

//const listItem = document.getElementsByTagName("li");
//console.log(listItem);

//queryselector

//const container = document.querySelector("div");
//console.log(container);

//queryselectorAll

const container = document.querySelectorAll("div");
console.log(container);


```


<br>

```
//DOM manipulation

//const title = document.querySelector("#main-heading");

//title.style.color = "red";

const listItems = document.querySelectorAll(".list-items");

for (i = 0; i < listItems.length; i++) {
  listItems[i].style.fontSize = "2rem";
}

console.log(listItems);


```
<br><br>

```
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="utf-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Movies</title>

  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #242222;
      margin: 0;
      padding: 0;
    }
    #home{
      float: inherit;
      margin: 0px 0px;
      padding: 0px 0px;
      
    }
    .container {
      max-width: auto;
      margin: 0 auto;
      padding: 20px;
      background-color: #fff;
      border-radius: 30px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
    }

    #main-heading {
      color: #5c4646;
      text-align: center;
      margin: 0px 0px 0px 0px;
      padding: 0px 0px 0px 0px;

    }

    .list-items {
      list-style: none;
      padding: 6px 0px;
      border: 1px solid #ccc;
      margin: 2px 100px;
      background-color: #f9f9f9;
    }

    .list-items span {
      color: #999;
      font-size: 14px;
      margin-left: 10px;
    }

    ul {
      padding: 0;
      text-align: left;
    }

  </style>

</head>

<body>
  <div class="container">
    <section id="home">
      <h1 id="main-heading">My favorite movies</h1>
      <ul>
        <li class="list-items">The Message<span>(1976)</span></li>
        <li class="list-items">Lion of the Desert</li>
        <li class="list-items">The Kingdom of Heaven</li>
      </ul>
    </section>
  </div>
  <script src="kapp.js"></script>
</body>

</html>

```

<br><br>


```

//DOM manipulation

//const title = document.querySelector("#main-heading");

//title.style.color = "red";

//const listItems = document.querySelectorAll(".list-items");

//for (i = 0; i < listItems.length; i++) {
//listItems[i].style.fontSize = "2rem";
//}

//Create elements

const ul = document.querySelector("ul");
const li = document.createElement("li");

ul.append(li);

li.innerText = "The Final legacy";

//Modify Attributes 

//li.setAttribute("id", "main-heading");
//li.removeAttribute("id");

//const title = document.querySelector('#main-heading');

//console.log(title.getAttribute('id'));

//Modify Classes

li.classList.add('list-items');


console.log(li.classList.contains('list-items'));

li.remove();

```

<br>

```js


//Parent Node Traversal 

//let ul = document.querySelector('ul');
//console.log(ul.parentNode.parentNode);

//const html = document.documentElement;
//console.log(html.parentNode);
//console.log(html.parentElement);

let ul = document.querySelector('ul');

console.log(ul.childNodes);
console.log(ul.firstChild);
console.log(ul.lastChild);

ul.childNodes[1].style.backgroundColor = 'green';


```

<br> <br>

```

//Parent Node Traversal 

//let ul = document.querySelector('ul');
//console.log(ul.parentNode.parentNode);

//const html = document.documentElement;
//console.log(html.parentNode);
//console.log(html.parentElement);



//console.log(ul.childNodes);
//console.log(ul.firstChild);
//console.log(ul.lastChild);

//ul.childNodes[1].style.backgroundColor = 'green';

//console.log(ul.children);
//console.log(ul.firstElementChild);
//console.log(ul.lastElementChild);

//Sibling Node Traversal

let ul = document.querySelector('ul');

const div = document.querySelector('div');

//console.log(div.childNodes);

console.log(ul.previousElementSibling);
console.log(ul.nextElementSibling);

```


<br>

```

<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="utf-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Movies</title>

  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #242222;
      margin: 0;
      padding: 0;
    }
    #home{
      float: inherit;
      margin: 0px 0px;
      padding: 0px 0px;
      
    }
    .container {
      max-width: auto;
      margin: 0 auto;
      padding: 20px;
      background-color: #fff;
      border-radius: 30px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
    }

    #main-heading {
      color: #5c4646;
      text-align: center;
      margin: 0px 0px 0px 0px;
      padding: 0px 0px 0px 0px;

    }

    .list-items {
      list-style: none;
      padding: 6px 0px;
      border: 1px solid #ccc;
      margin: 2px 100px;
      background-color: #f9f9f9;
    }

    .list-items span {
      color: #999;
      font-size: 14px;
      margin-left: 10px;
    }

    ul {
      padding: 0;
      text-align: left;
    }

  </style>

</head>

<body>
  <div class="container">
   
      <h1 id="main-heading">My favorite movies</h1>
      <!--Gap between-->
      <ul>
        <li class="list-items">The Message<span>(1976)</span></li>
        <li class="list-items">Lion of the Desert</li>
        <li class="list-items">The Kingdom of Heaven</li>
      </ul>
 
  </div>
  <script src="kapp.js"></script>
</body>

</html>

```

<br>

```

<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="utf-8">
  <meta http-equiv="X-UA-Compatible" content="IE-edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Movies</title>

  <style>
    body {
      font-family: 'Arial', sans-serif;
      background-color: #f0f0f0;
      text-align: center;
      margin: 0;
      padding: 0;
    }

    .container {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }

    .box {
      background-color: #f4f4f4;
      border: 2px solid #ccc;
      width: 250px; /* Set a fixed width for consistent size */
      padding: 20px;
      margin: 10px;
      border-radius: 10px;
      box-shadow: 0 3px 6px rgba(0, 0, 0, 0.1);
      text-align: center;
      transition: transform 0.2s, box-shadow 0.2s;
    }

    .box-1 {
      background-color: #ffcc66;
      border-color: #ffaa00;
    }

    .box-2 {
      background-color: #66ccff;
      border-color: #3399ff;
    }

    .box-3 {
      background-color: #66ffcc;
      border-color: #33ff99;
    }

    h1 {
      font-size: 28px;
      color: #333;
      margin-bottom: 15px;
    }

    button {
      background-color: #007bff;
      color: #fff;
      border: none;
      padding: 10px 20px;
      font-size: 16px;
      cursor: pointer;
      border-radius: 5px;
      transition: background-color 0.3s;
    }

    button:hover {
      background-color: #0056b3;
    }

    .box:hover {
      transform: scale(1.05);
      box-shadow: 0 6px 12px rgba(0, 0, 0, 0.2);
    }
  </style>
</head>

<body>
  <h1 id="main-heading">Event Listeners</h1>
  <div class="container">
    <div class="box box-1">
      <h1>The Message</h1>
      <button onclick="alert('Enjoy the movie')">Click</button>
    </div>
    <div class="box box-2">
      <h1>The Final Legacy</h1>
      <button class ="btn-2">Click</button>
    </div>
    <div class="box box-3">
      <h1>The Kingdom of Heaven</h1>
      <button class="btn-3">Click</button>
    </div>
  </div>
  <script src="kapp.js"></script>
</body>
</html>


```





















