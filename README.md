# English difficulty level evaluation
Watching movies in original language is a very popular and effective way to learn foreign language. It's important to choose a proper movie so student could understand 50-70% of dialogues. To fulfill this condition, the teacher must watch the film and decide which level it corresponds to. It requires much time and genre preferences of a student and a teacher may differ. 

The goal of this project is to develop an ML solution for automatically determining the level of complexity of English-language films.

Subtitles stored separately in srt files, labels stored in `labels.csv`

The main problem we have here is:
- too little sample with movies which can cause difficulties in training and testing model;
- different expert opinions led to the appearance of two different categories at once for some films;
- such qualitative features as prononciation quality and speech intelligibility weren't provided. 

## Conclusion
* The most realistic evaluation of model is 0.51 Accuracy.
* Dividing movies into parts helps to upsample. But in this way we receive a data leak. 
* Calculating features such as counting unique words, movie time, the amount of different difficulty levels words and so on can give good results. The main problem we have here is the lack of data and such qualitative features as prononciation quality and speech intelligibility which could have a strong influence on English difficulty level. 
* More data and expert information about prononciation quality and speech intelligibility could improve the results.
