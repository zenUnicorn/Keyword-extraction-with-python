# Keyword-extraction-with-python
## Keyword Extraction using Python (RAKE, YAKE, PKE, KeyBERT, MultiRake, and TextRank)

1. Using RAKE (Rapid Automatic Keyword Extraction)
```
from rake_nltk import Rake
rake_class = Rake()
```

```
text = """ Programming is writing computer code to create a program, to solve a problem. 
Programs are created to implement algorithms. Algorithms can be represented as pseudocode or a flowchart , 
and programming is the translation of these into a computer program."""
```

```
rake_class.extract_keywords_from_text(text)
extracted_keyword = rake_class.get_ranked_phrases()
print(extracted_keyword)
```

2. Using YAKE (Yet Another Keyword Extractor)

```
import yake
```

```
text = """ Programming is writing computer code to create a program, to solve a problem. 
Programs are created to implement algorithms. Algorithms can be represented as pseudocode or a flowchart , 
and programming is the translation of these into a computer program."""
```

```
extractor = yake.KeywordExtractor(top=10, stopwords=None)
keywords = extractor.extract_keywords(text)
for kw, u in keywords:
  print("Keyphrase: ",kw, ": score", u)
```


### Happy Coding🥳
