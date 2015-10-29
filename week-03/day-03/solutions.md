

Access the text node and log it's value:

<div>
  <p>JavaScript is pretty powerful.</p>
</div>
Hint: use nodeValue

Log all the text:
_______________________________________________________________

<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>JS Bin</title>
  <style>
    .highlight {
      background-color: yellow;
    }
  </style>
  <script>
    setTimeout(function () {
      
     var x = document.getElementsByTagName("p")[0];
    textvalue = x.firstChild.nodeValue;
    console.log(textvalue);
      
    }, 0);
  </script>
</head>
<body>
  <div><p>JavaScript is pretty powerful.</p>
</body>
</html>

_________________________________________________________________________

NEXT QUESTION:
Log all the text in this:


Hint: use textContent

ANSWER:
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>JS Bin</title>
  <style>
    .first {
      background-color: yellow;
    }
  </style>
  <script>
     setTimeout(function () {
    var c = document.querySelector("p").textContent;
  
    console.log(c);
   
      }, 0);
  </script>
</head>
<body>
  <div>
  <p><em>JavaScript</em> is pretty <strong>powerful</strong>.</p>
</div>
</body>
</html>



___________________________________________________________________________

Convert all list item text to links:

<ul>
  <li>London</li>
  <li>Paris</li>
  <li>New York</li>
</ul>

SOLUTION ONE:
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>JS Bin</title>
  <style>
    .first {
      background-color: yellow;
    }
   
     
      }
    }
  </style>
  <script>
    setTimeout(function () {
     
      var frag = document.createDocumentFragment(); 
      var wantedElements = document.getElementsByTagName("li");
      console.log(wantedElements.length);   
      
      for (x=0;x<wantedElements.length;x++){    
        
          var aTag = document.createElement('a');      //create an a tag
          var aTaglink=document.createTextNode(wantedElements[x].outerText);
       //   aTag.appendChild(aTaglink);          //add the text to the tag
          aTag.href="wantedElements[x].outerText";  //add the ref to the tag
          frag.appendChild(aTag);           //add tag to new fragment
         console.log(wantedElements[x].outerText);
        // document.getElementsByTagName('li')[x].parentNode.removeChild;
         document.getElementsByTagName('li')[x].appendChild(frag);
         
      
      }
      
       
    }, 0);
  </script>
</head>
<body>
  <ul>
  <li>London</li>
  <li>Paris</li>
    <li>New York</li>
    <li>Dubai<li>
</ul>
</body>
</html>
_________________________________________________________________________

Add class highlight to even list items:

<ul>
  <li class="based-in">London</li>
  <li class="visited">San Francisco</li>
  <li>Paris</li>
  <li>Tokyo</li>
  <li class="going-to">New York</li>
</ul>
___________________________________________________________________________

ANSWER:

<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>JS Bin</title>
  <style>
  .first {
    background-color: yellow;}
   .visited{
      background-color:green;
    }
    
  </style>
  <script>
    setTimeout(function () {
     
     var highElements = document.getElementsByTagName("li");
      console.log(highElements.length);   
       
      for (var x=0;x<highElements.length;x++){
        if (x % 2===0){
          console.log(x);
          highElements[x].setAttribute("class","first");
        }
      }
      
    }, 0);
  </script>
</head>
<body>
<ul>
  <li >London</li>
  <li class="visited">San Francisco</li>
  <li>Paris</li>
  <li>Tokyo</li>
  <li >New York</li>
</ul>
</body>
</html>

__________________________________________________________________

Given an array of image URLs, create a web page with a slideshow that updates image every 2 seconds.

var images = [
  'http://valuestockphoto.com/freehighresimages/roast_veg_DSC2834.jpg',
  'http://valuestockphoto.com/freehighresimages/snowy_trees1995.jpg',
  'http://valuestockphoto.com/freehighresimages/nt_alice_springs140362.jpg',
  'http://valuestockphoto.com/freehighresimages/diwali_deepavali_DSC2292.jpg'
];
Take a look at window.setInterval() function.

