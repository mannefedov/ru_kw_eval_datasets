# ru_kw_eval_datasets
Four datasets for evaluation keyword extraction in Russian

You can find all the datasets in /data directory. The datasets are stored in .jsonlines format (every line in a file is a json). The datasets are split into parts due to github file size limitations.

Sources of data: 

https://russian.rt.com/

https://habr.com/

http://www.ng.ru/

https://cyberleninka.ru/

Every line in files represent one document. For the RussiaToday, NG and Habrahabr the json line has following structure:
***{'content': "Text of the document here', 'title': 'Title of the document here', 'summary': 'short summary of the document here', 'keywords': ['key', 'words', 'here']}***


For Cyberleninka files the structure of the json is this:
***{'content': "Text of the document here', 'title': 'Title of the document here', 'abstract': 'abstract of the document here', 'keywords': ['key', 'words', 'here']}***

Cyberleninka documents are pdf converted to text with pdf2text so may be a bunch of mistakes and random linebreaks there.
