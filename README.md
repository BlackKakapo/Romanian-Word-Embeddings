# Romanian Word Embeddings

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
| CBOW | 300 | 25 | 5 | 13% | 23% | <a href="https://utm-my.sharepoint.com/:u:/g/personal/alexandru_petrachi_iis_utm_md/ERi2j7fQ5bJEgD0-AkLqxacBENnRopTmoyNmF27fmgu9SQ?e=ce9v2C">Download</a> | 4.2 GB |
| CBOW | 300 | 25 | 15 | 63% | 91% | <a href="https://utm-my.sharepoint.com/:u:/g/personal/alexandru_petrachi_iis_utm_md/EUREkeqmIjxMhLaRs5Z_0QUBlYiFNKmMjE5zdfCjeStaxA?e=tdsfrf">Download</a> | 4.2 GB |
| CBOW | 300 | 25 | 20 | 64% | 93% | <a href="https://utm-my.sharepoint.com/:u:/g/personal/alexandru_petrachi_iis_utm_md/Eb33ZorHlgNCibiE9HQdq9oBW6szxsfGN-kvscq5MQH5Fw?e=H4TsLC">Download</a> | 4.2 GB |
| CBOW | 600 | 25 | 20 | 68% | 96% | <a href="">Coming soon</a> |  GB |
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
