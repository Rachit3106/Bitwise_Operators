<h1>Experiment 4:</h1>
<h3>Aim: To study and implememt C++ Bitwise Operators.</h3>
<h3>Software used: Visual Studio Code</h3>
<h3>Theory: </h3><h4>Bitwise operator in C++ is used to make changes or perform operations on bits. They work on bit level i.e. 0's and 1's. These operations are faster than arithmetic operations and are mostly used in low level programming.</h4>

<h3>Types of bitwise operators:</h3>
<ol>
  <li>AND(&)</li>
  <li>OR(|)</li>
  <li>NOT(~)</li>
  <li>XOR(^)</li>
  <li>Right Shift Operator (>>)</li>
  <li>Left Shift Operator(<<)</li>
</ol><br>
    
<h3><i>1) AND(&) : </i></h3>
<h4>AND(&) operator compares two integer bits as (0 & 0 --> 0) ; (0 & 1 -->0) ; (1 & 0 --> 0) and (1 & 1 --> 1)</h4>
<h4>For Example:-</h4>
<h4>10 --> 1010</h4>
<h4>20 --> 10100</h4>
<h4>(10 & 20) --> 1010 & 10100 --> 00000 --> 0</h4><br>

<h3><i>2) OR(|) : </i></h3>
<h4>OR(|) operator compares two integer bits as (0 & 0 --> 0) ; (0 & 1 --> 1) ; (1 & 0 --> 1) and (1 & 1 --> 1)</h4>
<h4>For Example:-</h4>
<h4>10 --> 1010</h4>
<h4>20 --> 10100</h4>
<h4>(10 & 20) --> 1010 & 10100 --> 11110 --> 30</h4><br>

<h3><i>3) XOR(^) : </i></h3>
<h4>XOR(^) operator compares two integer bits as (0 & 0 --> 0) ; (0 & 1 --> 1) ; (1 & 0 --> 1) and (1 & 1 --> 0)</h4>
<h4>For Example:-</h4>
<h4>10 --> 01010</h4>
<h4>20 --> 10100</h4>
<h4>(10 & 20) --> 1010 & 10100 --> 11110 --> 30</h4><br>

<h3><i>4) NOT(~) : </i></h3>
<h4>NOT(~) operator compares  one integer bits as (~0 --> 1) ; (~1 --> 0)</h4>
<h4>For Example:-</h4>
<h4>10 --> 1010</h4>
<h4>~10 --> 0101 --> 5</h4><br>

<h3><i>5) Left Shift Operator(<<) : </i></h3>
<h4>Left Shift operator shifts all bits left by n bits where n is "(no.)<<n"</h4>
<h4>For Example:-</h4>
<h4>10 --> 1010</h4>
<h4>10<<2 --> this will shift  left by 2 bits --> 101000 --> 40</h4><br>
  
<h3><i>6) Right Shift Operator (>>) : </i></h3>
<h4>Right Shift operator shifts all bits right by n bits where n is "(no.)>>n"</h4>
<h4>For Example:-</h4>
<h4>20 --> 10100</h4>
<h4>20>>2 --> Shift right by 2 bits --> 101 --> 5</h4>

<h2>Algorithm : </h2>
<h3>1) Basic Operation:</h3>
