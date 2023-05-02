Download Link: https://assignmentchef.com/product/solved-comp1012-lab3
<br>
Create a text file whose contents has one number per line. The file should look something line:

<pre><code>122334455667429001</code></pre>

Create a program that reads in the text file (you can hardcode the text filename into your program), computes the number of numbers in the file and the sum of all the numbers that are in the file. Then your program should print the number of numbers in the file and their sum.

Your output should look something like:

<pre><code>Number of numbers: 8Total: 9280</code></pre>

<h2 id="exercise-2-sum-of-digits">Exercise 2: sum of digits</h2>

In class we’ve seen a <code>for</code> loop used to iterate over lines in a file. A <code>for</code> loop can actually be used to iterate over <strong>any</strong> sequence of values, so that also includes <code>list</code> and <code>str</code> types.

First, experiment a bit with the <code>for</code> loop – what happens when you write a for loop that iterates over a <code>str</code>?

Once you’ve worked this out, write a program that will prompt the user for a positive whole number. Using a <code>for</code> loop, calculate the number of digits and the sum of digits.

Your output should look something like (<mark>highlighted</mark> text means the user typed this in):

<pre>Provide a number: <mark>321</mark>There are 3 digits and the sum of the digits is 6.</pre>

<hr>

<h2 id="optional-sanitize-a-string">Optional : Sanitize a string</h2>

Ask for a string from the user. Do the following operations:

<ol type="1">

 <li>Remove leading and trailing whitespace by using <a href="https://www.tutorialspoint.com/python3/string_strip.htm"><code>strip()</code></a>.</li>

 <li>Remove characters: <code>~</code>, <code>!</code> and <code>-</code> by using <a href="https://www.tutorialspoint.com/python3/string_replace.htm"><code>replace()</code></a>.</li>

</ol>

Report the sanitized string back to the user.

Your output should look something like (<mark>highlighted</mark> text means the user typed this in, note here the spaces before and after the characters in the string):

<pre>Please input a string: <mark>    Hello - my name is Earl!    </mark>Sanitized string: Hello  my name is Earl</pre>

<h2 id="optional-volume-of-a-cone">Optional: Volume of a cone</h2>

Calculate the volume of a cone, given user input.

Prompt the user for the radius of the cone, and the height of the cone.

The equation to calculate the volume of a cone is:

<span class="math display"><em>V</em> = <em>π</em><em>r</em><sup>2</sup>(<em>h</em>/3)</span>

Report the volume to the user with two decimal places of precision.

Your output should look something like (<mark>highlighted</mark> text means the user typed this in):

<pre>What is the radius of your cone (in cm)?  <mark>12</mark>What is the height of your cone (in cm)?  <mark>30</mark>The volume is 4523.89cm^2</pre>

<h2 id="optional-binary-to-decimal">Optional: Binary to Decimal</h2>

Write a program that will prompt the user for a binary number (0s and 1s only) and convert that number to a decimal (base 10) integer.

Binary numbers are base 2 numbers that use only two digits to represent a number, 0 and 1. We can freely convert between decimal and binary using <code>log</code>, but we’re going to convert between these two bases using basic arithmetic and loops in Python.

As an example, in base 10 we can decompose a number into a set of products of powers of 10.

<pre><code>5629|||└  9 * 10**0 (ones place)||└-  2 * 10**1 (tens place)|└--  6 * 10**2 (hundreds place)└---  5 * 10**3 (thousands place)</code></pre>

You can calculate the number by a summation of each digit:

<span class="math display">decimalValue = 9 × 10<sup>0</sup> + 2 × 10<sup>1</sup> + 6 × 10<sup>2</sup> + 5 × 10<sup>3</sup></span>

In binary, we can decompose a number into a set of products of powers of two:

<pre><code>1001|||└  1 * 2**0 (ones place)||└-  0 * 2**1 (twos place)|└--  0 * 2**2 (fours place)└---  1 * 2**3 (eights place)</code></pre>

We can convert a binary number by calculating by a summation of the digits multiplied by powers of two represented by their place:

<span class="math display">decimalValue = 1 × 2<sup>3</sup> + 0 × 2<sup>2</sup> + 0 × 2<sup>1</sup> + 1 × 2<sup>0</sup></span>

Use a <code>for</code> to convert each bit into a decimal number. Have a running sum in your loop to do the summation.

Your output should look something like (<mark>highlighted</mark> text means the user typed this in):

<pre>Please input a binary number &gt; <mark>101010</mark>The number in decimal is 42.</pre>

Things to think about:

<ol type="1">

 <li>What should the <strong>first</strong> power of 2 be? In our example it was 3, how would we represent that more generally based on something we can figure out about the <code>str</code> that was entered? (hint: we need to call a function!)</li>

 <li>When looping over a <code>str</code> with a <code>for</code> loop, in what <em>order</em> are we iterating over values? That is, in terms of a string written out in the example, are we going from right to left or from left to right?</li>

</ol>

<span class="kksr-muted">Rate this product</span>