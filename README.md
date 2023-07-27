# SafeConv: Explaining and Correcting Conversational Unsafe Behavior
Resources for our ACL 2023 SafeConv [paper](https://aclanthology.org/2023.acl-long.2.pdf).

## What is SafeConv?
SafeConv is a large-scale dataset (160000 prompt-response pairs) with comprehensive annotations
for conversational safety:
1) binary safety label of the prompt; 
2) binary safety label of the response; 
3) unsafe spans in the response; 
4) safe alternatives for the unsafe responses.


## Data
The splited data is in `data/`. Each line is an instance, which is a dictionary. Below are the meaning of the keys:

| Key      | Meaning  |
| -------- | -------- |
| source   | data source; 'P' denotes [Pchatbot](https://arxiv.org/abs/2009.13284); 'L' denotes [LCCC](https://arxiv.org/abs/2008.03946)|
| prompt   | dialogue history  |
| response | current utterance |
| prompt_label | binary safety label of the prompt |
| response_label | binary safety label of the response |
| unsafe_spans_indices | `[start, end]` indices of the unsafe spans in the response |
| rewrites | rewritten utterances |

## Cite
You could cite our paper if you find the dataset is helpful using this BibTeX:
```
@inproceedings{zhang-etal-2023-safeconv,
    title = "{S}afe{C}onv: Explaining and Correcting Conversational Unsafe Behavior",
    author = "Zhang, Mian  and
      Jin, Lifeng  and
      Song, Linfeng  and
      Mi, Haitao  and
      Chen, Wenliang  and
      Yu, Dong",
    booktitle = "Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers)",
    month = jul,
    year = "2023",
    address = "Toronto, Canada",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2023.acl-long.2",
    pages = "22--35",
}
```
