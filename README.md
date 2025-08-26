This jupyternotebook walks you through the process used for the PERC proceeding. You can clone this repo and run this using your own data. 

Keep in mind that the data used in the paper (articles' whole text) is under copyright protection and cannot be hosted. The notebook expects the following:

ajp_perc_prper_tpt_text_chunks_embeddings_jinav3_5.pkl <-- a pickled pandas.dataframe object with the following columns: 

'doi' -- DOI corresponding to each sentence chunk
'year' -- Year each DOI was published
'journal' -- Journal it was published in
'sentence_chunk' -- Plain text sentence chunk from the DOI
'chunk_char_count' -- Number of characters in a chunk, not used
'chunk_word_count' -- Number of words in a chunk, not used
'chunk_token_count' -- number of tokens in a chunk
'embedding' -- The embedding vectors for each sentence chunk
'title' -- Title of the paper the chunk corresponds to

Must have a Jina V3 key from huggingface. 
