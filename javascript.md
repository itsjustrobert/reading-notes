# WHAT IS JAVASCRIPT:
JavaScript (JS) is a lightweight, interpreted, or just-in-time compiled programming language with first-class functions.<br> While it is most well-known as the scripting language for Web pages, many non-browser environments also use it, such as Node.js, Apache CouchDB and Adobe Acrobat.<br> JavaScript is a prototype-based, multi-paradigm, single-threaded, dynamic language, supporting object-oriented, imperative, and declarative (e.g. functional programming) styles.
<hr>
 
<h1>
A FEW COMMANDS TO INTERACT WITH THE USER:</h1>

 >Alert<br>
 *alert("Hello");
The mini-window with the message is called a modal window. The word “modal” means that the visitor can’t interact with the rest of the page, press other buttons, etc, until they have dealt with the window. In this case – until they press “OK”.*

   >Prompt<br>
   *The function prompt accepts two arguments:
    result = prompt(title, [default]);
    It shows a modal window with a text message, an input field for the visitor, and the buttons OK/Cancel.*

   >Confirm<br>
      *shows a message and waits for the user to press “OK” or “Cancel”. It returns true for OK and false for Cancel/Esc.
       All these methods are modal: they pause script execution and don’t allow the visitor to interact with the rest of the page until the window has been dismissed.*

<hr>

<h1>
Conditional Branching
</h1>
<vr>

>Sometimes, we need to perform different actions based on different conditions.

>To do that, we can use the if statement and the conditional operator ?, that’s also called a “question mark” operator.

<h1>The “if” statement</h1>

>The if(...) statement evaluates a condition in parentheses and, if the result is 
true, executes a block of code.

<vr>

 
>>>For example:

let year = prompt('In which year was ECMAScript-2015 specification 

published?', '');


if (year == 2015) alert( 'You are right!' );

In the example above, the condition is a simple equality check > 

(year == 2015), but it can be much more complex.

>>>if we want to execute more than one statement, we have to wrap our code block inside curly braces:

if (year == 2015) {
  alert( "That's correct!" );
  alert( "You're so smart!");
 


<h1>
</h1>
<h1>
The "else" Clause
</h1>

>The “else” clause
The if statement may contain an optional “else” block. It executes when the condition is falsy.

For example:

let year = prompt('In which year was the ECMAScript-2015 specification published?', '');

if (year == 2015) {

  alert( 'You guessed it right!' );

} else {

  alert( 'How can you be so wrong?' ); // any value except 2015

}

<h1></h1>
<h1>several conditions: “else if”</h1>

>Sometimes, we’d like to test several variants of a condition. The else if clause lets us do that.
For example:

let year = prompt('In which year was the ECMAScript-2015 specification published?', '');

if (year < 2015) {

  alert( 'Too early...' );

} else if (year > 2015) {
 
  alert( 'Too late' );

} else {
 
  alert( 'Exactly!' );

}
