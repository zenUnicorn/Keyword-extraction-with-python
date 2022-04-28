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



### Happy Coding🥳
