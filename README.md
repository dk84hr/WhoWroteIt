# WhoWroteIt

The notebook entails a ***text classification project*** based on song lyrics.
The user may input an *unlimited* amount of artists (due to the speed of scraping, however, 2-4 are recommended), whose lyrics will be scraped from https://www.metrolyrics.com/. The goal is to ***train a model that predicts an artist based on new input/ piece of text***.

![image](https://user-images.githubusercontent.com/71432794/114549737-ac375400-9c61-11eb-94d6-192a076f330d.png)


After scraping the songs per artist and cleaning the corpus with **RegEx**, words are transformed into a feature matrix (per **TF-IDF Vectorizer**). Data are counter-balanced (*random undersampling*) and fitted on a **Multinomial Naive Bayes** model.

![image](https://user-images.githubusercontent.com/71432794/114549969-f4567680-9c61-11eb-8607-dc4c26276145.png)


Finally the user enters a piece of text/ a verse, and the model returns the alleged artist with a relative probability score.

![image](https://user-images.githubusercontent.com/71432794/114550052-0d5f2780-9c62-11eb-8222-2bc9b211000a.png)

BONUS: for every artist a ***WordCloud*** displaying the frequency of words is drawn; the bigger the word, the more frequent it is in the artist's corpus:

![image](https://user-images.githubusercontent.com/71432794/114712345-48c82780-9d30-11eb-89bb-a8395f08c26b.png)
