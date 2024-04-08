# Question answering using Llama-2 7b model with 4bit quantization

# used google colab
-----------------------------------------------------------------------------------
# libraries used
-llama-index, transformers, pdfminer.six, vector index

-----------------------------------------------------------------------------------
# input file
-blade runner 2049.pdf

-----------------------------------------------------------------------------------
# input pdf path
-"/content/blade runner 2049.pdf"

-----------------------------------------------------------------------------------
# model and tokenizer used
-"meta-llama/Llama-2-7b-chat-hf" model from huggingface is accessed

-----------------------------------------------------------------------------------
# quantization
- 4 bit quantization is done on top of parameters of the model

- 8 bit quantization can make the system slow and also more RAM is needed

-----------------------------------------------------------------------------------
# prompt template
-- <s> [INST] {query_str} [/INST] this prompt template is used on top of question asked

-----------------------------------------------------------------------------------
# VectorStoreIndex
- this is used to handle the large text or context from the input file for better retrieval of response corresponding to question

#response_mode = Tree Summarize
- gives quality and coherent response for the question asked with minimal hallucination than other response modes such as compact, refine etc.

-----------------------------------------------------------------------------------  


