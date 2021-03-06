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
<img src="null_hypo.png" align="center" border="0" alt="Ho:  \mu\_congruent =  \mu\_incongruent" width="299" height="19" /> <br>

<img src="alternative_hypo.png" align="center" border="0" alt="Ha:  \mu\_congruent  \neq   \mu\_incongruent" width="299" height="19" /> <br>
where <img src="mu.png" /> is the population mean.

<p>

<b>I will use a Dependent T-Test (Paired T-Test) because:  </b> <br>

 &nbsp; &nbsp; &nbsp; - Dependent variable is on a continuous scale <br>
 &nbsp; &nbsp; &nbsp; - Independent variable consists of two categorical, "related groups" or "matched pairs" <br>
 &nbsp; &nbsp; &nbsp; - There are no significant outliers in the differences between the two related groups (Random sampling from a defined population) <br>
 &nbsp; &nbsp; &nbsp; - The distribution of the differences in the dependent variable between the two related groups is approximately normally distributed <br>
 
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
 
1 - Define Null and Alternative Hypotheses <br>

<img src="null_hypo.png" align="center" border="0" alt="Ho:  \mu\_congruent =  \mu\_incongruent" width="299" height="19" /> <br>
<br>

<img src="alternative_hypo.png" align="center" border="0" alt="Ha:  \mu\_congruent  \neq   \mu\_incongruent" width="299" height="19" /> <br>
<br>

2 - State Alpha <br>

<img src="alpha.png" align="center" border="0" alt=" \alpha = 0.05" width="75" height="15" />
<br>

3 - Calculate Degrees of Freedom <br>

Degrees of freedom(df): N - 1 = 24 -1 = 23

4 - State Decision Rule <br>

I found a critical value of 2.0687 using the t-table for a two-tailed test with 23 degrees of freedom and an alpha of 0.05. <br>

t-critical: 2.0687 <br>

Then,  decision rule is rejecting the null hypothesis if t-statistic value is less than -2.0687 or greater than 2.0687.



5 - Calculate Test Statistic <br>

M_d = -7.96 <br>

S_d = 4.86 <br>

t_statistic = -8.02 <br>


6 - State Results <br>

t_statistic = -8.02 <br>

less than t_critical(-2.0687), so i reject the null hypothesis.

7 - State Conclusion <br>

There is a significant difference in the mean task completion times between the two conditions, at 0.05. The result matches up with my expectations and with my own test result. 

<p>

<h3>
6. Optional: What do you think is responsible for the effects observed? Can you think of an alternative or similar task that would result in a similar effect? Some research about the problem will be helpful for thinking about these two questions!
</h3>

I think, for the brain, reading a word is faster than determining the color. So there is an interference in the Stroop test. 

As an alternative task, i can give the confuse your legs example (http://www.sciencemadesimple.co.uk/activity-blogs/confuse_your_legs)

Lift your right foot a few inches from the floor and then begin to move it in a clockwise direction. While you’re doing this, use a finger your right index finger to draw a number 6 in the air. Your foot will turn in an anticlockwise direction and there’s nothing you can do about it!

The left side of your brain, which controls the right side of your body, is responsible for rhythm and timing. The left side of your brain cannot deal with operating two opposite movements at the same time and so it combines them into a single motion.

Try this with your right foot and left hand and you should have no problem!


<p><p>
Sources: 
<br>
<a href="https://classroom.udacity.com/nanodegrees/nd002">Udacity Data Analyst Nanodegree Program Statistics Lessons</a> 
<br>
http://www.statisticslectures.com/topics/dependentsamplest/
<br>
https://www.amazon.com/Essentials-Business-Statistics-Bruce-Bowerman/dp/0078020530
<br>
http://www.sciencemadesimple.co.uk/activity-blogs/confuse_your_legs
<br>
https://statistics.laerd.com/spss-tutorials/dependent-t-test-using-spss-statistics.php
<br>
http://www.psychology.emory.edu/clinical/bliwise/Tutorials/TOM/meanstests/assump.htm



 
