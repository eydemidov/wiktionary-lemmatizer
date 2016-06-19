# Wiktionary Lemmatizer

A script to extract list of lemmas for a given new-line separated list of words. Keeps order of the words and outputs which words were replaced by lemmas for manual checking. Requires Nokogiri gem. Uses SAX and wiktionary files are gygabytes in size, so might take a while to process.

## Example usage:

```
./lemmatizer.rb enwiktionary-20160501-pages-articles.xml fr.txt french
```

Outputs `fr/lemmas.csv` with the words replaced by lemmas with their indexes in the original lists, and `fr/replaced_words.csv` with the words replaced by lemmas and their original indexes.
