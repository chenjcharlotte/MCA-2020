# Music Curation and Analytics 20-21

| [Back to Homepage](https://github.com/chenjcharlotte/MCA-2020/blob/master/README.md) | [Musical Data](https://github.com/chenjcharlotte/MCA-2020/blob/master/weeklyTasks/week1.md) | [Notated Data](https://github.com/chenjcharlotte/MCA-2020/blob/master/weeklyTasks/week2.md) | [Encoded Notation](https://github.com/chenjcharlotte/MCA-2020/blob/master/weeklyTasks/week3.md) | [Computational Analytics](https://github.com/chenjcharlotte/MCA-2020/blob/master/weeklyTasks/week4.md) | [Standards in Curation](https://github.com/chenjcharlotte/MCA-2020/blob/master/weeklyTasks/week5.md) |
|---|---|---|---|---|---|


## Week 4: Computational Analytics

### Task 1: jSymbolic 

First, I exported *You'll Be Back* as a MIDI file. Then, I followed instructions and generated a jSymbolic of the piece.
I have selected a range of features and here is the [CSV file](https://github.com/chenjcharlotte/MCA-2020/blob/master/weeklyTasks/week4_jSymbolic1.csv). 

The table includes the basic fatures of the analysis, such as number of pitches, number of pitch classes, range, mean pitch, and mean pitch class. There are some interesting results from these basic features. For example, while the number of pitch classes is 11, there is only one common pitch class of this music piece. Further, I also selected some other features that I think are interesting and relevant to my piece. For instance, the pitch skewness of my piece is -0.9701, indicating that an asymmetrical pitch distribution to the left of the mean pitch. Also, the data shows that the middle register appears to be more significant than bass or high registers in this music piece. 

| Features | Data | Features | Data |
|---|---|---|---|
|Number of Pitches|34|Number of Pitch Classes|11|
|Number of Common Pitches|4|Number of Common Pitch Classes|1|
|Range|48|Importance of Bass Register|0.1628|
|Importance of Middle Register|0.7487|Importance of High Register|0.0885|
|Dominant Spread|3|Strong Tonal Centres|2|
|Mean Pitch|63.72|Mean Pitch Class|5.276|
|Most Common Pitch|71|Most Common Pitch Class|2|
|Prevalence of Most Common Pitch|0.1628|Prevalence of Most Common Pitch Class|0.2389|
|Relative Prevalence of Top Pitches|0.8913|Relative Prevalence of Top Pitch Classes|0.7481|
|Interval Between Most Prevalent Pitches|4|Interval Between Most Prevalent Pitch Classes|9|
|Pitch Variability|9.338|Pitch Class Variability|3.723|
|Pitch Class Variability After Folding|2.287|Pitch Skewness|-0.9701|
|Pitch Class Skewness|1.028|Pitch Class Skewness After Folding|1.163|
|Pitch Kurtosis|7.123|Pitch Class Kurtosis|4.778|
|Pitch Class Kurtosis After Folding|8.532|First Pitch|55|


### Task 2: music21 

I used the Python notebook and generated a piano roll and pitch histogram of *You'll Be Back* by using music21. 

|interpretations|Graphs|
|---|---|
|This is the histogram of the pitch, which demonstrates that the most common pitch is B4, a result that matches the jSymbolic results above (Most Common Pitch: 71). The graph shows the importance of the middle register, which is a fraction of notes between MIDI pitches 55 and 72.|![](https://github.com/chenjcharlotte/MCA-2020/blob/master/images/week4music21Graph.png)|
|The scatter plot is plotted quarter length against the pitch. According to the graph, the data regarding pitch is consistent with the last graph and the analysis from jSymbolic, with B5 appearing to be the most common pitch throughout the song. |![](https://github.com/chenjcharlotte/MCA-2020/blob/master/images/week4myScatterPlot.png)|
|There are 37 measures in total, and I decided to analyse the entire piece I transcribed. The graph here is a virtual representation of piano roll. The number of measures is represented on the horizontal axis against the pitch on the vertical axis. When the x-axis of the graph shows more information regarding the time, the pitch matches the previous analysis, with the middle register seeming more significant than bass and high voice. |![](https://github.com/chenjcharlotte/MCA-2020/blob/master/images/week4noteQuarterLengthByPitch.png)|
