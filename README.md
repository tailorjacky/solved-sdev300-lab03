Download Link: https://assignmentchef.com/product/solved-sdev300-lab03
<br>
<strong>Introduction to PHP </strong>

<strong>Overview </strong>

This lab walks you through using PHP to create simple applications. PHP is popular for many Web applications, so becoming comfortable with the syntax of PHP will help you diagnose and identify potential security issues.

<strong>Learning Outcomes: </strong>

At the completion of the lab you should be able to:

<ol>

 <li>Execute PHP scripts within the AWS Cloud VM</li>

 <li>Create simple PHP applications comprised of basic syntax, variables, strings, selection statements and repetition statements.</li>

</ol>

<strong> </strong>

<strong>Lab Submission Requirements: </strong>

After completing this lab, you will submit a word (or PDF) document that meets all of the requirements in the description at the end of this document. In addition, your PHP file should be submitted. You should submit multiple files in a zip file.

<strong> </strong>

<strong>Virtual Machine Account Information </strong>

Your Virtual Machine has been preconfigured with all of the software you will need for this class. You have previously connected to this machine in the previous labs. Reconnect again using the Remote Desktop connection, your Administrator username and password.




<strong>Part 1 – Execute PHP scripts at the shell prompt within the AWS Cloud VM </strong>

The Virtual Machine already has PHP installed. It is also configured to run properly on your Apache web server. This exercise will walk through creating a simple PHP script and running from a Web browser. We will use the notepad++ text editor to create the PHP file.




<ol>

 <li>Assuming you have already launched and logged into your AWS Cloud VM, click on the notepad++ icon found on the left side of the screen of your VM as shown in figure 1.</li>

</ol>




<ol start="2">

 <li>To create a new document just begin typing or copying and pasting the PHP code shown below:</li>

</ol>

&lt;!– Simple Hello, World PHP Script

Date: Jan 01, XXXX

Author: Dr. Robertson

Title: HelloSDEV300.php  description: Print Hello greeting

–&gt;

&lt;!DOCTYPE html&gt;

&lt;!– HelloPHP.html –&gt;

&lt;!– Jan 22, XXXX –&gt;

&lt;html&gt;

&lt;head&gt;

&lt;title&gt;My First PHP Script &lt;/title&gt;

&lt;/head&gt;

&lt;body&gt;

&lt;h1&gt;Welcome to SDEV 300. &lt;/h1&gt;

&lt;h1&gt;The following greeting is from PHP &lt;/h1&gt;

&lt;?php

echo “Hello, SDEV 300 students and class!&lt;/br&gt;”;     echo “The current time is ” . date(“g:i:h a”); ?&gt;

&lt;p&gt;

&lt;/body&gt;

&lt;/html&gt;

Save the file in the C:Bitnamiwampstack-7.1.16-0apache2htdocsSDEV300 folder in a file named HelloSDEV300.php. Recall the C:Bitnamiwampstack-7.1.16-0apache2htdocsis the location of the Apache web server html files. (See figure 2).







<em>Figure 2 Saving the Hello, World PHP File </em>

As shown in figure 3, launch the Firefox browser and run your home page by entering the following URL: localhost/SDEV300/HelloSDEV300.php.




<em>Figure 3 Launching the PHP Application </em>

<ol start="3">

 <li>We can take the Web page we created in week 2 and add some additional PHP components. Copy and paste the following PHP file into your text editor and save the file as CShome.php in the SDEV300 folder.</li>

</ol>




&lt;!DOCTYPE html&gt;

&lt;!– CShome.php –&gt;

&lt;!– Jan 22, XXXX –&gt;

&lt;html&gt;

&lt;head&gt;

&lt;title&gt;Computer Security Home Page &lt;/title&gt;

&lt;/head&gt;

&lt;body&gt;

&lt;h1&gt;Welcome to Computer Security Consultants! &lt;/h1&gt;

&lt;p&gt; &lt;?php

echo “Hello, SDEV 300 students and class!&lt;/br&gt;”;     echo “The current time is ” . date(“g:i:h a”);

?&gt;

&lt;!– Add Table of Hyperlinks –&gt;

&lt;p&gt;

Click on any link in the table below to see some of our current customers:

&lt;/p&gt;

&lt;table border = “1”&gt;

&lt;tr&gt;&lt;td&gt;Site&lt;/td&gt;&lt;td&gt;Web Address&lt;/td&gt;&lt;/tr&gt;

&lt;tr&gt;&lt;td&gt;UMUC&lt;/td&gt;&lt;td&gt;&lt;a href=”http://umuc.edu”&gt;UMUC&lt;/a&gt;&lt;/td&gt;&lt;/tr&gt;

&lt;tr&gt;&lt;td&gt;Oracle&lt;/td&gt;&lt;td&gt;&lt;a href=”http://oracle.com”&gt;Oracle&lt;/a&gt;&lt;/td&gt;&lt;/tr&gt;

&lt;tr&gt;&lt;td&gt;Microsoft&lt;/td&gt;&lt;td&gt;&lt;a href=”http://www.

microsoft.com”&gt;Microsoft&lt;/a&gt;&lt;/td&gt;&lt;/tr&gt; &lt;tr&gt;&lt;td&gt;Twitter&lt;/td&gt;&lt;td&gt;&lt;a href=”http://www. twitter.com”&gt;Twitter&lt;/a&gt;&lt;/td&gt;&lt;/tr&gt;

&lt;/table&gt;




&lt;!– Add some images in a table –&gt;

&lt;p&gt;

Check out our latest Mars photos:

&lt;/p&gt;

&lt;table&gt;

&lt;tr&gt;&lt;td&gt;Description&lt;/td&gt;&lt;td&gt;Photo&lt;/td&gt;&lt;/tr&gt; &lt;tr&gt;&lt;td&gt;Mars Near Darwin&lt;/td&gt;&lt;td&gt;&lt;img

src=”http://mars.jpl.nasa.gov/msl/images/mars-curiosity-rover-mount-sharppia19083-Sol387-br2.jpg” width=”300″ height=”150″/&gt;&lt;/td&gt;&lt;/tr&gt;

&lt;tr&gt;&lt;td&gt;Mars Parhump Hills&lt;/td&gt;&lt;td&gt;&lt;img

src=”http://mars.jpl.nasa.gov/msl/images/mars-curiosity-rover-pahrump-hillsrock-outcrop-pia19075-br2.jpg” width=”300″ height=”150″/&gt;&lt;/td&gt;&lt;/tr&gt;

&lt;/table&gt;




&lt;p&gt;

We offer the following products:

&lt;ul&gt;

&lt;li&gt;Security Consulting &lt;/li&gt;

&lt;li&gt;Apache security monitoring&lt;/li&gt;

&lt;li&gt;Software Penetration Testing&lt;/li&gt;

&lt;li&gt;Threat Modeling and Risk Managements &lt;/li&gt;

&lt;/ul&gt;

&lt;/p&gt;




&lt;!– Add a Form –&gt;

&lt;p&gt; Tell us about yourself and what you are interested in doing:

&lt;form action=”” method=”post”&gt;

Name: &lt;input type=”text” name=”username”&gt;&lt;/br&gt;

E-Mail: &lt;input type=”text” name=”e-mail”&gt;&lt;br/&gt;

Interest: &lt;select name=”sport”&gt;

&lt;option&gt;Apache Security Monitoring&lt;/option&gt;

&lt;option&gt;Security Consulting&lt;/option&gt;

&lt;option&gt;Software Penetration Testing&lt;/option&gt;

&lt;option&gt;Threat Modeling and Risk Management&lt;/option&gt;

&lt;/select&gt;

&lt;br/&gt;&lt;br/&gt;




&lt;input type=”submit” value=”Click to Submit”/&gt;

&lt;input type=”reset” value=”Reset”/&gt;

&lt;/form&gt;

&lt;/p&gt;




&lt;/body&gt;

&lt;/html&gt;




<ol start="4">

 <li>Launching the PHP file within Browser will result in the following output.</li>

</ol>




<em>Figure 4 Combining PHP and HTML </em>




Notice the Web page we created from previous week has the PHP welcome message at the top of the page. Combining PHP code and HTML to make dynamic web pages is just that easy. The key is to make sure you properly tag your PHP components. Notice, the use of the following PHP tags:

&lt;?php




?&gt;




The &lt;?php starts the PHP code, while ?&gt; ends the PHP code. Be sure all of your PHP specific commands are inside of those tags. Those tags tell PHP to start and stop interpreting the code between them. Everything outside of a pair of opening and closing tags is ignored by the PHP parser. Now, you can easily integrate those tags within existing HTML to add life to your web pages.

The next section of this lab, illustrates additional PHP functionality. Don’t let the newness of PHP bother you. You have coded in Java and probably other languages already. PHP is just another programming language with similar functionality and slightly different syntax.




<strong>Part 2 Create simple PHP applications </strong>

The reading for this week covered the basic syntax of PHP, variable definitions, operators and expressions, decision and loops and strings. As you review these readings, be sure to copy and paste code to create files to test functionality. Also, be sure to modify, enhance and experiment with the code to better understand what each line of code is doing. Use the php.net manual to better understand additional options and functionality available in PHP. The examples provided are just a subset of what PHP can do. With experimentation and time, you will become quite comfortable understanding how to use and analyze PHP code.




Here are some critical PHP syntax components and examples to help expedite learning the language:

<ol>

 <li>Use a semi-colon (;) to terminate PHP statements:</li>

</ol>

&lt;?php

echo ‘Statements end with a semi-colon’;

?&gt;

<ol start="2">

 <li>Comments are important for documenting the code you create in any programming language. C, Java and C++ style comments as well as Unix-shell Perl comments are accepted. Consider the following examples:</li>

</ol>

// A one-line c++ style comment

/* A multi line comment

That is too long for one line. */

# A one-line UNIX-shell-style comment

Consistency in programming style is important. I recommend using primarily the single or multi-line C/C++/Java commenting style.

<ol start="3">

 <li>Types are loosely defined in PHP but useful for providing some consistency for variables. The table below lists the more common types in PHP along with an example</li>

</ol>

<table width="580">

 <tbody>

  <tr>

   <td width="70"><strong>Type </strong></td>

   <td width="223"><strong>Description </strong></td>

   <td width="286"><strong>Example </strong></td>

  </tr>

  <tr>

   <td width="70">boolean</td>

   <td width="223">Expresses a truth value. (TRUE or FALSE.) values are case insensitive</td>

   <td width="286">$isValid = True;</td>

  </tr>

  <tr>

   <td width="70">integer</td>

   <td width="223">Expresses a whole number.Decimal, hexadecimal (0x), octal (0) or binary (0b) notation are available. May be optionally preceded by a sign (- or +).</td>

   <td width="286">$count = 6;$octcount = 05;$bincount = 0b0101;$hexcount = 0xf3;</td>

  </tr>

  <tr>

   <td width="70">float</td>

   <td width="223">Expresses a real number (float, double, real). May use e notation.</td>

   <td width="286">$avg = 4.12e5;$std = 16.432;</td>

  </tr>

  <tr>

   <td width="70">string</td>

   <td width="223"> A series of characters. Does not offer Unicode support. May be single of double quoted.</td>

   <td width="286">$lastname = ‘Robertson’;$firstname = “Jim”;</td>

  </tr>

  <tr>

   <td width="70">array</td>

   <td width="223">An ordered map aligning key pairs. Can be a simple list, trees, hash tables, collections and other data structures. Arrays of arrays are also possible.</td>

   <td width="286">$majors = array(“CMSC”, “SDEV”,“CMIT”, “CMST”);$capstones = array(“CMSC” =&gt; “Capstone A”,“SDEV” =&gt; “Capstone B”, );</td>

  </tr>

  <tr>

   <td width="70">object</td>

   <td width="223">An object to store functions and variables.</td>

   <td width="286">class car {var $speed=20.2; function get_speed() {     return $this-&gt;speed;}}// Create and use the Car$mycar = new car;$myspeed = $mycar-&gt;get_speed(); echo ‘myspeed is ‘ . $myspeed;</td>

  </tr>

 </tbody>

</table>




When experimenting with PHP types, be sure to include the code within the PHP start and end tags. If not, the PHP won’t know what to process. For example, for the car object, the following makes the code useful within a Web file or stand-along PHP command script.

&lt;?php class car {     var $speed=20.2;




function get_speed() {     return $this-&gt;speed;

}

}




$mycar = new car;

$myspeed = $mycar-&gt;get_speed(); echo ‘myspeed is ‘ . $myspeed;

?&gt;




Arrays can be declared and initialized with data.

For a single dimensional array, the declaration and initialization is fairly straight forward:

$numbers = array( 11,43,4,5,7,10);




For a multi-dimensional associative array the syntax is trickier:

$gpa=array(        array(

“student”=&gt;”Joe Smith”,

“grade” =&gt;”A”

),        array(

“student”=&gt;”Mary Jones”,

“grade” =&gt;”A”

),         array(

“student”=&gt;”John Perry”,

“grade” =&gt;”C”

),

);

Notice the use of a nested array statements and use of =&gt; to associate a value for array element.




<ol start="4">

 <li>Variables in PHP start with a dollar sign ($). Variables are case sensitive and must start with a letter or underscore, followed by any number of letters, numbers, or underscores.</li>

</ol>

Global variables are possible within PHP but are discouraged from being used. A variable defined within a function has scope to the function where it was defined. Variables defined outside functions are available to all other functions within PHP defined class or file but maybe extended to other included files as well.




<ol start="5">

 <li>Constants are identifiers whose values cannot be changed after being defined initially. Constants may be defined using the “define” reserved word or the const as shown below: define(“SCHOOLNAME”, “UMUC”); define(“AVAGADROS”, 6.022e-23); const HI = ‘Hello World
’;</li>

</ol>




To use the constants just type in the defined constant name along with the print or display option:

echo SCHOOLNAME; $mymole = 10.2*AVAGADROS; echo $mymole; print HI;

<ol start="6">

 <li>An operator takes one or more values and provides another value. Operators include arithmetic, assignment, relational, comparison, logical and others. The operator precedence is similar to most other modern programming languages with parenthesis taking highest priority, followed by increment and decrement, logical not, arithmetic operators and more. The details are found in the php.net manual available here: <a href="https://php.net/manual/en/language.operators.precedence.php">http://php.net/manual/en/language.operators.precedence.php</a></li>

</ol>

In all cases, logic and functionality should always be fully tested to make sure complex nested operators are being interpreted as you believe.

Arithmetic operators include +, -, *, / and %.

Table 2 illustrates an example of each Arithmetic operator.

<table width="588">

 <tbody>

  <tr>

   <td width="125"><strong>Operator </strong></td>

   <td width="463"><strong>Example </strong></td>

  </tr>

  <tr>

   <td width="125">Addition (+)</td>

   <td width="463">$num3 = $num1 + $num2;</td>

  </tr>

  <tr>

   <td width="125">Subtraction (-)</td>

   <td width="463">$num3 = $num1 – $num2;</td>

  </tr>

  <tr>

   <td width="125">Multiplication (*)</td>

   <td width="463">$num3 = $num1 * $num2;</td>

  </tr>

  <tr>

   <td width="125">Division (/)</td>

   <td width="463">$num3 = $num1 / $num2;</td>

  </tr>

  <tr>

   <td width="125">Modulo (%)</td>

   <td width="463">$num3 = $num1 % $num2; (Returns the remainder of$num1/$num2)</td>

  </tr>

  <tr>

   <td width="125">Exponent (**)</td>

   <td width="463">$num3 = $num1 ** $num2;  (Raises $num1 to $num2 power)</td>

  </tr>

 </tbody>

</table>




Assignment operators use the equals (=) sign. For example:

$num3 = $num1 + $num2;

Shortcuts are also available providing the combination of assignments and an operator. For example, the following code will takes the existing value of $num2 and adds $num1 to it.

$num2 += $num1;

This is equivalent to:

$num2 = $num2 + $num1;

Identical functionality is available for other arithmetic operators as well as most other binary operators.

Bitwise operators of &amp;,|, ^, ~, &lt;&lt;, and &gt;&gt; are also available for AND, OR, Xor, Not, Left-shift and rightshift; respectively. Bitwise operators work at the bit level. Bitwise operators are handy for fast arithmetic computation.

Comparison operators allow you to compare two variables and determine their equality or lack thereof.

Table 3 shows the commonly used comparison operators in PHP. Note the use of !== and === that include the test to see if the two variables are of the same type as well as the same value.

<table width="588">

 <tbody>

  <tr>

   <td width="151"><strong>Comparison </strong></td>

   <td width="127"><strong>Example </strong></td>

   <td width="310"><strong>Results </strong></td>

  </tr>

  <tr>

   <td width="151">Equal</td>

   <td width="127">$a==$b</td>

   <td width="310">TRUE if $a is equal to $b after type juggling.</td>

  </tr>

  <tr>

   <td width="151">Identical</td>

   <td width="127">$a===$b</td>

   <td width="310">TRUE if $a is equal to $b, and they are of the same type.</td>

  </tr>

  <tr>

   <td width="151">Not Equal</td>

   <td width="127">$a!=$b or$a&lt;&gt;$b</td>

   <td width="310">TRUE if $a is not equal to $b after type juggling.</td>

  </tr>

  <tr>

   <td width="151">Not identical</td>

   <td width="127">$a!==$b</td>

   <td width="310">TRUE if $a is not equal to $b, or they are not of the same type.</td>

  </tr>

  <tr>

   <td width="151">Less than</td>

   <td width="127">$a&lt;$b</td>

   <td width="310">TRUE if $a is strictly less than $b.</td>

  </tr>

  <tr>

   <td width="151">Greater than</td>

   <td width="127">$a&gt;$b</td>

   <td width="310">TRUE if $a is strictly greater than $b.</td>

  </tr>

  <tr>

   <td width="151">Less than or Equal</td>

   <td width="127">$a&lt;=$b</td>

   <td width="310">TRUE if $a is less than or equal to $b.</td>

  </tr>

  <tr>

   <td width="151">Greater than or Equal</td>

   <td width="127">$a&gt;=$b</td>

   <td width="310">TRUE if $a is greater than or equal to $b.</td>

  </tr>

 </tbody>

</table>




Pre- and post-increments as well as pre- and post-decrements are available using the ++ and — operators placed either before or after the variable name. These operators work identically in most programming languages. The following examples further clarifies the functionality.

<table width="390">

 <tbody>

  <tr>

   <td width="48">++$a</td>

   <td width="342">Pre-increment- Increments $a by one, then returns $a.</td>

  </tr>

  <tr>

   <td width="48">$a++</td>

   <td width="342">Post-increment- Returns $a, then increments $a by one.</td>

  </tr>

  <tr>

   <td width="48">–$a</td>

   <td width="342">Pre-decrement- Decrements $a by one, then returns $a.</td>

  </tr>

  <tr>

   <td width="48">$a–</td>

   <td width="342">Post-decrement-Returns $a, then decrements $a by one.</td>

  </tr>

 </tbody>

</table>




Logical operators are used for comparison and include AND, OR, NOT, and XOR. Both symbolic and string versions are available as shown in table 3.

Table 3. Logical Operators

<table width="504">

 <tbody>

  <tr>

   <td width="67"><strong>Logical  </strong></td>

   <td width="155"><strong>Example </strong></td>

   <td width="282"><strong>Results </strong></td>

  </tr>

  <tr>

   <td width="67">And</td>

   <td width="155">$a and $b</td>

   <td width="282">TRUE if both $a and $b are TRUE.</td>

  </tr>

  <tr>

   <td width="67">Or</td>

   <td width="155">$a or $b</td>

   <td width="282">TRUE if either $a or $b is TRUE.</td>

  </tr>

  <tr>

   <td width="67">XOR</td>

   <td width="155">$a xor $b</td>

   <td width="282">TRUE if either $a or $b is TRUE, but not both.</td>

  </tr>

  <tr>

   <td width="67">Not</td>

   <td width="155">! $a</td>

   <td width="282">TRUE if $a is not TRUE.</td>

  </tr>

  <tr>

   <td width="67">&amp;&amp;</td>

   <td width="155">$a &amp;&amp; $b</td>

   <td width="282">TRUE if both $a and $b are TRUE.</td>

  </tr>

  <tr>

   <td width="67">||</td>

   <td width="155">$a || $b</td>

   <td width="282">TRUE if either $a or $b is TRUE.</td>

  </tr>

 </tbody>

</table>




Note the precedence of &amp;&amp;, || is higher than And, Or. In most cases it is recommended to use the symbolic representation of &amp;&amp; and ||.

String operators include “.” and “.=”. Both are useful for concatenating two strings. For example the following PHP code results in concatenating “Welcome ” and “to SDEV 300.”

$str1 = “Welcome ”;

$str2 = “to SDEV 300.”;

$str3 = $str1 . $str2;




<ol start="7">

 <li>Control Structures such selection and repetitions statements are available within PHP.</li>

</ol>




There are multiple options to select when using control structures. For consistency in style it is recommended to use the structures you are most comfortable if they provide the desired functionality. For example, for loops are very functional and could be used instead of while loops. Table 4 shows popular control structures along with an example. Experiment with these and other control structures available in the PHP manual.




Table 4. PHP control structures

<table width="648">

 <tbody>

  <tr>

   <td width="208"><strong>Control </strong></td>

   <td width="440"><strong>Example</strong></td>

  </tr>

  <tr>

   <td width="208">if/else</td>

   <td width="440">if ($a &gt; $b) {echo “a is greater than b”;} else {echo “a is NOT greater than b”; }</td>

  </tr>

  <tr>

   <td width="208">else if/else</td>

   <td width="440">if ($a &gt; $b) {echo “a is bigger than b”;} elseif ($a == $b) {     echo “a is equal to b”;} else {echo “a is smaller than b”; }</td>

  </tr>

  <tr>

   <td width="208">while</td>

   <td width="440">$i = 1;while ($i &lt;= 10) {     echo $i++;   }</td>

  </tr>

  <tr>

   <td width="208">do-while</td>

   <td width="440">$i = 0; do {echo $i; } while ($i &gt; 0);</td>

  </tr>

  <tr>

   <td width="208">for</td>

   <td width="440">for ($i = 1; $i &lt;= 10; $i++) {     echo $i;}</td>

  </tr>

  <tr>

   <td width="208">foreach</td>

   <td width="440">$a = array(1, 2, 3, 17); foreach ($a as $v) {echo “Current value of $a: $v.
”; }</td>

  </tr>

  <tr>

   <td width="208">switch</td>

   <td width="440">switch ($i) {     case 0:echo “i equals 0”;         break;     case 1:echo “i equals 1”;         break;     case 2:         echo “i equals 2”;break;}</td>

  </tr>

 </tbody>

</table>




The functionality is not unlike what you have used in Java and C in previous courses. However; be sure to use $ for the variable names as this syntax looks different than other languages although the functionality is the same.




<ol start="8">

 <li>Functions are critical to any programming language. PHP includes both user-defined and built-in functions. In both cases, the functions may use input parameters and return values.</li>

</ol>

Functions help organize your code and provide more portability and potential future code reuse in other projects or applications. When possible, use functions regardless of the programming language.

The following is a user defined function to calculate the area of a rectangle:

function calcRectArea($len, $width)

{

echo “Calling Rectangle Area.
”;     return $len*$width;

}




To call the function the following PHP code would work:

$myLen = 4.2;

$myWidth = 8.7;

$myArea = calcRectArea($myLen, $myWidth);










Function names are case insensitive, however for consistency, programmers should follow a programming style for naming functions. Similar to other programming languages, recursive functions are possible and used as appropriate.

Multiple built-in functions are available within the core PHP installation and additional useful functions are available as packages are installed. Although just a minor subset of String and Math built-in functions, table 5 provides a list of useful built-in functions:

Table 5. PHP built-in function examples

<table width="623">

 <tbody>

  <tr>

   <td width="312"><strong>Function </strong></td>

   <td width="312"><strong>Example call </strong></td>

  </tr>

  <tr>

   <td width="312">strlen – get the string length</td>

   <td width="312">$str = ‘SDEV300’;$myStr =  strlen($str);</td>

  </tr>

  <tr>

   <td width="312">strrev — Reverse a string</td>

   <td width="312">$str = ‘SDEV300’; strrev(“Hello world!”);</td>

  </tr>

  <tr>

   <td width="312">strtoupper — Make a string uppercase</td>

   <td width="312">$str = ‘Welcome Students!’;$str = strtoupper($str);</td>

  </tr>

  <tr>

   <td width="312">trim — Strip whitespace (or other characters) from the beginning and end of a string</td>

   <td width="312">$str = ‘   Welcome Students!  ‘;$trimmed = trim($text);</td>

  </tr>

  <tr>

   <td width="312">str_shuffle — Randomly shuffles a string</td>

   <td width="312">$str = ‘SDEV300’;$shuffled = str_shuffle($str);</td>

  </tr>

  <tr>

   <td width="312">floor — Round fractions down</td>

   <td width="312">echo floor(8.6); // Prints 8</td>

  </tr>

  <tr>

   <td width="312">dechex — Decimal to hexadecimal</td>

   <td width="312">echo dechex(16);</td>

  </tr>

  <tr>

   <td width="312">sqrt — Square root</td>

   <td width="312">echo sqrt(9);</td>

  </tr>

 </tbody>

</table>




You should review and use the php.net manual to look-up additional useful math, string and other PHP functions as needed. For example, the following URLs take you to the String and Math function definitions:

<a href="https://php.net/manual/en/ref.math.php">http://php.net/manual/en/ref.math.php</a>

<a href="https://php.net/manual/en/ref.strings.php">http://php.net/manual/en/ref.strings.php</a>




The following is another PHP function example that calls a user-defined function named cubeIt() and two built-in math functions.

&lt;!– PHP and Functions

Date: Jan 01, XXXX

Author: Dr. Robertson  Title: FunctionsDemo.php

description: Demo how to use Functions in PHP

–&gt;

&lt;!DOCTYPE html&gt;

&lt;html&gt;

&lt;head&gt;

&lt;title&gt;Functions Demo &lt;/title&gt;

&lt;/head&gt;

&lt;body&gt;

&lt;h1&gt;PHP Functions Demo &lt;/h1&gt;

&lt;?php

// Create a simple array of Degrees

$numbers = array( 15,30,45,75,90);




echo “&lt;h3&gt; Example PHP Functions &lt;/h3&gt;”; // Create a table and display the numbers




echo “&lt;table border=’1′&gt;”; echo “&lt;tr&gt;

&lt;th&gt;Degree &lt;/th&gt;

&lt;th&gt; Sqrt(Degree) &lt;/th&gt;

&lt;th&gt; sin(Degree) &lt;/th&gt;

&lt;th&gt; cos(Degree) &lt;/th&gt;

&lt;th&gt; tan(Degree) &lt;/th&gt;

&lt;th&gt; cubeIt(Degree) &lt;/th&gt;

&lt;/tr&gt;”;

foreach ( $numbers as $val ) {     echo “&lt;tr&gt;”;

echo “&lt;td&gt;” . $val . “&lt;/td&gt;”;     echo “&lt;td&gt;” . sqrt($val). “&lt;/td&gt;”;     echo “&lt;td&gt;” . sin(deg2rad($val)). “&lt;/td&gt;”;     echo “&lt;td&gt;” . cos(deg2rad($val)). “&lt;/td&gt;”;     echo “&lt;td&gt;” . tan(deg2rad($val)). “&lt;/td&gt;”;     echo “&lt;td&gt;” . cubeIt($val). “&lt;/td&gt;”;     echo “&lt;/tr&gt;”;

}

echo “&lt;/table&gt;”;




// Simple Cube function

// Return the cube of the input value  function cubeIt($val) {           return $val*$val*$val;

}




?&gt;

&lt;/body&gt;

&lt;/html&gt;







Reviewing the above code you should note the following:

<ol>

 <li>Built-in PHP functions can be used easily by calling the function name and any required parameters. For this example, sqrt(), deg2rad(), sin(), cos() and tan() existing functions were called.</li>

 <li>PHP functions you create should be of the format:</li>

</ol>

function functionName($parameter1, $parameter2 …) {

// Code here         return $returnvalue;

}

<ol>

 <li>You can create functions with any level of rigor and complexity as needed to solve the computing problem at hand. The simple PHP function provided for this example calculates the cube of the input parameter:</li>

</ol>

function cubeIt($val) {           return $val*$val*$val;

}







In this exercise we will create a PHP web page that displays the multiplication table using a nested, for loop. HTML table tags will be used to format the data values.







<ol>

 <li>Copy and paste the following code into a file named MultiplicationTable.php in the SDEV300 folder within the Apache2 location on your Virtual Machine.</li>

</ol>

&lt;!DOCTYPE html PUBLIC “-//W3C//DTD XHTML 1.0 Strict//EN” &gt;

&lt;html&gt;

&lt;head&gt;

&lt;title&gt;Multiplication Table&lt;/title&gt;

&lt;/head&gt;

&lt;body&gt;

&lt;h1&gt; Week 3 PHP and HTML Blending &lt;/h1&gt;

&lt;h2&gt;Multiplication Table&lt;/h2&gt;




&lt;!– First part of table –&gt;

&lt;table border=”1″&gt;

&lt;tr&gt;

&lt;td&gt;X&lt;/td&gt;

&lt;td&gt;1&lt;/td&gt;

&lt;td&gt;2&lt;/td&gt;

&lt;td&gt;3&lt;/td&gt;

&lt;td&gt;4&lt;/td&gt;

&lt;td&gt;5&lt;/td&gt;

&lt;td&gt;6&lt;/td&gt;

&lt;td&gt;7&lt;/td&gt;

&lt;td&gt;8&lt;/td&gt;

&lt;td&gt;9&lt;/td&gt;

&lt;td&gt;10&lt;/td&gt;

&lt;/tr&gt;







&lt;!– Notice interweaving of PHP and HTML –&gt;

&lt;?php

$iterations = 10;

// Nested for loop to calculate product




for ( $num1=1; $num1 &lt;= $iterations; $num1++ ){

?&gt;

&lt;tr&gt;&lt;td&gt;&lt;?php echo $num1;?&gt;&lt;/td&gt;

&lt;?php

for ( $num2=1; $num2 &lt;= $iterations; $num2++ ){

$product = $num1 * $num2;

?&gt;




&lt;td&gt;&lt;?php echo $product;?&gt; &lt;/td&gt;

&lt;?php

}

?&gt;

&lt;/tr&gt;

&lt;?php

}

?&gt;




&lt;/table&gt;




&lt;p&gt;

&lt;h3&gt;A quote from Edgar Allan Poe&lt;/h3&gt;

&lt;?php

// Add a string for manipulation

$poequote = “I have no faith in human perfectability. I think    that human exertion will have no appreciable effect upon humanity.   Man is now only more active – not more happy – nor more wise, than   he was 6000 years ago.”;   echo $poequote;

?&gt;

&lt;p&gt;

&lt;h3&gt;Quote modified with ucwords &lt;/h3&gt;

&lt;?php

// Make Uppercase for first letter    $newquote = ucwords($poequote);

echo $newquote;

?&gt;




&lt;/body&gt;

&lt;/html&gt;

Figure shows the PHP file created in notepad++ on the AWS Cloud VM.




<em>Figure 5 Multiplication Table PHP file. </em>




<ol start="2">

 <li>Using your AWS Cloud VM, launch your Firefox browser and run the Web application using the localhost/SDEV300/MultiplicationTable.php</li>

</ol>

If successful, the resulting output will look similar to the screen shown in figure 6.




<em>Figure 6 Running the MultiplicationTable.php file </em>




<ol start="3">

 <li>Reviewing the code you should note the following:

  <ol>

   <li>PHP codes start and stop with &lt;?php ?&gt;. This can get tricky to do by hand but for simple applications keeping track of the opening and closing braces is feasible.</li>

   <li>HTML code is interleaved between the PHP code. You will need to make sure you have a complete table structure between the PHP code. For example, the following HTML code is within a PHP loop to echo the data into just one cell. &lt;td&gt;&lt;?php echo $product;?&gt;</li>

  </ol></li>

</ol>

&lt;/td&gt;

<ol>

 <li>Adding ending braces for loops can be challenging. If you do this by hand, be sure to write your loops first, and then integrate the HTML tags. This will help you avoid infinite loops. The following is a typical listing for a table built using PHP loops. You should take your time walking through this code to see the complete structure and how PHP is used to provide for looping and dynamic programming.</li>

</ol>

&lt;!– First part of table –&gt;

&lt;table border=”1″&gt;

&lt;tr&gt;

&lt;td&gt;X&lt;/td&gt;

&lt;td&gt;1&lt;/td&gt;

&lt;td&gt;2&lt;/td&gt;

&lt;td&gt;3&lt;/td&gt;

&lt;td&gt;4&lt;/td&gt;

&lt;td&gt;5&lt;/td&gt;

&lt;td&gt;6&lt;/td&gt;

&lt;td&gt;7&lt;/td&gt;

&lt;td&gt;8&lt;/td&gt;

&lt;td&gt;9&lt;/td&gt;

&lt;td&gt;10&lt;/td&gt;

&lt;/tr&gt;







&lt;!– Notice interweaving of PHP and HTML –&gt;

&lt;?php

$iterations = 10;

// Nested for loop to calculate product




for ( $num1=1; $num1 &lt;= $iterations; $num1++ ){

?&gt;

&lt;tr&gt;&lt;td&gt;&lt;?php echo $num1;?&gt;&lt;/td&gt;

&lt;?php

for ( $num2=1; $num2 &lt;= $iterations; $num2++ ){

$product = $num1 * $num2;

?&gt;




&lt;td&gt;&lt;?php echo $product;?&gt; &lt;/td&gt;

&lt;?php

}

?&gt;

&lt;/tr&gt;

&lt;?php

}

?&gt;

&lt;/table&gt;




<strong>Lab submission details: </strong>

As part of the submission for this Lab, you will create your own Web page that uses both HTML and PHP to create several different tables providing specific information. You will get a chance to use most of the concepts you studied so far in this course as you will apply both HTML and PHP code to this exercise. You may enhance your HTML display with CSS style sheets as desired but that is not required.

Specifically, you will create a PHP Web application that provides 2 different tables. You will use your design skills to determine the size and organization of the resulting tables.

The first table should include the results of using PHP to calculate several mathematical and trigonometric functions. Specifically, the following formulas should be implemented as f<strong>unctions</strong> in PHP:

x    slope-intercept equation for a line:   y = mx+b x Surface Area of Sphere: A = 4SR<sup>2</sup>

x    Distance an object travels for given velocity and time : d = vt

The values used for each of the formulas are as follows:

<table width="606">

 <tbody>

  <tr>

   <td width="208"><strong>Shape </strong></td>

   <td width="398"><strong>Values and parameters </strong></td>

  </tr>

  <tr>

   <td width="208">Slope intercept calculate y</td>

   <td width="398">x={2,5,8,10} for m=-2; b=0;</td>

  </tr>

  <tr>

   <td width="208">Surface Area of Sphere A</td>

   <td width="398">R = {2,6,10, 100,1000};</td>

  </tr>

  <tr>

   <td width="208">Distance object travels: d</td>

   <td width="398">v={10m/s, 30m/s, 327m/s, 1200 m/s} for time from 0 to 10 in steps of 0.5 seconds.</td>

  </tr>

 </tbody>

</table>




Note, you will have multiple results for each formula. Organize the results in an HTML table of dimensions of your choice. The results should clearly provide the formula used and the input and output results for each formula in the table.

Also, be sure to define the formulas as PHP function and call the functions.

The second table should include a famous quote (or quote that you like) and slightly modified versions of that quote using PHP String functions.  You should use existing PHP functionality (e.g. built-in functions) to modify the quote. The modifications are described below:

Note, the quote should be at least 300 characters in length.

<table width="623">

 <tbody>

  <tr>

   <td width="312"><strong>Modification </strong></td>

   <td width="312"><strong>Description </strong></td>

  </tr>

  <tr>

   <td width="312">Original</td>

   <td width="312">Original quote as is</td>

  </tr>

  <tr>

   <td width="312">Capitalize the first letter of each word.</td>

   <td width="312">For example: Hello, I Am A Robot With An AImotivated Brain.</td>

  </tr>

  <tr>

   <td width="312">Displays the word length of each word in the quote separated by commas.</td>

   <td width="312">For example for “My name is Joe.”, the output would be 2, 4, 2, 4 (note the period is counted as part of the last word.</td>

  </tr>

  <tr>

   <td width="312">Randomly shuffles each word in the quote.</td>

   <td width="312">For example for “My name is Joe”, the output might be: yM maen si OJ.e</td>

  </tr>

 </tbody>

</table>




Create screen captures showing the successful running of your application. Be sure to label your screen captures and fully describe them. Each screen capture should clearly show the AWS Cloud VM was used to run the code.

Be sure to appropriately label the output cells for each table to indicate which formula or String function is being.

For your deliverables, you should submit a winzip file containing your word document (or PDF file) with screen captures of the application running successfully along with your PHP web application file.

You should include the Apache log file. <strong>Submissions without access.log files will not be accepted. </strong>

Include your full name, class number and section, date and the professor’s name in the document.

Hints:

<ol>

 <li>Make sure your math calculations, formulas and functions are correct.</li>

 <li>Test everything before submitting.</li>

 <li>Start with the PHP functions and then build the display output around HTML tables that call those functions.</li>

 <li>Use PHP arrays to store your datasets.</li>

 <li>Use for loops (or other repetition) to cycle through the datasets and the String data.</li>

 <li>Use the built-in functions. (e.g. explode() is perfect for some of the String work you will need to do)</li>

 <li>Start early on this project. It will take you longer than you think.</li>

 <li>Ask questions if you get stuck</li>

</ol>




<strong> </strong>