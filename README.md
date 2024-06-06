# Data-Extraction-and-NLP
To extract textual data articles from the given URL and perform text analysis to compute variables.
Using Python, extract article text from Input.xlsx, saving each in a text file named by URL_ID, excluding website headers and footers.

Perform text analysis on extracted texts, computing variables outlined in BELOW, saving output in the format of "Output Data Structure.xlsx"

1.Sentimental Analysis
1.1 Cleaning using Stop Words Lists
- Remove stop words to enable sentiment analysis, excluding words in the stop words list.
1.2 Creating dictionary of Positive and Negative words
- Use a master dictionary to form positive and negative word dictionaries, excluding stop words.
1.3 Extracting Derived variables
- Calculate:
- Positive Score: Σ(+1 if word in Positive Dictionary)
- Negative Score: -Σ(+1 if word in Negative Dictionary)
- Polarity Score: (Positive Score - Negative Score) / ((Positive Score + Negative Score) + 0.000001)
- Subjectivity Score: (Positive Score + Negative Score) / ((Total Words after cleaning) + 0.000001)

2.Analysis of Readability

Calculate using Gunning Fox index formula:
Average Sentence Length: Total words / Total sentences
Percentage of Complex words: (Complex Words / Total Words)
Fog Index: 0.4 * (Average Sentence Length + Percentage of Complex words)

3.Average Number of Words Per Sentence
Formula: Total number of words / Total number of sentences

4.Complex Word Count
Count words with more than two syllables.

5.Word Count
Count total cleaned words, excluding stop words and punctuation.

6.Syllable Count Per Word
Count syllables in each word, handling exceptions like "es" and "ed" endings.

7.Personal Pronouns
Calculate occurrences of personal pronouns using regex, excluding "US" as a country name.

8.Average Word Length
Formula: Sum of characters in each word / Total number of words.
