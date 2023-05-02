Download Link: https://assignmentchef.com/product/solved-comp350-numerical-computing-assignment-3-solving-linear-systems
<br>
<ol>

 <li>(a) (3 points) Solve the following system using GEPP (Gaussian elimination with partial pivoting):</li>

</ol>

<table width="228">

 <tbody>

  <tr>

   <td width="77">−31<em>A </em>=  4<sub>2</sub></td>

   <td width="34">1−34−2</td>

   <td width="33">−3−4 −4−4</td>

   <td width="84">15<sub>4 </sub> 17<sub>16</sub>8<sub>8 </sub> <sup>= </sup><sub>16</sub><sup>8 </sup></td>

  </tr>

 </tbody>

</table>

Show intermediate matrices, vectors and multipliers at each step.

(b) (2 points) Compute the LU factorization of the matrix in the previous question with partial pivoting: <em>PA </em>= <em>LU</em>. You have to show intermediate results at each step. This question and the previous one can be answered together.

Note: Do the computations by your hands and don’t consider any rounding errors.

<ol start="2">

 <li>(3 points) Suppose we have a complex linear system <em>Ax </em>= <em>b</em>, where <em>A </em>∈C<em><sup>n</sup></em><sup>×<em>n </em></sup>is nonsingular and <em>b </em>∈C<em><sup>n</sup></em>. Can you solve it in real arithmetic operations? What is the cost?</li>

</ol>

Hint: Rewrite <em>Ax </em>= <em>b </em>as an equivalent 2<em>n </em>× 2<em>n </em>real linear system.

<ol start="3">

 <li>Suppose <em>A </em>∈R<em><sup>n</sup></em><sup>×<em>n </em></sup>is nonsingular.

  <ul>

   <li>(4 points) Given <em>B </em>∈R<em><sup>n</sup></em><sup>×<em>p</em></sup>, show how to use the LU factorization with partial pivoting to solve <em>AX </em>= <em>B</em>. What is the cost of your method?</li>

  </ul></li>

</ol>

Hint: <em>AX </em>= <em>B </em>is equivalent to <em>AX</em>(:<em>,j</em>) = <em>B</em>(:<em>,j</em>) for <em>j </em>= 1 : <em>p</em>.

<ul>

 <li>(5 points) Use m given in the lecture notes to solve <em>AX </em>= <em>B</em>, where 10 × 10 Hilbert matrix <em>A </em>= (<em>a<sub>ij</sub></em>)<em>, a<sub>ij </sub></em>= 1<em>/</em>(<em>i </em>+ <em>j </em>− 1);</li>

</ul>

10 × 5 <em>B </em>= <em>A </em>∗randn(10<em>,</em>5)<em>.</em>

Here randn is a MATLAB built-in function to generate a random matrix. Denote this randn(10<em>,</em>5) by <em>X<sub>t </sub></em>and your computed solution by <em>X<sub>c</sub></em>.

<ul>

 <li>Compute k<em>X<sub>c </sub></em>− <em>X<sub>t</sub></em>k<em><sub>F</sub>/</em>k<em>X<sub>t</sub></em>k<em><sub>F </sub></em>and <em>ǫ</em>k<em>A</em>k<em><sub>F</sub></em>k<em>A</em><sup>−1</sup>k<em><sub>F</sub></em>, where <em>ǫ </em>is the machine epsilon. Check MTALAB built-in functions or constants norm, cond and eps, to see how to compute or get related quantities.</li>

 <li>Compute the relative residual k<em>B </em>− <em>AX<sub>comp</sub></em>k<em><sub>F</sub>/</em>(k<em>A</em>k<em><sub>F</sub></em>k<em>X<sub>comp</sub></em>k<em><sub>F</sub></em>).</li>

</ul>

<ol>

 <li>Run your code 10 times (you may use a loop). Notice each time you have different<em>B</em>, since <em>X<sub>true </sub></em>is random. Answer the following questions:</li>

 <li>Do you see any rough relation between k<em>X<sub>c </sub></em>− <em>X<sub>t</sub></em>k<em><sub>F</sub>/</em>k<em>X<sub>t</sub></em>k<em><sub>F </sub></em>and <em>ǫ</em>k<em>A</em>k<em><sub>F</sub></em>k<em>A</em><sup>−1</sup>k<em><sub>F</sub></em>? iii. Do you see any rough relation between k<em>B </em>− <em>AX<sub>c</sub></em>k<em><sub>F</sub>/</em>(k<em>A</em>k<em><sub>F</sub></em>k<em>X<sub>c</sub></em>k<em><sub>F</sub></em>) and <em>ǫ </em>?</li>

</ol>

Print out your MATLAB code and the results.

1

(c) Computing <em>A</em><sup>−1</sup>

<ol>

 <li>(3 points) Show how to use the LU factorization with partial pivoting to computethe inverse of a general <em>n </em>× <em>n </em>nonsingular matrix <em>A</em>. What is the cost of your method? (Hint: Think about what matrix equation <em>AX </em>= <em>B </em>you should solve to get <em>A</em><sup>−1</sup>).</li>

</ol>

Compute the inverse of a 5 × 5 Hilbert matrix defined in 3(b). Print out your MATLAB code and the result.

<ol>

 <li>(3 bonus points) For the sake of simplicity, suppose we use the LU factorizationwith no pivoting to compute <em>A</em><sup>−1</sup>. Briefly state an algorithm which costs 2<em>n</em><sup>3 </sup> You need to explain why its cost is 2<em>n</em><sup>3 </sup>flops.</li>

</ol>

2