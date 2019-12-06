# thaipbs-111k
**A dataset for Thai Text Summarisation from https://news.thaipbs.or.th/news.**

The `thaipbs-111k` dataset is crawled from the news site Thai PBS News. This dataset is purposefully scraped for evaluating various Thai NLP tasks especially text summarization and news article text classification. We filtered out those articles which match, at least, one of following conditions:

- Article body contains less than 50 words.
- Summary contains less than 8 words.
- The abstractedness of the summary at 1-grams is *higher* than 65%.

After filtering, it contains 111,614 articles with — tags and — lebels from May 8, 2015 to October 21, 2019. This dataset was crawled and cleaned by [Tanachat Arayachutinan](https://github.com/caramelWaffle) and [Nakhun Chumpolsathien](https://github.com/nakhunchumpolsathien). You can see preliminary exploration in `exploration.ipynb`.
> Code in `exploration.ipynb` is borrowed from the exploratory notebook of [prachathai-67k](https://github.com/PyThaiNLP/prachathai-67k) dataset.

## `thaipbs-111k` Dataset Statistics
| Properties     | Value |
| :--------- | -----:|
| Dataset Size  | 111,614 |
| Average Article Length     |   254.28 |
| Average Summary Length     |    36.52 |
| Average Title Length |      —|
| Unique Tag Size |  — |
| Vocabulary Size | — |
> — To be updated
### Compression Ratio
|    | `thaipbs-111k`|`thairath-228k`|
| :--------- | -----:| -----:|
| Article Sentence Length | 21.02|37.18|
| Summary Sentence Length   |   3.07|3.54|
|**Compression Ratio**|6.84|10.50|

> Compression ratio of `thaipbs-111k` and `thairath-228k` datasets. The represented article and summary lengths are the mean over all sentences

### Level of Abstractedness
Abstractedness of the dataset is measured by calculating the unique n-grams in the reference summary which are not in the article. We compare the abstractedness level of `thaipbs-111k` dataset to `thairath-228k` dataset. The comparison is shown in the below figure.

<img src="data/ab_c.png"
     alt="thaipbs-111k"
     style="width: 200px"
     width="500px"
     />
> Note: According Koupaee and Wang (2018), “The higher level of abstractedness creates new challenges for the summarization systems as they have to be more creative in generating more novel summaries”.

## Experimental Results
#### Classification-benchmarks
 >※ To be updated 
#### Thai Text Summarization
 >※ To be updated 

## License
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/80x15.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">This dataset</span> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/caramelWaffle/thaipbs-111k" rel="dct:source">https://github.com/caramelWaffle/thaipbs-111k</a>.
