Download Link: https://assignmentchef.com/product/solved-microwave-oven
<br>
<a id="user-content-learning-objectives" class="anchor" href="https://github.com/Grimlek/Course-Work/tree/master/Microwave%20Oven#learning-objectives" aria-hidden="true"></a>Learning Objectives

<ul>

 <li>Write a complete (but simple) class with multiple methods</li>

 <li>Write instance variable (field) declarations</li>

 <li>Write accessor methods (getter methods)</li>

 <li>Write mutator methods</li>

 <li>Write methods with simple parameters</li>

 <li>Write a default constructor</li>

 <li>Write a simple test program (a test driver)</li>

</ul>

<h3><a id="user-content-overview" class="anchor" href="https://github.com/Grimlek/Course-Work/tree/master/Microwave%20Oven#overview" aria-hidden="true"></a>Overview</h3>

In this assignment, you will write another complete class that is intended to reinforce your basic skills in writing instance variables, getter methods, and setter methods, while also introducing the use of if statements to provide conditional logic, controlled by boolean conditions based on object state. You will also switch from writing “tester programs” that just print output to writing repeatable, automatically executable software tests for your work using the JUnit testing framework.

The subject of this assignment is inspired by one of the programming exercises from Chapter 5 of the textbook, which is based on the textbook author’s own minivan. If you drive a late model minivan with power doors, you might recognize some of these behaviors yourself.

Your task is to simulate a portion of the control software for the vehicle. You will write a class that represents the state of the controls, providing accessor and mutator methods for the state of the relevant vehicle switches. You will also provide methods that represent door opening actions, and that implement logic matching the description provided below.

<h3><a id="user-content-details" class="anchor" href="https://github.com/Grimlek/Course-Work/tree/master/Microwave%20Oven#details" aria-hidden="true"></a>Details</h3>

Write a class called MicrowaveOven that models the behavior of a really simple microwave oven. This microwave includes a power setting, ranging from 1-10, a timer, indicating the number of seconds of cooking time, and a “start” button that starts the cooking process. Your class should provide the following:

<ul>

 <li>Instance variables (fields) to hold the power and the cooking time as integers.</li>

 <li>MicrowaveOven(): a constructor that initializes the instance variables. Initially, the power setting should be 10, and the cooking time should be zero.</li>

 <li>getPower(): an accessor method (or getter method) that returns the current power setting.</li>

 <li>setPower(): a mutator method (this specific kind of mutator is also known as a setter method) that takes a single parameter representing the new power level and changes the microwave’s power level to the requested value. You may assume that only legal values of 1-10 will be passed into this method.</li>

 <li>getCookingTime(): an accessor (or getter) method that returns the current cooking time setting.</li>

 <li>setCookingTime(): a mutator (or setter) method that takes a single parameter representing the new cooking time in seconds and changes the microwave’s cooking time setting to the requested value.</li>

 <li>start(): a mutator method that takes no parameters and that represents pressing the start button. This method should print a message of this form (with appropriate values appearing in place of the blanks):</li>

</ul>

Cooking for ___ seconds at power level ___

The textbook author’s minivan has two power sliding doors. Each door can be opened by either a dashboard switch, its inside handle, or its outside handle. However, the inside handles do not work if the minivan’s child lock switch is activated. In order for the sliding doors to open, the gear shift must be in park, and the master unlock switch must be activated. You will write a class that represents these vehicle features, and models the process of deciding whether a sliding door will open or not.

At the same time, you will also write software tests to confirm your solution works the way it should. Instead of writing a “tester” program that just prints out expected results, you will instead write your software tests using the JUnit testing framework, which makes it much easier to repeatedly run and recheck test results as you work.