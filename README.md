# Parameter Optimization of SVM
<b>Dataset Used :</b> MAGIC Gamma Telescope Data Set <br>
<b>Number of Instances:</b> 19020 <br>
<b>Number of Attributes:</b> 11 <br>

<b>Dataset Description :</b>
The data are MC generated (see below) to simulate registration of high energy gamma particles in a ground-based atmospheric Cherenkov gamma telescope using the imaging technique. Cherenkov gamma telescope observes high energy gamma rays, taking advantage of the radiation emitted by charged particles produced inside the electromagnetic showers initiated by the gammas, and developing in the atmosphere. This Cherenkov radiation (of visible to UV wavelengths) leaks through the atmosphere and gets recorded in the detector, allowing reconstruction of the shower parameters. The available information consists of pulses left by the incoming Cherenkov photons on the photomultiplier tubes, arranged in a plane, the camera. Depending on the energy of the primary gamma, a total of few hundreds to some 10000 Cherenkov photons get collected, in patterns (called the shower image), allowing to discriminate statistically those caused by primary gammas (signal) from the images of hadronic showers initiated by cosmic rays in the upper atmosphere (background).

Typically, the image of a shower after some pre-processing is an elongated cluster. Its long axis is oriented towards the camera center if the shower axis is parallel to the telescope's optical axis, i.e. if the telescope axis is directed towards a point source. A principal component analysis is performed in the camera plane, which results in a correlation axis and defines an ellipse. If the depositions were distributed as a bivariate Gaussian, this would be an equidensity ellipse. The characteristic parameters of this ellipse (often called Hillas parameters) are among the image parameters that can be used for discrimination. The energy depositions are typically asymmetric along the major axis, and this asymmetry can also be used in discrimination. There are, in addition, further discriminating characteristics, like the extent of the cluster in the image plane, or the total sum of depositions.


<h2> Parameter Optimisation of SVM </h2>
Kernels Used:
<ul>
<li> linear </li>
<li> poly </li>
<li> rbf </li>
<li> sigmoid </li>
</ul>
<h1>Final Result</h1>
<table class="tg">
<thead>
  <tr>
    <th class="tg-jbod">Sample</th>
    <th class="tg-jbod">Best Accuracy</th>
    <th class="tg-jbod">Best Kernel</th>
    <th class="tg-jbod">Best Nu</th>
    <th class="tg-0r4h">Best Epsilon</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">1</td>
    <td class="tg-c3ow">0.64</td>
    <td class="tg-c3ow">rbf</td>
    <td class="tg-c3ow">4.17</td>
    <td class="tg-c3ow">4.60</td>
  </tr>
  <tr>
    <td class="tg-0pky">2</td>
    <td class="tg-c3ow">0.40</td>
    <td class="tg-c3ow">sigmoid</td>
    <td class="tg-c3ow">4.67</td>
    <td class="tg-c3ow">6.55</td>
  </tr>
  <tr>
    <td class="tg-0pky">3</td>
    <td class="tg-c3ow">0.38</td>
    <td class="tg-c3ow">sigmoid</td>
    <td class="tg-c3ow">8.05</td>
    <td class="tg-c3ow">4.33</td>
  </tr>
  <tr>
    <td class="tg-0pky">4</td>
    <td class="tg-c3ow">0.41</td>
    <td class="tg-c3ow">sigmoid</td>
    <td class="tg-c3ow">6.56</td>
    <td class="tg-c3ow">5.27</td>
  </tr>
  <tr>
    <td class="tg-0pky">5</td>
    <td class="tg-c3ow">0.47</td>
    <td class="tg-c3ow">linear</td>
    <td class="tg-c3ow">9.63</td>
    <td class="tg-c3ow">1.50</td>
  </tr>
  <tr>
    <td class="tg-0lax">6</td>
    <td class="tg-0lax">         0.38</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;&nbsp;sigmoid</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;0.65</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;9.79</td>
  </tr>
  <tr>
    <td class="tg-0lax">7</td>
    <td class="tg-0lax">         0.64</td>
    <td class="tg-0lax">      poly</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;6.88</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;8.92</td>
  </tr>
  <tr>
    <td class="tg-0lax">8</td>
    <td class="tg-0lax">         0.39</td>
    <td class="tg-0lax">    sigmoid</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;5.60</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;8.19</td>
  </tr>
  <tr>
    <td class="tg-0lax">9</td>
    <td class="tg-0lax">         0.72</td>
    <td class="tg-0lax">     linear</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;0.37</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;7.36</td>
  </tr>
  <tr>
    <td class="tg-0lax">10</td>
    <td class="tg-0lax">         0.40</td>
    <td class="tg-0lax">    sigmoid</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;3.84</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.23</td>
  </tr>
</tbody>
</table>

<h1> Convergence Graph </h1>
![convgraph](https://user-images.githubusercontent.com/79705963/233173092-94e3faeb-b2a6-404f-a2c0-f1cca726481c.png)

