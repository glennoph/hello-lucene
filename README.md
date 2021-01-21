hello-lucene
============

Mavenized version of Kelvin Tan's example (http://www.lucenetutorial.com/lucene-in-5-minutes.html)

Use the following command to run the program:
```
$ mvn package -q
```

## Steps/output
```
A. create analyzer=...StandardAnalyzer
B. create index=RAMDirectory...
C. add document doc=Document<stored,indexed,tokenized<title:Lucene in Action> stored,indexed,omitNorms,indexOptions=DOCS
C. add document doc=Document<stored,indexed,tokenized<title:Lucene for Dummies> stored,indexed,omitNorms,indexOptions=DOCS
C. add document doc=Document<stored,indexed,tokenized<title:Managing Gigabytes> stored,indexed,omitNorms,indexOptions=DOCS
C. add document doc=Document<stored,indexed,tokenized<title:The Art of Computer Science> stored,indexed,omitNorms,indexOptions=DOCS
D. create query string: lucene
E. specify fields "title" in query:title:lucene
F. execute search searcher:IndexSearcher...
F. Found 2 hits. (below)

1. 193398817	Lucene in Action
2. 55320055Z	Lucene for Dummies
```