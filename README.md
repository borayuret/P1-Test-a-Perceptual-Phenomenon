# P1: Test a Perceptual Phenomenon

<h2>Background Information</h2>

In a Stroop task, participants are presented with a list of words, with each word displayed in a color of ink. The participant’s task is to say out loud the color of the ink in which the word is printed. The task has two conditions: a congruent words condition, and an incongruent words condition. In the congruent words condition, the words being displayed are color words whose names match the colors in which they are printed: for example RED, BLUE. In the incongruent words condition, the words displayed are color words whose names do not match the colors in which they are printed: for example PURPLE, ORANGE. In each case, we measure the time it takes to name the ink colors in equally-sized lists. Each participant will go through and record a time from each condition.

<h2>Questions For Investigation</h2>

[Dataset: stroopdata.csv](stroopdata.csv)
<p>

<h3> 1. What is our independent variable? What is our dependent variable? </h3>

<b>Independent Variable:</b> Congruent and incongruent words
<br>
<b>Dependent Variable:</b> Time to name the color

<p>

<h3> 2. What is an appropriate set of hypotheses for this task? What kind of statistical test do you expect to perform? Justify your choices.</h3>

<b>Ho (Null Hypothesis):</b> The time required to name the color for congruent word is equal to the time required to name the color of incongruent word. 

<b>Ha (Alternative Hypothesis):</b> The time required to name the color for congruent word is not equal to the time required to name the color of incongruent word. 

<p>

<b>I will use a Dependent T-Test (Paired T-Test) because:  </b> <br>
 &nbsp; &nbsp; &nbsp; - i want to compare the means of two related groups to determine whether there is a statistically significant difference between these means <br>
 &nbsp; &nbsp; &nbsp; - i don't know the populations standard deviation <br>
 &nbsp; &nbsp; &nbsp; - i have a limited sample (n < 30) <br>
 &nbsp; &nbsp; &nbsp; - data is derived from subjects who have been measured at two time points (each individual has two measurements) <br>
 
<p>

<h3>3. Report some descriptive statistics regarding this dataset. Include at least one measure of central tendency and at least one measure of variability.</h3>

<center>
<table>
<tr>
<th></th>
<th>Congruent</th>
<th>Incongruent</th>
</tr>
<tr>
<td>Mean</td>
<td>14.05</td>
<td>22.02</td>
</tr>

<tr>
<td>Median</td>
<td>14.36</td>
<td>21.02</td>
</tr>

<tr>
<td>Variance</td>
<td>12.67</td>
<td>23.01</td>
</tr>

<tr>
<td>St. Dev.</td>
<td>3.56</td>
<td>4.80</td>
</tr>

<tr>
<td>St. Err.</td>
<td>0.73</td>
<td>0.98</td>
</tr>


</table>
</center>

<p>


<h3>
4. Provide one or two visualizations that show the distribution of the sample data. Write one or two sentences noting what you observe about the plot or plots.
</h3>

<center>
<table>

<tr>
<td>
   <img src="graph1.JPG" alt="graph1">
</td>
<td>
   <img src="graph2.JPG" alt="graph1">
</td>
</tr>



</table>
</center>
<br>
It is obvious on the graphs that reading incongruent words takes more time than reading congruent words, at every point (for every person in the sample). 

<p>


<h3>
5. Now, perform the statistical test and report your results. What is your confidence level and your critical statistic value? Do you reject the null hypothesis or fail to reject it? Come to a conclusion in terms of the experiment task. Did the results match up with your expectations?
</h3>

I will perform a dependent sample t-test.<br>

Steps: <br>
 
1. Define Null and Alternative Hypotheses <br>

<img src="http://www.sciweavers.org/tex2img.php?eq=Ho%3A%20%20%5Cmu%5C_congruent%20%3D%20%20%5Cmu%5C_incongruent&bc=White&fc=Black&im=png&fs=12&ff=arev&edit=0" align="center" border="0" alt="Ho:  \mu\_congruent =  \mu\_incongruent" width="299" height="19" /> <br>
<br>

<img src="http://www.sciweavers.org/tex2img.php?eq=Ha%3A%20%20%5Cmu%5C_congruent%20%20%5Cneq%20%20%20%5Cmu%5C_incongruent&bc=White&fc=Black&im=png&fs=12&ff=arev&edit=0" align="center" border="0" alt="Ha:  \mu\_congruent  \neq   \mu\_incongruent" width="299" height="19" /> <br>
<br>

2. State Alpha <br>

<img src="http://www.sciweavers.org/tex2img.php?eq=%20%5Calpha%20%20%3D%200.05&bc=White&fc=Black&im=jpg&fs=12&ff=arev&edit=0" align="center" border="0" alt=" \alpha  = 0.05" width="75" height="15" />
<br>

3. Calculate Degrees of Freedom <br>

4. State Decision Rule <br>

5. Calculate Test Statistic <br>

6. State Results <br>

7. State Conclusion <br>




<p><p>
Sources: 
<br>
<a href="https://classroom.udacity.com/nanodegrees/nd002">Udacity Data Analyst Nanodegree Program Statistics Lessons</a> 
<br>
http://www.statisticslectures.com/topics/dependentsamplest/
<br>
https://www.amazon.com/Essentials-Business-Statistics-Bruce-Bowerman/dp/0078020530




