# Ru_kw_eval_datasets
### Datasets for evaluation of keyword extraction in Russian

You can find all the datasets in /data directory. The datasets are stored in .jsonlines format (every line in a file is a json). The datasets are split into parts due to github file size limitations.

Sources of data: 

* https://russian.rt.com/

* https://habr.com/

* http://www.ng.ru/

* https://cyberleninka.ru/

Every line in files represents one document. For the **RussiaToday, NG** and **Habrahabr** the json line has the following structure:
```python
{'url':'https://url.here', content': 'Text of the document here', 'title': 'Title of the document here', 
 
'summary': 'short summary of the document here', 'keywords': ['key', 'words', 'here']}
```

For **Cyberleninka** files the structure of the json is:
```python
{'url':'https://url.here', 'content': 'Text of the document here', 'title': 'Title of the document here',

'abstract': 'abstract of the document here', 'keywords': ['key', 'words', 'here']}
```

Cyberleninka documents are pdfs converted to raw texts with pdf2text so there may be a bunch of mistakes and random linebreaks. Also note that the keywords were extracted from the documents **manually** (hell, that was boring!) after conversion and I could easily skipped something. Please inform me if you find undeleted keywords inside the content field.

My e-mail: manefedov26@gmail.com


## Dataset Metadata
The following table is necessary for this dataset to be indexed by search
engines such as <a href="https://g.co/datasetsearch">Google Dataset Search</a>.
<div itemscope itemtype="http://schema.org/Dataset">
<table>
  <tr>
    <th>property</th>
    <th>value</th>
  </tr>
  <tr>
    <td>name</td>
    <td><code itemprop="name">RuKWEval Dataset</code></td>
  </tr>
  <tr>
    <td>url</td>
    <td><code itemprop="url">https://github.com/mannefedov/ru_kw_eval_datasets</code></td>
  </tr>
  <tr>
    <td>sameAs</td>
    <td><code itemprop="sameAs">https://github.com/mannefedov/ru_kw_eval_datasets</code></td>
  </tr>
  <tr>
    <td>description</td>
    <td><code itemprop="description">Datasets for evaluation of keyword extraction in Russian</code></td>
  </tr>
</table>
</div>
