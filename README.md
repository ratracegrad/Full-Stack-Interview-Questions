# Full-Stack Interview Questions

> Over 70 actual interview questions to help you prepare for your Full-Stack Interview Questions.

## Table of Contents
1. [General Questions]('#general questions')
1. [JavaScript Questions]('#javascript questions')
1. [jQuery Questions]('#jquery questions')
2. [HTML/CSS Questions]('#html/css questions')
1. [Author](#author)
1. [Contributing](#contributing)

## General Questions
1. What is your favorite new library / framework / technology?

2. What tools do you use to debug your code?

3. What is a factory pattern?

4. Describe some code you wrote that you would write differently if you were writing it today?

5. What are some common storage structures?

6. Tell me about a challenging interaction with a teammate?

7. Why should we hire you?

8. Tell me something about yourself that is not on your resume?

9. Have you ever been in a situation where you were asked to do something you weren't sure was morally right? Explain how you handled it.

10. Describe a situation where you had to deliver bad news or report a significant problem with a project to your boss or to a client.

## JavaScript Questions
1. What is JavaScript?

2. What are the differences between the following expressions:

  x = y;

  x == y;

  x === y;
      
3. What is hoisting in JavaScript? Provide an example?

4. Is this valid JavaScript? Why or why not?

  var x = multiply(2)(3);
      
5. What is 'this' keyword in JavaScript?

6. What will be the output to the console for the following?

  function firstHalf() {
    var qtr1 = "kickoff";

    if (true){
      var qtr1 = "touchdown";
      qtr2 = "field goal";
    }

    console.log(qtr1); 
    console.log(qtr2); 
  }

  function  secondHalf() {
    console.log(qtr1); 
    console.log(qtr2); 
  }

  firstHalf();
  secondHalf();
      
7. How do you remove a property from an object?

8. What will be the output to the console for the following?

  function countDown() {
    for (var index = 5; index > 0; index--){
      setTimeout(function() {
        console.log('Index: ' + index);
      }, 5000 );
    }
  }
  countDown();
      
9. What is the difference between substr and substring? Provide an example showing how to use each.

10. What will be the output to the console for the following?

  function foo() {
    console.log(this.bar);
  }
  var bar = "bar";
  var biz = { bar: "biz", foo: foo };
  var bang = { bar: "bang" };
  foo(); 
  biz.foo(); 
  biz.foo.call(); 
  biz.foo.call(bang);
      
11. Why would you ever wrap an entire function or source file in a function block?

12. What do the following statements return?

  typeof "Hello World"; 
  typeof [1, 2, 3].concat();
  typeof {a:1}; 
  typeof function test() {}
  typeof [1, 2, 3]; 
  typeof null;
  typeof NaN;
      
13. What is a "closure" in JavaScript? Provide an example.
14. What is the output from the following code?

  (function() {
     foo = 5;
     var bar = 10;
  })();

  console.log(foo);
  console.log(bar);
          
15. What is the difference between a function declaration and a function expression?

16. What is the output from the following code?

  (function() {
    var apple = 2;
    function pie() {
      var apple = 3;
    }
    pie();
    console.log(apple);
    if (apple) {
      var apple = 3;
    }
    console.log(apple);
   })();

        
17.List all the JavaScript data types?

18. Write a multiply function that will produce the following outputs when invoked.

  console.log( multiply(2, 3); // output: 6
  console.log( multiply(4)(5) ); // output: 20
        
19. What is strict mode in JavaScript? How do you implement it? Why would you use it?

20. Answer the following questions.

  How do you remove the first item in an array?
  How do you remove the last item in an array?
  How do you add a new item to the beginning of an array?
  How do you add a new item to the end of an array?
  How do you remove all the entries in an array?        
        
21. Your function takes one parameter. How would you verify that the parameter is an array?

22. What is event bubling?


## jQuery Questions
1. What is jQuery and why would you use it?

2. What does this command do?

  $("p")
            
3. How do you deal with cross domain requests?

4. What does the following command do?

  <script type="text/javascript" 
    src="http://ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.min.js">
  </script>
            
5. Can you list some HTTP verbs?

6. What is the difference between $(document).ready and window.onLoad()?

7. Can you delay the execution of $(document).ready?

8. Can you have more than one $(document).ready function on the same page?

9. Would you use jQuery for client side scripting or server side scripting?

10. What is the difference between jQuery detach() and remove() functions?

11. What is the difference between jQuery.ajax() and jQuery.get()?

12. What does the dollar sign ($) mean in jQuery?

13. What does the following code do?

  $( "div" ).css( "width", "100px" ).add( "p" ).css( "background-color", "red" );
            
14. Can you replace the dollar sign ($) in jQuery with your own chosen character?

15. What is the difference between get() and post()?

16. How can the style of an element be changed?

17. How would you load jQuery from a CDN? How would you load jQuery if the CDN is not working?

18. How can the class of an element be changed?

19. Which is faster getElementsByTagName() or querySelectorAll()? Why?

20. What is the difference between .textContent and .innerText?

21. What is method chaining in jQuery. Provide an example.


## HTML/CSS Questions
1. In CSS what is the difference between an id and a class?

2. What are sprites and why would you use them?

3. Write a CSS selector to select only the inner two li's in the markup below:

  <ul class="myList">
    <li>One</li>
    <li>Two</li>
    <li>
      <ul>
        <li>Three A</li>
        <li>Three B</li>
      </ul>
    </li>
    <li>Four</li>
  </ul>
              
4. What does the box-model refer to in CSS?

5. What is the difference beween :link and :visited?

6. Write a CSS selector to select only the first li of the inner two li's in the markup below:

  <ul class="myList">
    <li>One</li>
    <li>Two</li>
    <li>
      <ul>
        <li>Three A</li>
        <li>Three B</li>
      </ul>
    </li>
    <li>Four</li>
  </ul>
              
7. Can an HTML element have multiple classes?

8. Using CSS properties alone, recreate this button: (*from Mobify's CodePen account)
button

9. What are media queries and why would you use them?

10. What is the difference between these three selectors?


  div {
    background: red;
  }
  .div {
    background: blue;
  }
  #div {
    background: green;
  }
            
11. What are some ways to change the location of an element on a page via CSS?

12. What would a table look like with this css applied?


  tr:nth-child(even) {
    background: red;
  }
  col:first-child {
    background: yellow;
  }
            
13. Is there a way to change the box-model?

14. What is the difference between visibility: hidden and visibility: none?

15. Given this CSS:

  div span {
    color: red;
  }
  div > span {
    background: green;
  }
            
What would this HTML look like when rendered?


  <div>
    <p>
      <span>All work and no play</span>
    </p>
  </div>
  <div>
    <span>makes Jack a dull boy</span>
  </div>
            
16. How do you clear a floated element?

17. What is specificity in CSS? Give examples of all levels.

18. What will the HTML look like for the following?

  <style>
  div span {
      color: red;
  }

  div > span {
      background: green;
  }
  </style>

  <div>
      <p>
          <span>Hello World</span>
      </p>
  </div>
  <div>
      <span>foo bar</span>
  </div>
            
19. What are Sass and LESS? Why would you use them?

20. What is a "reset" CSS file? What is normalize.css? Are they the same or different?

21. What is the difference between inline, inline-block and block?


## Author

  - __Product Owner__: Jennifer Bland
  
I am a Software Developer with over 10 years of development experience. I am the author of the book "Developing e-Business Applications Using Lotus Domino on the AS\400". 
  

## Contributing
See [CONTRIBUTING.md](CONTRIBUTING.md) for contribution guidelines.
