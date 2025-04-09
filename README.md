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
| CBOW | 300 | 25 | 5 | 14% | 23% | Lost in Void | 4.2 GB |
| CBOW | 300 | 25 | 15 | 66% | 91% | Lost in Void | 4.2 GB |
| CBOW | 300 | 25 | 20 | 67% | 93% | Lost in Void | 4.2 GB |
| Skip-Gram | 300 | 25 | 5 | 71% | 92% | <a href="https://drive.google.com/file/d/1BenQcAFpo-K4FSL0DcdxMa0uLLT-uZvu/view?usp=sharing">Download</a> | 4.2 GB |
| Skip-Gram | 300 | 25 | 15 | 79% | 98% | <a href="https://drive.google.com/file/d/1getGtHreDWL0TAZdXaovPewKx0OGgPQS/view?usp=sharing">Download</a> | 4.2 GB |
| Skip-Gram | 300 | 25 | 20 | 79% | 98% | <a href="https://drive.google.com/file/d/17AzcDiM9FVwE9TUZToZiEqUP9OGrXqIM/view?usp=sharing">Download</a> | 4.2 GB |
| FastText | 300 | 25 | 5 | 66% | 95% | <a href="https://drive.google.com/file/d/1zgm8v_scFWhbECOp9T0ZnLQtJ89T6h5r/view?usp=sharing">Download</a> | 6.29 GB |
| FastText | 300 | 25 | 15 | 72% | 97% | <a href="https://drive.google.com/file/d/1XOcijO_gAP3PZJCf8-PO3Tii4ThNxX6p/view?usp=sharing">Download</a> | 6.29 GB |
| FastText | 300 | 25 | 20 | 74% | 98% | <a href="https://drive.google.com/file/d/1YRMq7Gt_Eq-IJm1-2RLPCQxyOsfQgc_k/view?usp=sharing">Download</a> | 6.29 GB |
|-------------------------------------------------------------------|

#

SET1 and SET2 are sets with questions-answer with country and capitals, that was made by Romanian Academy (They have their own vectors, you can check it right there [CoRoLa](http://89.38.230.23/word_embeddings/)).


##### Example:
- austria - vienna + amsterdam = netherlands  (eng).
- austria - viena + amsterdam = olanda (rom).

#

[SET1](https://github.com/BlackKakapo/Romanian-Word-Embeddings/tree/main/SET/SET1) - 1892 analogies for European countries and their capitals

[SET2](https://github.com/BlackKakapo/Romanian-Word-Embeddings/tree/main/SET/SET2) - 462 analogies for European countries and their capitals (subset of SET1)

#

```python
from gensim.models import Word2Vec

model = Word2Vec.load('SG_300_20_15.model')

resultQuery = model.wv.most_similar('**WORD**')

for result in resultQuery:
    print(result)
    
In: spania
Out:
('italia', 0.8326004147529602)
('portugalia', 0.8248708248138428)
('castilla-leon', 0.7556794285774231)
('belgia', 0.7364105582237244)
('argentina', 0.7281147241592407)
('spania-', 0.727818489074707)
('brazilia', 0.7213218212127686)
('olanda', 0.6885160207748413)
('germania', 0.6858677864074707)
('anglia', 0.6833646297454834)

In: ilie
Out:
('adrian', 0.7264171242713928)
('andrei', 0.7138616442680359)
('valentin', 0.6969763040542603)
('dumitru', 0.673446536064148)
('llie', 0.6705739498138428)
('nicolae', 0.6643682718276978)
('vasile', 0.6577962636947632)
('marian', 0.6359540224075317)
('constantin', 0.6084895133972168)
('nicu', 0.6063842177391052)

In: ruble
Out: 
('grivne', 0.795340359210968)
('hrivne', 0.7273794412612915)
('copeici', 0.7101361155509949)
('dolari', 0.6791703104972839)
('yuani', 0.6516059041023254)
('rublă', 0.6284367442131042)
('kopeici', 0.6272767186164856)
('zloţi', 0.6005615592002869)
('usd', 0.5963905453681946)
('piaştri', 0.5942535996437073)

In: fizician
Out:
('matematician', 0.6948787569999695)
('savant', 0.6890636086463928)
('fizicianul', 0.6560385823249817)
('inventator', 0.653334379196167)
('astrofizician', 0.644870936870575)
('chimist', 0.6142269372940063)
('astronom', 0.6096892356872559)
('filozof', 0.604558527469635)
('teoretician', 0.6006152629852295)
('cercetător', 0.5948916673660278)
```
