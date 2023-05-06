Download Link: https://assignmentchef.com/product/solved-ee559-homework-10
<br>
<strong>Note:</strong>  The problems in this assignment are to solved by hand.  If you want to use a computer to help with the plots, you may; but you will probably find that unnecessary.

<ol>

 <li>In a 2-class problem with 1 feature, you are given the following data points:</li>

</ol>

<em>S</em><sub>1 </sub>: −3, − 2, 0 <sub>  </sub><em>S</em><sub>2 </sub>: −1, 2

<ul>

 <li>Give the <em>k</em>-nearest neighbor estimate of <em>p</em>(<em>xS</em><sub>1</sub>) with <em>k</em>=3, for all <em>x</em>. Give both algebraic (simplest) form, and a plot.  On the plot, show the location (<em>x</em> value) and height of (each) peak.</li>

 <li>Give the Parzen Windows estimate of <em>p</em>(<em>xS</em><sub>2</sub>) with window function:</li>

</ul>

( ) ⎧ ⎪ 0.25, −2 ≤<em>u</em>&lt; 2

Δ <em><sub>u </sub></em>=⎨

⎪⎩ 0,      otherwise

Give both algebraic (simplest) form, and a plot.  On the plot, show the <em>x</em> value of all significant points, and label the values of <em>p</em>(<em>xS</em><sub>2</sub>) clearly.

<ul>

 <li>Estimate prior probabilities <em>P</em>(<em>S</em><sub>1</sub>) and <em>P</em>(<em>S</em><sub>2</sub>) from frequency of occurrence of the data points.</li>

 <li>Give an expression for the decision rule for a Bayes minimum error classifier using the density and probability estimates from (a)-(c). You may leave your answer in terms of  <em>p</em>ˆ(<em>xS</em><sub>1</sub>), <em>p</em>ˆ(<em>xS</em><sub>2</sub>), <em>P</em>ˆ(<em>S</em><sub>1</sub>), <em>P</em>ˆ(<em>S</em><sub>2</sub>) , without plugging in for these quantities.</li>

 <li>Using the estimates you have made above, solve for the decision boundaries and regions of a Bayes minimum error classifier using the density and probability estimates from (a)-(c). Give your answer in 2 forms:

  <ul>

   <li>Algebraic expressions of the decision rule, in simplest form (using numbers and variable <em>x</em>);</li>

   <li>A plot showing the decision boundaries and regions.</li>

  </ul></li>

</ul>

<strong>Tip:</strong> you may find it easiest to develop the algebraic solution and plot and the same time.

<ul>

 <li>Classify the points: <em>x</em>=−5, 0.1, 0.5 using the classifier you developed in (e).</li>

 <li>Separately, use a discriminative 3-NN classifier to classify the points <em>x</em>=−5, 0.1, 0.5. (<strong>Hint:</strong>  if this takes you more than a few steps for each data point,</li>

</ul>

you are doing more work than necessary.)

<em>Assignment continues on next page… </em>

<ol start="2">

 <li>[Comment: this problem is on parameter estimation, which is covered in Lecture 26 on Monday, 4/27.]</li>

</ol>

In a 1D problem (1 feature), we will estimate parameters for one class.  We model the density <em>p</em>(<em>x</em>θ) as:

⎧

<em>px</em>θ)=⎪⎨ θ<em>e</em>−θ<em>x</em>,            <em>x</em>≥ 0

⎪⎩ 0,      otherwise

in which θ≥0 .

You are given a dataset <em>Z : x</em><sub>1</sub>,<em>x</em><sub>2</sub>,!,<em>x<sub>N </sub></em>, which are drawn i.i.d. from <em>p</em>(<em>x</em>θ).

In this problem, you may use for convenience the notation:

1 <em>N</em>

<em>m</em>!<sup>∑</sup><em>x<sub>i</sub></em> .

<em><sub>N </sub></em><em>i</em><sub>=</sub>1

<ul>

 <li>Solve for the maximum likelihood (ML) estimate θ<sup>ˆ</sup><em><sub>ML </sub></em>, of θ, in terms of the given data points. Express your result in simplest form.</li>

</ul>




For parts (b) and (c) below, assume there is a prior for θ, as follows:

<em>p</em>(θ)=⎧⎪⎨   <em>ae</em>−<em>a</em>θ, θ≥ 0

⎪⎩ 0,      otherwise

in which <em>a</em>≥0 .




<ul>

 <li>Solve for the maximum a posteriori (MAP) estimate θ<sup>ˆ</sup><em><sub>MAP </sub></em>, of θ, in terms of the given data points. Express your result in simplest form.</li>

 <li>Write θ<sup>ˆ</sup><em><sub>MAP</sub></em> as a function of θ<sup>ˆ</sup><em><sub>ML</sub></em> and given parameters. Find <sub>σ</sub><sup>l</sup>θ<sup>i</sup><sub>→</sub><sup>m</sup><sub>∞</sub>θ<sup>ˆ</sup><em><sub>MAP</sub></em> , in which σ<sub>θ</sub> is the standard deviation of the prior on θ.  What does this limit correspond to in terms of our prior knowledge of θ?</li>

</ul>

<table width="632">

 <tbody>

  <tr>

   <td width="31"> </td>

   <td width="601">θ <em>a</em></td>

  </tr>

  <tr>

   <td width="31">3.</td>

   <td width="601"><strong>[Extra credit]</strong> Comment: this problem is not more difficult than the regular-credit problems above; it is extra credit because the total length Problems 1 and 2 above is already sufficient and reasonable for one homework assignment.</td>

  </tr>

  <tr>

   <td width="31"> </td>

   <td width="601">In a 2-class problem with <em>D</em> features, you are to use Fisher’s Linear Discriminant to find an</td>

  </tr>

 </tbody>

</table>

<strong>Hint:</strong>  the standard deviation of θ for the given <em>p</em>(θ) is:  σ =<sup>1</sup> .

optimal 1D feature space.  You are given that the scatter matrices for each class (calculated from the data for each class) are diagonal:

=⎡⎢⎢ ⎢⎢   σ12 σ2  0 ⎤⎥⎥⎥<sub>, <em><u>S</u></em></sub>2 =⎢⎢⎡⎢ ρ<sub>1</sub>2        0 <sub>⎥</sub>⎥ ⎤ ⎥

<em><u><sub>S</sub></u></em>1           2               ⎥          <sub>⎢           ρ</sub>22         <sub>⎥</sub>

⎢⎢ ⎢⎣                               0    ! 2          ⎥⎥          ⎢⎢ 0   ! ρ<em>D</em>2    ⎥ ⎥⎥⎦ σ<em>D                  </em>⎥⎦         ⎢⎣

and you are given the sample means for each class:

⎛⎜   <em>m</em>1(1) ⎞⎟ ⎛⎜ <em>m</em>1(2) ⎞⎟ <em><u>m</u></em><sub>1 </sub>=⎜⎜   <em>m</em>2(1) ⎟⎟ , <em><u>m</u></em>2 =⎜⎜ <em>m</em>2(2) ⎟⎟ .

⎜           !        ⎟           ⎜           !        ⎟

⎜⎜⎝ <em>m</em>(<em><sub>D </sub></em>1) ⎟⎟⎠     ⎜⎝⎜ <em>m</em>(<em>D</em>2) ⎟⎟ ⎠

<ul>

 <li>Find the Fisher’s Linear Discriminant <em><u>w</u></em> . Express in simplest form.</li>

 <li>Let <em>D</em>= Suppose σ<sub>1</sub><sup>2 </sup>=4σ<sub>2</sub><sup>2 </sup>, and ρ<sub>1</sub><sup>2 </sup>=4ρ<sub>2</sub><sup>2</sup> , and:</li>

</ul>

⎛

<em><u>m</u></em>1 =⎜⎝ 2<sub>2   </sub>⎞⎟⎠ , <em><u>m</u></em>2 =⎛⎜⎝ −<sub>1</sub>2 ⎞⎟⎠

Plot vectors <em><u>m</u></em><sub>1</sub>, <em><u>m</u></em><sub>2</sub>, (<em><u>m</u></em><sub>1</sub>−<em><u>m</u></em><sub>2</sub>),  and <em><u>w</u></em>.

<ul>

 <li>Interpreting your answer of part (b), which makes more sense for a 1D feature space direction: (<em><u>m</u></em><sub>1</sub>−<em><u>m</u></em><sub>2</sub>) or <em><u>w</u></em>?  Justify your answer.</li>

</ul>


