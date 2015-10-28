Problems

1. Make sure variable message is defined in a private scope:
var message = 'Welcome!';

ANS:
function(){
	var message='Welcome!';
}
(Now its in the scope of the anonymous function.


__________________________________________________________________

2. Write validate Parameter function that takes a parameter, checks whether it's type is string and length is greater than 0.

function xx(input){
	if (typeof(input==='string') && (input.length>0)) {
	console.log (input);
	return true;
	}
	return false;
}

xx('text');
xx(5);
xx("Who's a pretty boy then?");

How to test:

validateParameter(); // returns: false
validateParameter(''); // returns: false
validateParameter(5); // returns: false
validateParameter('Welcome'); // returns: true



________________________________________________________

 Write findInList function that takes 2 parameters: a string and a character and returns a number of times that character is repeated in that string.

function findInList(str1, ch1){
  var instances=0;
  
  if ((typeof(str1)==='string')&& (typeof(ch1)==='string')) {
    var lowerstr=str1.toLowerCase(); 
    for (var i=0; i<lowerstr.length;i++){
        if (lowerstr[i]===ch1) {
            instances=instances+1;
        } 
    }
  }
   
  console.log(instances);
  return(instances);
}

findInList('', 'a'); // returns: 0
findInList('Hello', 'a'); // returns: 0
findInList('Again', 'a'); // returns: 2
findInList(); // returns: 0
findInList(''); // returns: 0


_____________________________________________

Write squareList function that takes an array of numbers and returns a new array where each number is squared.

function squareList(input){

var newArray=[];
if (typeof(input)==='object') {
for (var i=0;i<input.length;i++){
  newArray[i]=input[i]*input[i];
}
}
console.log(newArray);
}

squareList(); // returns: []
squareList([]); // returns: []
squareList([2]); // returns: [4]
squareList([2, 4, 1]); // returns: [4, 16, 1]

Version 2:
function squareList(myArray){

var squaredArray=[];
  
if (typeof(myArray)==='object') {
  for (var i=0;i<myArray.length;i++){
    squaredArray[i]=myArray[i]*myArray[i];
	}
}
console.log(squaredArray);
return(squaredArray);
}

squareList(); // returns: []
squareList([]); // returns: []
squareList([2]); // returns: [4]
squareList([2, 4, 1]); // returns: [4, 16, 1]

________________________________________________

Write filterList function that takes an array of any values and returns a new array with only non-empty strings.

function filterList(myArray){

var newArray=[];
if (typeof(myArray)==='object'){
for (var i=0;i<myArray.length;i++){
  if ((typeof(myArray[i])==='string') &&(myArray[i].length>0)){ 
    newArray.push(myArray[i]);
    }
   }
}
console.log(newArray);
return(newArray);
}

filterList(); // returns: []
filterList([]); // returns: []
filterList(['', 78]); // returns: []
filterList([37, 'Welcome', [], 'back']); // returns: ['Welcome', 'back']


_____________________________________________________________

Write iterateList function that takes an array and a function and for each item in that array it calls the function and passes array's item as a parameter.

function iterateList(myArray,myFunction){
  
  for (var i=0;i<myArray.length;i++){
    myFunction(myArray[i]);
     
  } 
}
iterateList([1, 2, 3, 4, 5], function (listItem) {
  console.log(listItem);
});

___________________________________________________________________



Write add function that adds two numbers, but it needs to be called twice for that.

total=0;
function add(arg1){

  count=0;
  
  if (count < 2) {
    total=total+arg1;
    count++;
  }
 console.log(total);
}

var add5 = add(5);
var sum = add(10); // returns: 15

Version 2:


total=0;
function add(arg1){
	total=total+arg1;
    console.log("step1",total);
   	function add5 (arg2)
        {total=total+arg2;
        console.log(total);}
   	return (add5);
   	}
console.log(total);
 
 
var add5 = add(5);
var sum = add5(10); // returns: 15

Version 3:

function add(arg1){
	return function (arg2){
	return(arg1+arg2);
	};
}
var add5 = add(5);
var sum = add5(10); // returns: 15
console.log(sum);
______________________________________________________________


Explain why undefined is logged and how to get the actual message logged:

var message = (function () {
  var message = 'Welcome';

  function getMessage(message) {
    return message;
  }
  return {
    getMessage: getMessage
  };
})();

console.log(message.getMessage());

______________________________________________________________


Write mergeArrays function:

mergeArrays([1,2,3], ['a', 'b', 'c']); // returns [[1, a], [2, b], [3, c]];

function mergeArrays(a1,b1){
var newArray=[];
  for (var i=0;i<a1.length;i++){
    newArray.push([a1[i],b1[i]]);    
  }
  console.log(newArray);
  return(newArray);
}

mergeArrays(['a','b','c'],[1,2,3]);
______________________________________________________________
STOP *******
----------------------------------------------------------


Given this HTML, add first class to the first element in the list and last class to the last element in the list:

<ul>
  <li class="first">London</li>
  <li>Paris</li>
  <li>Tokyo</li>
  <li class="last">New York</li>
</ul>

//Or li:firstchild li:lastchild
//or without changing the HTML directly?

______________________________________________________________


Replace content of the element with latest id to Monday is finally here., where Monday is strong:

<div>
  <p id="latest"><strong>Friday</strong> is finally here.</p>
  <p>In addition the weather is sunny today.</p>
</div>

if id==="latest" {
	text = <strong>Monday</strong> is finally here
}

