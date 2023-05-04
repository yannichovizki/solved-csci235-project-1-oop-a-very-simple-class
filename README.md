Download Link: https://assignmentchef.com/product/solved-csci235-project-1-oop-a-very-simple-class
<br>
<strong> </strong>

Project1 is trivial and simply a starter project to establish basic ideas of <strong>OOP </strong>and ensuring you can successfully submit to Gradescope.

You will write 1 very simple class: <strong>Animal. </strong>Every Animal has a name, it may be domestic (or not) and it may be a predator (or not).

<strong>Implementation: </strong>

You must separate interface from implementation (.hpp and .cpp files) and implement the class based on the following specification (FUNCTION PROTOTYPES AND MEMBER VARIABLE NAMES MUST MATCH EXACTLY). This class has only accessor and mutator functions for its private data members. Recall that accessor functions (e.g. getName()) are used to access the private data members (e.g. all getName() will do is return name_), while mutator functions give a value to the data members. Remember, <strong>you must thoroughly document your code!!! </strong>

<strong>class Animal </strong><strong>public</strong><strong> members:</strong>

Animal();

Animal(<strong>std</strong><strong>::</strong><strong>string</strong> name, <strong>bool</strong> domestic = <strong>false</strong>, <strong>bool</strong> predator = <strong>false</strong>);  <strong>std</strong><strong>::</strong><strong>string</strong> getName() <strong>const</strong>;   <strong>bool</strong> isDomestic() <strong>const</strong>;      <strong>bool</strong> isPredator() <strong>const</strong>;     <strong>void</strong> setName(<strong>std</strong><strong>::</strong><strong>string</strong> name);      <strong>void</strong> setDomestic();      <strong>void</strong> setPredator();

<strong>class Animal </strong><strong>private</strong><strong> members:</strong>

<strong>std</strong><strong>::</strong><strong>string</strong> name_;  <strong>bool</strong> domestic_;  <strong>bool</strong> predator_;

<strong>Testing: </strong>

This project is very basic, but it is never too early to set in good debugging and testing habits. You must always implement and test your programs <strong>INCREMENTALLY</strong>!!!

<strong><em>What does this mean? </em></strong>

<ul>

 <li>Implement and test one class at a time!!!</li>

 <li>For each class:</li>

 <li>Implement one function/method and test it thoroughly (multiple test cases + edge cases if applicable)</li>

 <li>Implement the next function/method and test it …</li>

 <li>…</li>

</ul>

<strong><em>How do you do this?</em></strong><em>  </em>

Write your own <strong>main()</strong> function to test your classes. In this course you will never submit your test program but you must always write one to test your classes.  As you implement each Animal method, instantiate objects of type Animal in main and call the method to test it is correct. Start from the constructor(s), then move on to the other functions.  You may output the return values to inspect your program’s behavior. Choose the order in which you implement your methods so that you can test incrementally (i.e. implement mutator functions before accessor functions). Sometimes functions depend on one another. If you need to use a function you have not yet implemented, you can use <strong>stubs: </strong>a dummy implementation that always returns a single value for testing (don’t forget to go back and implement the stub!!! If you put the word STUB in a comment, some editors will make it more visible so you will remember to implement it later) For example:

<em>//******** STUB ************//</em> <strong>bool</strong> Animal::isPredator() <strong>const</strong>

{

<strong>return</strong> false;

}

<u>Note:</u> this will make much more sense as your programs become more complex, but it is very important to understand the fundamental concepts and develop good implement/test/debug habits from the very beginning.