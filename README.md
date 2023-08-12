# R Analysis of Little Women

# Text Analysis of *Little Women*
This repository includes code to perform a text analysis and sentiment analysis on Lousia May Alcott's novel, *Little Women* (1868). The purpose of this repository is to explore the words associated with the text through visualizing their frequencies and their sentiments and provide a deeper understanding of the narrative and Alcott's style. 

# Data Description
To analyze *Little Women*, I downloaded its text from the gutenbergr package, which provides access to the public domain works from the Project Gutenberg collection. The textual data in "Little Women" consists of the complete text of the novel written by Louisa May Alcott, including the dialogues, descriptions, and narrative passages that comprise the story.

# Result Replication
This code imports, processes, and analyzes the text and sentiments of *Little Women*, creating different visualizations of the word frequency and sentiments of the novel (in `little_women_analysis_files` folder). The code outputs include descriptive tables of word counts, plots of word frequency, sentiment analysis of common sentiments, trust word analysis, sentiments throughout the narrative, common positive and negative words, and word clouds. Please note that you need to have R and the required libraries installed to run the code successfully.

To replicate the analyses, you will need the following libraries:
- `library(dplyr)`
- `library(gutenbergr)`
- `library(tidytext)`
- `library(ggplot2)`
- `library(textdata)`
- `library(knitr)`
- `library(tidyverse)`
- `library(stringr)`
- `library(wordcloud)`
- `library(reshape2)`
- `library(RColorBrewer)`

You can install them by running the below code: 
```{r}
# Install required libraries
install.packages(c("dplyr", "gutenbergr", "tidytext", "ggplot2", "textdata", "knitr", "tidyverse", "stringr", "wordcloud", "reshape2" "RColorBrewer"))
```
The code can be found in the `little_women_analysis.Rmd`. The file is divided into different chunks labeled for their outputs. You will need to run the `import` and `process` chunks in order to run the later code and create the visualizations. Each chunk is prefaced by a title and description and followed by a brief interpretation for clarity. 

# Resources
- Julia Silge and David Robinson, [Text Mining with R] (https://www.tidytextmining.com/index.html), 2022
- David Robinson, [gutenbergr: Download and Process Public Domain Works from Project Gutenberg] (https://cran.rstudio.com/package=gutenbergr), 2016
- StackOverflow, [How to create a custom RColorBrewer palette] (https://stackoverflow.com/questions/66684545/how-to-create-custom-rcolorbrewer-palette)

# Reflection
This assignment provided an opportunity for me to apply the textual analysis skills we studied as well as explore one of my favorite classical novels, *Little Women*. I faced challenges handling the textual data, cleaning and preprocessing it, and creating my desired visualizations. The [Text Mining with R] (https://www.tidytextmining.com/index.html) book and online resources such as StackOverflow provided great models for my analysis, and I was able to even format my visualizations, for example,  incorporating colors into my wordclouds. Taking a suggestion from an office hours, I reordered my code to show the barcharts and word clouds consecutively to consider how to best order my visualizations to maximize audience understanding. 

I found my resultsfascinating, as the textual and sentiment analysis shed light into Alcott's style and the emotional arc of the novel. It was enjoyable to explore the data and aesthetically represent my findings-I was surprised about how easy libraries like `wordcloud` make generating seemingly complex graphics. Especially given my interests in the political role of media, I see myself applying these textual analysis skills to future projects, perhaps examining the sentiments of media posts during the Arab Spring. This was a great opportunity to practice and apply these skills! Thank you for reading! 