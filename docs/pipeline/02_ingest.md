# Ingestion

Once we have our data that has been cleaned and formatted, we need to ingest it into our knowledge base. Ingestion is the process of taking data and converting it into a format that can be used by our knowledge base.

This means creating vector embeddings for each chunk, (which is termed a document and many documents make a paper/pdf) and then indexing them into a vector database.

- https://www.youtube.com/watch?v=ymON0qXbbdw
- scispacy 
- medcat

## Prepocessing 

We can use ML NLP to create additional metadata for each document.

This will enable Hybrid Search where we use both semantic and traditional lexical searches.

## Tokenization

We can convert the document to tokens that form a set of tags to help with filtering queries.

### Named Entity Recognition

We can use MedNER to extract named entities from each document. This can help with traditional searches/filtering as well as enable GraphDB creation.

### Summarization

For documents with a certain amount of content, we can do NLP Summarization, vecorizing the summary and indexing it into the vector database.

This will also enable article summarization for users and we can sue the LLM to combine summarising the document as a whole with the summary of all the section summaries.

### Create questions

Given a document (chunk), we can use the LLM to create questions that can be used to improve retrieval. "What questions does this document answer?"

This is a technique of RAG but rather than do this with each search, we can as a background task do this with each document.

We then have the options to add this strategy if needed.

### Postgresql FTS

We can use Postgresql FTS to create a full text search engine for our knowledge base.

This more than just `LIKE 'word*` and for many searches that involve terms much better than semantic search where semantic search may fail.

This is called Hybrid Search.

https://bigmachine.io/2022/06/12/creating-a-full-text-search-engine-in-postgresql-2022/

<br>