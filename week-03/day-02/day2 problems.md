WEEK3 DAY 2:

Given this HTML, add first class to the first element in the list and last class to the last element in the list:

<ul>
  <li>London</li>
  <li>Paris</li>
  <li>Tokyo</li>
  <li>New York</li>
</ul>

LOGIC: Find the unordered list - refer to its firstChild - get reference back - add attribute node to it

CODE:

setAttribute(document.getElementsByTagName('ul').firstChild) class="first"
setAttribute(document.getElementsByTagName('ul').lastChild) class="last"

document.getElementsByTagName("ul").firstChild.setAttribute(class, "first");
document.getElementsByTagName("ul").lastChild.setAttribute(class, "last");

ONE THAT WORKS:
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>JS Bin</title>
  <style>
    .first {
      background-color: yellow;
    }
    .last{
      background-color:red;
    }
  </style>
  <script>
    setTimeout(function () {
      
      var desiredElement = document.getElementsByTagName("ul");
       var att =desiredElement[0].firstChild;
  
   att.setAttribute("class","first");
      
      var desiredElement = document.getElementsByTagName("ul");
       var att =desiredElement[0].lastChild;
  
   att.setAttribute("class","last");
      
      
    }, 0);
  </script>
</head>
<body>
  <h1>what is up with this?</h1>
  <ul><li>London</li>
  <li>Paris</li>
  <li>Tokyo</li>
  <li>New York</li></ul>
</body>
</html>

OPTIMISED VERSION:

  <script>
    setTimeout(function () {
      
      document.getElementsByTagName("ul")[0].firstChild.setAttribute("class", "first");
      document.getElementsByTagName("ul")[0].lastChild.setAttribute("class", "last");
      
    }, 0);
  </script>


___________________________________________________________________________

Replace this:

<div>
  <p id="latest"><strong>Friday</strong> is finally here.</p>
  <p>In addition the weather is sunny today.</p>
</div>

with this using JavaScript:

<div>
  <p id="latest">Monday is finally here.</p>
  <p>In addition the weather is sunny today.</p>
</div>

LOGIC:
Find ID with value 'latest' and replace text with a new value.
Nope - there is a textContent reserved thingy that will do it.

document.getElementById("latest").textContent="Monday is finally here";
      
____________________________________________________________________________

Build the content of <body></body> tag with JavaScript only: http://jsbin.com/tomita/edit?html,output


__________________________________________________________________________________

4. Create a function that can remember data, but without having to use global variables and without resending the same data with each function call.


ANSWER:
function greeting(greetingText){
    return function(name) {
     return (greetingText+' '+name);  
};
}

var dayGreeting = greeting('Good morning');
var nightGreeting = greeting('Good evening');

var name = 'Art';

console.log(dayGreeting(name));
console.log(nightGreeting(name));

_______________________________________________________________________________

Implement a function that will recursively traverse an array and return a string of the array values, in reverse order.

How to test
console.log(text);

function traverse(myArray){

for (var counter=myArray.length - 1;counter<0;counter=counter-1){
	console.log(myArray[counter]);
}
}
var array = ['London', 'Paris', 'Tokyo'];
var text = reverseArray(array, array.length, '');

