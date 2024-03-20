# Intent detection and slot filling


## Famous DATASETS used in various papers for intent detection : 

1. ATIS => Airline travel information system 
	- [Kaggle](https://www.kaggle.com/datasets/hassanamin/atis-airlinetravelinformationsystem)

	- [Hugging face](https://huggingface.co/datasets/fathyshalab/atis_intents)
	- [Paper1](https://paperswithcode.com/paper/a-bi-model-based-rnn-semantic-frame-parsing) || [paper2](https://arxiv.org/abs/1812.10235v1)
		
2. SNIPS => The SNIPS Natural Language Understanding benchmark is a dataset of over 16,000 crowdsourced queries distributed among 7 user intents of various complexity
	- [Dataset](https://paperswithcode.com/dataset/snips)
	- [Hugging face](https://huggingface.co/datasets/snips_built_in_intents)
	- [paper](https://arxiv.org/abs/2303.10606v1)
	- [github link](https://github.com/rafiepour/CTran)

3. BANKING => 
	- [Paper1](https://arxiv.org/pdf/2003.04807.pdf)
	- [Hugging face](https://huggingface.co/datasets/banking77)
	- [paper2](https://arxiv.org/abs/2302.05096v1)



## Check out hindi intent classification 
1. https://huggingface.co/datasets/cfilt/HiNER-original
2. https://huggingface.co/datasets/bbc_hindi_nli
3. https://microsoft.github.io/GLUECoS/ hindi training 


## Implementation and paper on github related to intent detection and slot filling 

1. [BERT for Joint Intent Classification and Slot Filling - DONE](https://paperswithcode.com/paper/bert-for-joint-intent-classification-and-slot)

2. [A Prompt Learning Based Intent Recognition Method on a Chinese Implicit Intent Dataset CIID - DONE](https://link.springer.com/article/10.1007/s11063-023-11362-6)

3. [Efficient Intent Detection with Dual Sentence Encoders](https://paperswithcode.com/paper/efficient-intent-detection-with-dual-sentence)

4. [Explicit Slot-Intent Mapping with Bert for Joint Multi-Intent Detection and Slot Filling - Need to explore](https://ieeexplore.ieee.org/abstract/document/9747477) 

5. [Multi-lingual Intent Detection and Slot Filling in a Joint BERT-based Model](https://arxiv.org/abs/1907.02884) 

6. [Joint intent detection and slot filling using weighted finite state transducer and BERT](https://link.springer.com/article/10.1007/s10489-022-03295-9) 

7. [BERT for Joint Intent Classification and Slot Filling](https://arxiv.org/abs/1902.10909)

## calculating similarity between sentences

1. For vectorization use **bert** then you can use 
    1. Cosine similarity 
2. **Semantic Textual Similarity (STS) Metrics**: These metrics, such as Pearson correlation or Spearman rank correlation, are designed specifically for assessing the semantic similarity between two pieces of text. They are often used in NLP benchmarks.
3. **BLEU (Bilingual Evaluation Understudy)**: Originally designed for machine translation evaluation, BLEU measures the n-gram overlap between the generated sentence and a reference (paragraph in this case). It can be adapted for similarity by treating the paragraph as a reference.
4. **Word Mover's Distance (WMD)**: WMD calculates the minimum cumulative distance that words in one document need to travel to match the words in another document. It considers semantic similarity and can be effective for measuring the distance between a sentence and a paragraph.
5. **Fine-Tuned Models**: Alternatively, you can use fine-tuned BERT models that are specifically trained for sentence similarity tasks. These models may provide more accurate similarity scores tailored to your specific application.
6. **Sentence Transformers**: There are libraries and models built on top of BERT, such as Sentence Transformers, which provide ready-to-use implementations for computing sentence embeddings and similarity scores. These models are trained to generate semantically meaningful sentence embeddings that capture similarity effectively.
7. Jaccard simmilarity
