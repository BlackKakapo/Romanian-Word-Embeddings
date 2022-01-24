# Romanian Word Embeddings

These vectors was trained with 3 different methods (CBOW, Skip-Gram, FastText) from Gensim library. The dataset is a bunch of text that was taken from internet (news, comments, blogs etc.).

#

> Please notice I do not claim that these vectors are the best for romanian language!

#

### About Dataset
The text is pre processed and cleaned.

- 784.150.193 -  Sentences (One of purpose is the sentence need to be bigger than 35 characters, including the spaces) 
- 11.628.712.127 -  Words
- 1.311.442 - Unique words
- 14,82 - AVG number of words in sentence

#

| Method | Size | Min_count | Window | SET1 - Precision | SET2 - Precision | Download | Size | 
| ------ |----- | --------- | ------ | ---- | ---- | --------- | ----- |
| CBOW | 300 | 25 | 5 | 14% | 23% | <a href="https://utm-my.sharepoint.com/:u:/g/personal/alexandru_petrachi_iis_utm_md/ERi2j7fQ5bJEgD0-AkLqxacBENnRopTmoyNmF27fmgu9SQ?e=ce9v2C">Download</a> | 4.2 GB |
| CBOW | 300 | 25 | 15 | 66% | 91% | <a href="https://utm-my.sharepoint.com/:u:/g/personal/alexandru_petrachi_iis_utm_md/EUREkeqmIjxMhLaRs5Z_0QUBlYiFNKmMjE5zdfCjeStaxA?e=tdsfrf">Download</a> | 4.2 GB |
| CBOW | 300 | 25 | 20 | 67% | 93% | <a href="https://utm-my.sharepoint.com/:u:/g/personal/alexandru_petrachi_iis_utm_md/Eb33ZorHlgNCibiE9HQdq9oBW6szxsfGN-kvscq5MQH5Fw?e=H4TsLC">Download</a> | 4.2 GB |
| Skip-Gram | 300 | 25 | 5 | 71% | 92% | <a href="https://utm-my.sharepoint.com/:u:/g/personal/alexandru_petrachi_iis_utm_md/EZ5nl68KBxJDm4VoLcAzV9wBrNW9eglb2Pse0hg3U1kQAg?e=B9Ok5n">Download</a> | 4.2 GB |
| Skip-Gram | 300 | 25 | 15 | 79% | 98% | <a href="https://utm-my.sharepoint.com/:u:/g/personal/alexandru_petrachi_iis_utm_md/EfQge6CHUVtLsnL0uKVIbvgBLeLZi44cA9LX23HF439nSg?e=5lxBZ2">Download</a> | 4.2 GB |
| Skip-Gram | 300 | 25 | 20 | 79% | 98% | <a href="https://utm-my.sharepoint.com/:u:/g/personal/alexandru_petrachi_iis_utm_md/EXT1iP0bYn9GmFgLM18cCeEBixKcuOjjekNOf5FqgDEZJw?e=Ned0KZ">Download</a> | 4.2 GB |
| FastText | 300 | 25 | 5 | 66% | 95% | <a href="https://utm-my.sharepoint.com/:u:/g/personal/alexandru_petrachi_iis_utm_md/ERpnT8Uxk4JIhcIq3uk3xSoBih9-nWGGFoIPnYkLOPJ8kQ?e=ZRlGQv">Download</a> | 6.29 GB |
| FastText | 300 | 25 | 15 | 72% | 97% | <a href="https://utm-my.sharepoint.com/:u:/g/personal/alexandru_petrachi_iis_utm_md/Ec4aEOxyeylCocxOeEe7BjgBiXTRsRmM4jl7OfQ6ZjIS_w?e=6qfqcA">Download</a> | 6.29 GB |
| FastText | 300 | 25 | 20 | n | n |

#

SET1 and SET2 are sets with questions-answer with country and capitals, that was made by Romanian Academy (They have their own vectors, you can check it right there [CoRoLa](http://89.38.230.23/word_embeddings/)).


##### Example:
- Romania - Bucharest + London = Great Britain (eng).
- România - București + Londra = Marea Britanie (rom).

#

[SET1](https://github.com/BlackKakapo/Romanian-Word-Embeddings/tree/main/SET/SET1) - 1892 analogies for European countries and their capitals

[SET2](https://github.com/BlackKakapo/Romanian-Word-Embeddings/tree/main/SET/SET2) - 462 analogies for European countries and their capitals (subset of SET1)
