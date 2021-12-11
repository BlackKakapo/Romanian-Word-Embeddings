# Romanian Word Embeddings (Coming soon)

###### [CopyLeft Project](https://en.wikipedia.org/wiki/Copyleft)
These vectors was trained with 3 different methods (CBOW, Skip-Gram, FastText). The dataset is a bunch of text that was taken from internet (news, comments, blogs etc.).

#

> Please notice I do not claim that these vectors are the best for romanian language!

#

### About Dataset
The text is pre processed and cleaned.

- 3.136.600.772 -  Sentences (One of purpose is the sentence need to be bigger than 35 characters, including the spaces) 
- 46.514.848.508 -  Words
- 1.311.442 - Unique words
- 14,82 - AVG number of words in sentence

#

| Method | Size | Min_count | Window | SET1 - Precision | SET2 - Precision | Download | Size | 
| ------ |----- | --------- | ------ | ---- | ---- | --------- | ----- |
| CBOW | 300 | 25 | 5 | 13% | 23% | <a href="https://drive.google.com/file/d/1rZw5gVw5iXcs8438QWPKY0aIHGCYO6wk/view?usp=sharing">Download</a> | 4.2 GB |
| CBOW | 300 | 25 | 15 | 63% | 91% | <a href="">Coming soon</a> | 4.2 GB |
| CBOW | 300 | 25 | 20 | 64% | 93% | <a href="">Coming soon</a> | 4.2 GB |
| CBOW | 600 | 25 | 20 | n | n |
| Skip-Gram | 300 | 25 | 5 | n | n |
| Skip-Gram | 300 | 25 | 15 | n | n |
| Skip-Gram | 300 | 25 | 20 | n | n |
| Skip-Gram | 600 | 25 | 20 | n | n |
| FastText | 300 | 25 | 5 | n | n |
| FastText | 300 | 25 | 15 | n | n |
| FastText | 300 | 25 | 20 | n | n |
| FastText | 600 | 25 | 20 | n | n |

#

SET1 and SET2 are sets with questions-answer with country and capitals, that was made by Romanian Academy (They have their own vectors, you can check it right there [CoRoLa](http://89.38.230.23/word_embeddings/)).


##### Example:
- Romania - Bucharest + London = Great Britain (eng).
- România - București + Londra = Marea Britanie (rom).

#

SET1 - 1892 analogies for European countries and their capitals

SET2 - 462 analogies for European countries and their capitals (subset of SET1)