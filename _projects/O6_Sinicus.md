---
layout: project
title: MAE 2250 - Exhibit Client Report
description: Class Assignment
image: /assets/images/spotted_lanternfly4.jpg
fontsize: 11pt 
geometry: margin=1in 
papersize: letter 
pagestyle: empty
group: group1
--- 
**Team:** _Sinicus_
<br>
Karen Chen, Elias Herrera Hernandez, Mallory Moore, Tien Phan, Rachel Williams

## Context and Problem Statement
During grape harvest season, spotted lanternflies (SLFs) are more attracted to grapevines than their typically preferred trees of heaven. SLFs feed on the phloem of gravepines, which reduces nitrogen and carbon in the soil, resulting in less healthy grapes. In addition, grape harvest batches containing too many SLFs are immediately discarded. Because grapes are essential to wine and juice industries, plentiful grape harvests are essential for the success of these industries. Our solution involves attracting SLFs to something other than the grapevines and trapping them before they access grapevines at all. We decided to take this approach in order to stem grapevine damage from the start, preventing harvest complexity and preserving harvest profits.

## Final Prototype and Application
We built a hand crank mechanism that attracts SLFs and sweeps them into a collection bin with a funnel. The main focus of our final prototype is a disk that we can cover in honey to model tree of heaven sap that SLFs are attracted to over grapevines. The SLFs will stick to the honey, and the rake will sweep stuck SLFs off the disk into the funnel, which causes the SLFs to slide into a collection bin. To operate our mechanism, a user periodically rotates the hand crank, which in turn rotates the rake.

<div style="text-align: center;">
  <img src="{{ '/assets/images/final_presentation_assembly.png' | relative_url }}" alt="Centered Image" style="max-width:100%; height:auto;">
</div>
<center> Fig 1. Rough sketch of final prototype </center>
<br>

<div style="text-align: center;">
  <img src="{{ '/assets/images/overall_assembly_diagram.png' | relative_url }}" alt="Centered Image" style="max-width:100%; height:auto;">
</div>
<center> Fig 2a. Overall Assembly Diagram </center>
<br>

<div style="text-align: center;">
  <img src="{{ '/assets/images/shaft_stand_detail.png' | relative_url }}" alt="Centered Image" style="max-width:100%; height:auto;">
</div>
<center> Fig 2b. Detail of Shaft and Stand Assembly</center>
<br>


## Conclusion and Recommendations
<p>Our final prototype successfully passed our tests; it could sweep SLF models from the disk into the funnel, which diverted the SLFs into our collection bin. In addition, our prototype was free-standing. However, during exhibition day, our acrylic rake noticeably deformed when sweeping through a thick layer of honey, and it ended up fracturing. In a redesign, we should reconsider what material our rake is made out of, as well as how it interacts with honey. In addition, during the exhibition, our setup was extremely sticky (because of the honey) and unpleasant to clean up. However, because the sap on the disk is intended to be continuously reapplied, we believe cleaning up is not a significant issue when this design is put into practice.</p>
<p>To improve the manufacturing process, we recommend more meticulous machining practices be observed. The current prototype was manufactured using loose tolerances, leading to non-negligible misalignment between components that were likely the cause of the rake failure described above. More careful quality control in the manufacturing process would eliminate the factors that led to this failure and in turn extend the service life of the prototype.</p>
<p>During onfield testing, we recommend placing our design in multiple places (including next to trees of heaven, next to grapevines, and far away from grapevines) to test which location will steer the most SLFs away from grapevines and towards our trap. In addition to this, in practical use, we recommend automating the spinning rake by replacing the hand crank with a solar-powered motor. This way, people do not have to be physically present to operate the device. Finally, the ground in a vineyard is not as flat as the tables we have placed our prototype on. We recommend attaching our hand-crank-disk component to three small stakes that can be stuck in the ground, which will prevent our design from wobbling on or sinking into uneven ground.</p>

## Testing and Results
The two most important things we tested were the style of the rake and the funnel of the collection bin. This is because the rake and the collection bin are the most essential to our prototype’s functionality: we need the rake to sweep away the SLFs, and we need the bin to trap them.
We first tested the functionality of two different rake styles at sweeping off SLFs.

<div style="text-align: center;">
  <img src="{{ '/assets/images/rake_1.jpg' | relative_url }}" alt="Centered Image" style="max-width:100%; height:auto;">
</div>
<center>Fig 2. Prototype rake style 1</center>
<br>

<div style="text-align: center;">
  <img src="{{ '/assets/images/rake_2.jpg' | relative_url }}" alt="Centered Image" style="max-width:100%; height:auto;">
</div>
<center>Fig 3. Prototype rake style 2</center>
<br>

<p>We found that prototype rake style 1 was much more effective than prototype rake style 2, because our SLF models would get stuck in between the metal tines in style 2.</p>
<p>In our funnel test, we tested different funnel diameters. We found that for smaller funnel diameters, some SLF models would fall off the left and right sides of the disk and not land in the funnel. In the end, we found that the funnel diameter should be at least the disk diameter.</p> 
<p>We also tested two stand designs, one with a separate stand for the hand crank and one with the crank directly fixed to a panel behind the funnel. This testing revealed that the crank should be simply-supported, rather than cantilevered, to maximize the stability of the prototype as a whole.</p>

## Prototype and Testing Details
Testing parameters on our wood prototype helped inform us of what to keep and what to change in our final prototype. In the absence of actual SLFs, we crumpled up sticky notes to mimic their size (approximately 1 inch in length) and weight.

### _Rake test_
<p><u>Success criterion:</u> The rake implemented in our design must be capable of scraping all eight SLF models placed on the lure disc across six successive trials of two rake revolutions each.</p>
<p><u>Design parameters:</u> Two rake designs were tested. One design consisted of a flat rake with wide, flat teeth with their face normal to the plane of the disc. The other design consisted of metal tines, normal to the plane of the disc, attached to a flat board installed parallel to the face of the disc.</p>
<p><u>Testing results:</u> Eight SLF models were placed on the lure disc at the start of each trial.</p>

<b>Flat Rake</b>
<table>
    <tr>
        <th>Trial #</th>
        <th>SLFs removed from disk</th>
    </tr>
    <tr>
        <td>1</td>
        <td>8</td>
    </tr>
     <tr>
        <td>2</td>
        <td>8</td>
    </tr>
     <tr>
        <td>3</td>
        <td>8</td>
    </tr>
     <tr>
        <td>4</td>
        <td>8</td>
    </tr>
     <tr>
        <td>5</td>
        <td>8</td>
    </tr>
     <tr>
        <td>6</td>
        <td>8</td>
    </tr>
</table>
<br>

<b>Tine Rake</b>
<table>
    <tr>
        <th>Trial #</th>
        <th>SLFs removed from disk</th>
    </tr>
     <tr>
        <td>1</td>
        <td>6</td>
    </tr>
     <tr>
        <td>2</td>
        <td>6</td>
    </tr>
     <tr>
        <td>3</td>
        <td>6</td>
    </tr>
     <tr>
        <td>4</td>
        <td>5</td>
    </tr>
     <tr>
        <td>5</td>
        <td>6</td>
    </tr>
     <tr>
        <td>6</td>
        <td>6</td>
    </tr>
</table>
<br>

<p><u>Conclusion:</u> While the flat rake consistently removed all SLF models from the lure disc, the tine rake consistently failed to do so. This shortcoming of the tine rake mostly arose from the fact that some SLF models became stuck between the metal tines and subsequently could not be scraped off the lure plate.</p> 

### _Collection bin test_
<p><u>Success criterion:</u> The collection bin should collect at least 85% of the SLFs that are scraped off the disk. </p>
<p><u>Design parameters:</u> 5 different widths of collection bin funnels were tested with both rake designs, and the number of SLFs captured was recorded. 8 SLFs were initially placed on the disk.</p>
<p><u>Testing results:</u></p>

<b>Flat tine rake:</b>
<table>
    <tr>
        <th>Trial #</th>
        <th>OD of funnel (in)</th>
        <th>Funnel OD / Wheel Diameter</th>
        <th>SLFs captured</th>
    </tr>
    <tr>
        <td>1</td>
        <td>7.75</td>
        <td>0.65</td>
        <td>4</td>
    </tr>
    <tr>
        <td>2</td>
        <td>8.50</td>
        <td>0.71</td>
        <td>5</td>
    </tr>
    <tr>
        <td>3</td>
        <td>10.00</td>
        <td>0.83</td>
        <td>7</td>
    </tr>
    <tr>
        <td>4</td>
        <td>11.00</td>
        <td>0.92</td>
        <td>6</td>
    </tr>
    <tr>
        <td>5</td>
        <td>11.00</td>
        <td>0.92</td>
        <td>7</td>
    </tr>
    <tr>
        <td>6</td>
        <td>12.00</td>
        <td>1.00</td>
        <td>7</td>
    </tr>
</table>
<br>

<b>Metal tine rake:</b>
<table>
    <tr>
        <th>Trial #</th>
        <th>OD of funnel (in)</th>
        <th>Funnel OD / Wheel Diameter</th>
        <th>SLFs captured</th>
        <th>SLFs stuck in rake</th>
    </tr>
    <tr>
        <td>1</td>
        <td>7.75</td>
        <td>0.65</td>
        <td>2</td>
        <td>2</td>
    </tr>
    <tr>
        <td>2</td>
        <td>8.50</td>
        <td>0.71</td>
        <td>5</td>
        <td>2</td>
    </tr>
    <tr>
        <td>3</td>
        <td>10.00</td>
        <td>0.83</td>
        <td>5</td>
        <td>2</td>
    </tr>
    <tr>
        <td>4</td>
        <td>11.00</td>
        <td>0.92</td>
        <td>4</td>
        <td>3</td>
    </tr>
    <tr>
        <td>5</td>
        <td>11.00</td>
        <td>0.92</td>
        <td>5</td>
        <td>2</td>
    </tr>
    <tr>
        <td>6</td>
        <td>12.00</td>
        <td>1.00</td>
        <td>5</td>
        <td>2</td>
    </tr>
</table>
<br>

<p><u>Conclusion:</u> The funnel diameter of 10 inches was the smallest diameter to consistently meet the success criteria of collecting 85% of the bugs. Up to 75% of the bugs that escaped the collection bin escaped on the “upswing” of the rake. A further 25% of the escapee bugs landed directly outward from the bin, where the funnel was not extended.</p>
<br>

## Appendix A: Component List

<table>
    <tr>
        <th>Component</th>
        <th>Material/Part</th>
        <th>Purpose</th>
        <th>Fabrication Details</th>
    </tr>
    <tr>
        <td>Disk</td>
        <td>Laser cut acrylic</td>
        <td>Area for SLFs to stick to</td>
        <td>Lasercut in RPL</td>
    </tr>
    <tr>
        <td>Rake</td>
        <td>Laser cut acrylic</td>
        <td>Tool to scrape SLFs off disk</td>
        <td>Lasercut in RPL</td>
    </tr>
    <tr>
        <td>Crank handle</td>
        <td>McMaster product</td>
        <td>Hand mechanism to rotate rake</td>
        <td>COTS, no modifications</td>
    </tr>
    <tr>
        <td>Axle</td>
        <td>McMaster stock</td>
        <td>Attaches to handle and rake such that rotating the handle rotates the rake</td>
        <td>Turned to ensure slip-fit with bearings. ¼-20 threads die-cut to retain disk and rake.</td>
    </tr>
    <tr>
        <td>Collection bin</td>
        <td>McMaster product</td>
        <td>Collects and captures SLFs</td>
        <td>Drilled hole for funnel to direct SLFs into as well as mounting holes for the funnel.</td>
    </tr>
    <tr>
        <td>Funnel</td>
        <td>McMaster stock sheet metal</td>
        <td>Guides SLFs to drop into the collection bin</td>
        <td>Bent and bolted sheet metal to give it funnel shape and attach it to collection bin.</td>
    </tr>
    <tr>
        <td>Disk stand</td>
        <td>McMaster stock wood and metal</td>
        <td>Supports the disk, axle, and handle, and orients the disk above the collection bin</td>
        <td>Aluminum bar stock milled, drilled, tapped, and bored</td>
    </tr>
</table>
<br>


## Appendix B: Final Prototype Bill of Materials

<table>
    <tr>
        <th>Description</th>
        <th>Qty.</th>
        <th>Unit Price</th>
        <th>Total Cost</th>
    </tr>
    <tr>
        <td>Multipurpose 6061 Aluminum Rod, 1 ft</td>
        <td>1</td>
        <td>$5.12 / 2ft</td>
        <td>$2.56</td>
    </tr>
    <tr>
        <td>Adjustable-Position Threaded-Hole-Mount Crank Handle with Revolving Grip, 5/16-18 Thread</td>
        <td>1</td>
        <td>$19.66</td>
        <td>$19.66</td>
    </tr>
    <tr>
        <td>Multipurpose 6061 Aluminum Sheet</td>
        <td>1</td>
        <td>$19.80</td>
        <td>$19.80</td>
    </tr>
    <tr>
        <td>Steel Ball Bearing, Sealed, Trade No. 3003-2RS, for 5/16" Shaft Diameter</td>
        <td>2</td>
        <td>$15.14</td>
        <td>$30.28</td>
    </tr>
    <tr>
        <td>Multipurpose 6061 Aluminum Bar, 1" x 1.5" x 9"</td>
        <td>1</td>
        <td>$41.29 for 12" bar</td>
        <td>$30.97</td>
    </tr>
    <tr>
        <td>Jar</td>
        <td>1</td>
        <td>$17.83</td>
        <td>$17.83</td>
    </tr>
    <tr>
        <td>Corrosion-Resistant 18-8 Stainless Steel Standoff</td>
        <td>4</td>
        <td>$9.73</td>
        <td>$38.92</td>
    </tr>
    <tr>
        <td>Premium Softwood Board, 1.5" x 3.5" x 12"</td>
        <td>1</td>
        <td>$1.37</td>
        <td>$1.37</td>
    </tr>
    <tr>
        <td>Zinc Yellow-Chromate Plated Hex Head Screw, Grade 8 Steel, 1/4"-20 Thread Size, 1-1/2" Long, Fully Threaded</td>
        <td>6</td>
        <td>$11.82 / pack of 25</td>
        <td>$2.84</td>
    </tr>
    <tr>
        <td>Zinc-Plated Medium-Strength Steel Hex Nut, SAE Grade 5, 1/4"-20 Thread Size</td>
        <td>2</td>
        <td>$3.54 / pack of 100</td>
        <td>$0.07</td>
    </tr>
    <tr>
        <td colspan="3" style="text-align:right;"><strong>Total:</strong></td>
        <td>$164.30</td>
    </tr>
</table>
<br>

## Appendix C: Total R&D Bill of Materials

<table>
  <tr>
    <th>Description</th>
    <th>Qty.</th>
    <th>Unit Price</th>
    <th>Total Cost</th>
  </tr>
  <tr>
    <td>Multipurpose 6061 Aluminum Rod, 2ft</td>
    <td>1</td>
    <td>$5.12</td>
    <td>$5.12</td>
  </tr>
  <tr>
    <td>Adjustable-Position Threaded-Hole-Mount Crank Handle with Revolving Grip, 5/16-18 Thread</td>
    <td>1</td>
    <td>$19.66</td>
    <td>$19.66</td>
  </tr>
  <tr>
    <td>Multipurpose 6061 Aluminum Sheet</td>
    <td>3</td>
    <td>$19.80</td>
    <td>$59.40</td>
  </tr>
  <tr>
    <td>Steel Ball Bearing, Sealed, Trade No. 3003-2RS, for 5/16" Shaft Diameter</td>
    <td>3</td>
    <td>$15.14</td>
    <td>$45.42</td>
  </tr>
  <tr>
    <td>Multipurpose 6061 Aluminum Bar, 1" x 1.5" x 2"</td>
    <td>1</td>
    <td>$41.29</td>
    <td>$41.29</td>
  </tr>
  <tr>
    <td>Jar</td>
    <td>1</td>
    <td>$17.83</td>
    <td>$17.83</td>
  </tr>
  <tr>
    <td>Corrosion-Resistant 18-8 Stainless Steel Standoff</td>
    <td>4</td>
    <td>$9.73</td>
    <td>$38.92</td>
  </tr>
  <tr>
    <td>Premium Softwood Board, 1.5" x 3.5" x 12"</td>
    <td>1</td>
    <td>$1.37</td>
    <td>$1.37</td>
  </tr>
  <tr>
    <td>Zinc Yellow-Chromate Plated Hex Head Screw, Grade 8 Steel, 1/4"-20 Thread Size, 1-1/2" Long, Fully Threaded, 25ct.</td>
    <td>1</td>
    <td>$11.82</td>
    <td>$11.82</td>
  </tr>
  <tr>
    <td>Zinc-Plated Medium-Strength Steel Hex Nut, SAE Grade 5, 1/4"-20 Thread Size, 100ct.</td>
    <td>1</td>
    <td>$3.54</td>
    <td>$3.54</td>
  </tr>
  <tr>
    <td colspan="3" style="text-align:right;"><strong>Total:</strong></td>
    <td>$244.37</td>
  </tr>
</table>
<br>

_**Note:** all materials used for prototypes prior to the final prototype, as well as any materials used in the final prototype not included in the Bill of Materials above, were obtained from leftover stock found in the TDS and as such placed no burden on our budget._

## References
Harner, Andrew D., Heather L. Leach, Lauren Briggs, and Michela Centinari. 2022. “Prolonged Phloem Feeding by the Spotted Lanternfly, an Invasive Planthopper, Alters Resource Allocation and Inhibits Gas Exchange in Grapevines.” Plant Direct 6 (10). <a href="https://doi.org/10.1002/pld3.452">https://doi.org/10.1002/pld3.452.</a>

Petit, Elsa, Zoe Robinson, Jessica Ellis, Max Resnick, Amber Ali, and Sonia Schloemann. n.d. “2021 New England and New York Grape Production Survey.” Fruit Notes 88: 2023. Accessed February 12, 2026. <a href="http://umassfruitnotes.com/v88n1/FN6.pdf">http://umassfruitnotes.com/v88n1/FN6.pdf</a>.

Rohde, Barukh, Miriam F Cooperband, Isaiah Canlas, and Richard W Mankin. 2022. “Evidence of Receptivity to Vibroacoustic Stimuli in the Spotted Lanternfly Lycorma Delicatula (Hemiptera: Fulgoridae).” Journal of Economic Entomology 115 (6): 2116–20. <a href= "https://doi.org/10.1093/jee/toac167">https://doi.org/10.1093/jee/toac167.</a>