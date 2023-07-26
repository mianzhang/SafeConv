# SafeConv
Resources for our ACL 2023 paper: "SafeConv: Explaining and Correcting Conversational Unsafe Behavior" [[paper](https://aclanthology.org/2023.acl-long.2.pdf)]


## Data
The splited data is in `data/`. Each line is an instance, which is a dictionary. Below are the meaning of the keys:

| Key      | Meaning  |
| -------- | -------- |
| prompt   | dialogue history  |
| response | current utterance |
| prompt_label | binary safety label of the prompt |
| response_label | binary safety label of the response |
| unsafe_spans_indices | `[start, end]` indices of the unsafe spans in the response |
| rewrites | rewritten utterances |

## Cite
You could cite our paper if you find the dataset is helpful:
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