Download Link: https://assignmentchef.com/product/solved-cpsc355-computing-machinery-i-assignment-6
<br>
<strong>File I/O and Floating-Point Numbers </strong>

Write an ARMv8 assembly language program to compute the cube root of positive real numbers using Newton’s method. Use double precision floating-point numbers. The program will read a list of input values from a file whose name is specified at the command line. The input values will be in binary format; each number will be double precision (and thus each is 8 bytes long). Read from the file using system I/O (i.e.

generate an exception using the <em>svc</em> instruction). Process the input values one at a time using a loop (be sure to detect end-of-file correctly), calculate the cube root, and then use printf() to print out the input value and its corresponding cube root in table form (i.e. in columns, with column headings) to the screen. Print out all values with a precision of 10 decimal digits to the right of the decimal point.

Newton’s method requires an initial guess for the cube root; use <em>x</em> = <em>input</em> / 3.0. Compute <em>y</em>, the cube of your current guess <em>x</em>, using <em>y</em> = <em>x</em> * <em>x</em> * <em>x</em>. Then calculate the difference <em>dy</em> between <em>y</em> and the input value:  use <em>dy</em> = <em>y</em> – <em>input</em>. Compute the derivative <em>dy/dx</em> with <em>dy/dx</em> = 3.0 * <em>x</em> * <em>x</em>. Then compute the new trial value for <em>x</em> with <em>x</em> = <em>x</em> – <em>dy</em> / (<em>dy/dx</em>).  Repeat these steps until the error |<em>dy</em>| has been minimized using the formula |<em>dy</em>| &lt; <em>input</em> * 1.0e-10. Put these calculations into a separate function that will be called from your main routine.




Run your program using the input binary file given on D2L. Capture its execution using <em>script</em>.




N<strong>ew Skills needed for this Assignment: </strong>




<ul>

 <li>Use of system I/O (exceptions) to open and read an input binary file</li>

 <li>Understanding and use of floating-point single and double formats</li>

 <li>Use of floating-point instructions to do simple calculations</li>

 <li>Use of floating-point branching instructions</li>

</ul>




<strong>Submit the following: </strong>




<ol>

 <li>Your assembly source code and script via electronic submission. Use the <em>Assignment 6 </em>Dropbox Folder in D2L to submit electronically. Your TA will assemble and run your program to test it. Name your program <em>a6.asm</em> and the script as <em>script.txt</em>.</li>

</ol>


