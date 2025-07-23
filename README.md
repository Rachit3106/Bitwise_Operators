<h1>Experiment 4: Bitwise Operators in C++</h1>
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
<ol>
  <li><strong>Start</strong> the program.</li>
  
  <li><strong>Declare and initialize</strong> two integer variables:
    <ul>
      <li><code>a = 10</code></li>
      <li><code>b = 20</code></li>
    </ul>
  </li>
  
  <li><strong>Perform Bitwise Operations</strong>:
    <ul>
      <li><strong>Bitwise AND (&amp;):</strong> <code>bit_add = a &amp; b</code> – Performs AND operation on each bit.</li>
      <li><strong>Bitwise OR (|):</strong> <code>bit_sub = a | b</code> – Performs OR operation on each bit.</li>
      <li><strong>Bitwise Complement (~):</strong> 
        <ul>
          <li><code>bit_com_a = ~a</code> – Inverts all bits of <code>a</code>.</li>
          <li><code>bit_com_b = ~b</code> – Inverts all bits of <code>b</code>.</li>
        </ul>
      </li>
      <li><strong>Bitwise XOR (^):</strong> <code>bit_xor = a ^ b</code> – Performs XOR operation on each bit.</li>
      <li><strong>Left Shift (&lt;&lt;):</strong> <code>left_shift_a = a &lt;&lt; 2</code> – Shifts bits of <code>a</code> two positions to the left.</li>
      <li><strong>Right Shift (&gt;&gt;):</strong> <code>right_shift_a = a &gt;&gt; 2</code> – Shifts bits of <code>a</code> two positions to the right.</li>
    </ul>
  </li>
  
  <li><strong>Display</strong> all results using <code>cout</code>.</li>
  
  <li><strong>Stop</strong> the program.</li>
</ol><br>
<h3>2) Resetting a Bit using Bitwise XOR in C++</h3>

<h3>Steps</h3>
<ol>
  <li><strong>Start</strong> the program.</li>
  
  <li><strong>Declare and initialize</strong> the required variables:
    <ul>
      <li><code>a = 22</code> – The initial number whose bit will be changed.</li>
      <li><code>reset = 1</code> – A helper value used for bit manipulation.</li>
      <li><code>pos_for_reset</code> – To store the bit position entered by the user.</li>
    </ul>
  </li>
  
  <li><strong>Display message</strong> to the user: <em>"Type pos for reset:"</em></li>
  
  <li><strong>Take input</strong> from the user and store it in <code>pos_for_reset</code>.</li>
  
  <li><strong>Perform the Bitwise Operation</strong>:
    <ul>
      <li>Use <code>a = a ^ (reset &lt;&lt; pos_for_reset)</code></li>
      <li>This shifts the <code>reset</code> (1) to the given bit position and then toggles (changes) that bit in <code>a</code> using XOR.</li>
      <li>If the bit was 1, it becomes 0 (reset); if it was 0, it becomes 1.</li>
    </ul>
  </li>
  
  <li><strong>Display the result</strong>:
    <ul>
      <li>Print: <em>"Value of a after changing position: "</em> followed by the updated value of <code>a</code>.</li>
    </ul>
  </li>
  
  <li><strong>Stop</strong> the program.</li>
</ol><br>
<h3>3) Setting a Bit using Bitwise OR in C++</h3>

<h3>Steps</h3>
<ol>
  <li><strong>Start</strong> the program.</li>
  
  <li><strong>Declare and initialize</strong> the required variables:
    <ul>
      <li><code>i = 22</code> – The initial number whose bit will be changed.</li>
      <li><code>a = 1</code> – A helper value used for bit manipulation.</li>
      <li><code>pos_to_reset</code> – To store the bit position entered by the user.</li>
      <li><code>set</code> – To store the updated value after changing the bit.</li>
    </ul>
  </li>
  
  <li><strong>Display message</strong> to the user: <em>"Type Position to reset:"</em></li>
  
  <li><strong>Take input</strong> from the user and store it in <code>pos_to_reset</code>.</li>
  
  <li><strong>Perform the Bitwise Operation</strong>:
    <ul>
      <li>Shift the helper bit to the desired position: <code>a = a &lt;&lt; pos_to_reset</code></li>
      <li>Set (turn ON) that bit in <code>i</code> using Bitwise OR: <code>set = i | a</code></li>
      <li>This operation ensures the specific bit at the given position is changed to 1, 
          while other bits remain unchanged.</li>
    </ul>
  </li>
  
  <li><strong>Display the result</strong>:
    <ul>
      <li>Print: <em>"Value of a after changing position: "</em> followed by the updated value stored in <code>set</code>.</li>
    </ul>
  </li>
  
  <li><strong>Stop</strong> the program.</li>
</ol>
<h2>Conclusion</h2>
<p>
This experiment successfully demonstrates how to <strong>set (turn ON) a specific bit</strong> in an integer using 
<strong>Bitwise OR ( | )</strong> and <strong>Left Shift ( &lt;&lt; )</strong> operators in C++.  
The left shift moves the bit (1) to the desired position, and the bitwise OR ensures that the corresponding bit in 
the original number is changed to 1, while all other bits remain unchanged.  
This technique is widely used in low-level programming, hardware control, and memory manipulation.
</p>
