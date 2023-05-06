Download Link: https://assignmentchef.com/product/solved-ece471-assignment-1-linear-regression-of-a-noisy-sinewave-using-a-set-of-gaussian-basis
<br>
Perform linear regression of a noisy sinewave using a set of gaussian basis

<strong>005          </strong>functions with learned location and scale parameters. Model parameters are

<strong><sup>006          </sup></strong>learned with stochastic gradient descent. Use of automatic differentiation is

<strong>007</strong>

<strong>008           </strong>required. Hint: note your limits!

<strong>009</strong>

<strong>010</strong>

<strong>011          </strong><strong>Problem Statement            </strong>Consider a set of scalars {<em>x</em><sub>1</sub><em>,x</em><sub>2</sub><em>,…,x<sub>N</sub></em>} drawn from U(0<em>,</em>1) <strong>012  </strong>and a corresponding set {<em>y</em><sub>1</sub><em>,y</em><sub>2</sub><em>,…,y<sub>N</sub></em>} where:

<strong>013</strong>

<table width="0">

 <tbody>

  <tr>

   <td width="46"><strong>014</strong><strong>015</strong><strong>016</strong><strong>017</strong><strong>018</strong><strong>019</strong><strong>020</strong><strong>021</strong><strong>022</strong></td>

   <td width="496"><em>y<sub>i </sub></em>= sin(2<em>πx<sub>i</sub></em>)+ <em>ϵ<sub>i</sub></em>and <em>ϵ<sub>i </sub></em>is drawn from N(0<em>,σ</em><sub>noise</sub>). Given the following functional form:<em>y</em>ˆ<em><sub>i </sub></em>= ∑<em>w<sub>j</sub>ϕ<sub>j </sub></em>(<em>x<sub>i </sub></em>| <em>µ<sub>j</sub>,σ<sub>j</sub></em>)+ <em>b </em><em>M</em><em>j</em>=1with:</td>

   <td width="32">(1)(2)</td>

  </tr>

 </tbody>

</table>

<strong>023</strong>

<strong>024</strong>(3)

<strong>025</strong>

<table width="0">

 <tbody>

  <tr>

   <td width="46"><strong>026</strong><strong>027</strong></td>

   <td width="454">find estimates <sup>ˆ</sup><em>b</em>, {<em>µ</em>ˆ<em><sub>j</sub></em>}, {<em>σ</em>ˆ<em><sub>j</sub></em>}, and {<em>w</em>ˆ<em><sub>j</sub></em>} that minimize the loss function:</td>

  </tr>

 </tbody>

</table>

<strong>028</strong>

<strong>029</strong>(4)

<strong>030</strong>

<strong><sup>031             </sup></strong>for all (<em>x<sub>i</sub>,y<sub>i</sub></em>) pairs. Estimates for the parameters must be found using stochastic

<strong>032 </strong>gradient descent. A framework that supports automatic differentiation must be

<strong>033</strong>

<strong>034                  </strong>used. Set <em>N </em>= 50<em>,σ</em><sub>noise </sub>= 0<em>.</em>1. Select <em>M </em>as appropriate. Produce two plots. First,

<strong><sup>035          </sup></strong>show the data-points, a noiseless sinewave, and the manifold produced by the

<strong>036</strong>

regression model. Second, show each of the <em>M </em>basis functions. Plots must be of

<strong>037</strong>

<strong>038         </strong>suitable visual quality.