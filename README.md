# GRS
GRS Data Mining

Original data has more female samples than male ones, in most analysis, 207 male and 207 random selected female samples are used as in GenderEven207.csv. Preprocessed (removing -c) data with all samples saved in data-c_removed.csv

#### [x] Do certain keywords in the written content appear, which correlate to specific Wellgorithms and / or categories? E.g. “When people do the Close Confessor Wellgorithm, they use these words and phrases more / less frequently:”

See files in Raw/ . Files in this directory contain frequently used words sorted according to wellgorithms, categories and gender.

Note that High frequent functional words are not indicative, thus in .*_filted.csv file those are removed based on POS tags: n_tags=['PRP','PRP$','VBD','RB','VBZ','VBP','VB','MD',’VB']. POS tag reference in bottom of RAW.ipynb

#### [x] Can we determine from the written content how much of the problems explored are related to self? Other people? Circumstance?
POS doesn't differ myself, herself... only present tense third person. However, Raw/W-fdist_Top30-gender.csv answers the question to some extent.

#### [ ] Especially interested to know if there are any Big Insights to discover when comparing Food addictions to Drug/Alcohol addictions.


#### [ ] Also especially interested in clusters that are not obvious to the human eye. What combinations of words, categories, patterns are you finding? Things a human might never have thought to ask?

See Cluster.ipynb file, comments are made below each plot.

#### [x] From the NLP insights, what sorts of gender differences are you finding?
     
Male total/average words: 20,703 / 114.51

Female total/avg words:  17,679 / 85.41

See result in file in Raw/W-fdist_Top30-gender.csv. Non-indicative words with negative_tags=['$',"''",'(',')','--','.',',',':','DT','CC','IN','TO'] are removed.

In gender-even distribution:

Male: Focus more on past, and self ==> Suffer, past

Female: Focus more on present and others ==> Hope, future
    
#### [ ] We humans discovered 209 categories. What additional categories can we discover from the written answers using NLP?  
Categories are sometime abstract, topic modelling algorithms can’t generate something that’s not inside the expression.

#### [x] Any insights about past, present or future focus on their language?

Male: Focus more on past, and self ==> Suffer, past

Female: Focus more on present and others ==> Hope, future


#### [ ] Any insights about willpower and motivation in their language?

### Basic statistical analysis of categories & Wellgorithms:

#### [x] Do men / women gravitate toward different Wellgorithms?
  
See below files in Gender/

WELGOS_vs_GENDER_total.csv - total 'female': 578, 'male': 207

Gender_vs_Welgos-EvenDist.csv - Randomly selected 207 female samples from original dataset

GenderPolar-Welgos.csv - File contain gender polarity with respect to wellgorithms with a threshold (dif > 6 | dif < -4).

#### [x] What are the commonly overlapping Wellgorithms? (Which Wellgorithms occur together as pairs with other Wellgorithms)
See files in Overlap/

G-even = gender even

Total = original data set with -c removed

Matrix = all overlaps

Top10 = top10 most overlapped 

#### [x] What are the commonly overlapping categories? (Which categories occur together more often than others)

See files in Overlap/

#### [x] What are the relationships between Wellgorithms and categories? Which Wellgorithms match to which categories most often?

See files in Overlap/

