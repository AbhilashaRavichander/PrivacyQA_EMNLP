# Question Answering for Privacy Policies


This repository contains the PrivacyQA dataset described in the EMNLP 2019 paper, [Question Answering for Privacy Policies: Combining Computational and Legal Perspectives] (https://arxiv.org/abs/1911.00841). PRIVACYQA is a corpus consisting of 1750 questions about the contents of privacy policies, paired with expert annotations. The goal of this effort is to kickstart the development of question-answering methods for this domain, to address the (unrealistic) expectation that a large population should be reading many policies per day.

The data has been partitioned into a train and test set. The same split has been used in the experiments reported in the paper. 

The data is in a tab seperated format with the following fields:
1) Folder	: Physical location of app data and metadata.
2) DocID	: Unique identifier for privacy policy
3) QueryID	: Unique identifier for query
4) SentID	: Unique identifier for sentence
5) Split	: Train or test split
6) Query	: Text field consisting of crowdsourced question against policy
7) Segment	: Sentence from privacy policy
8) Ann0, Ann1, Ann2,	Ann3,	Ann4, Ann5 and Ann6: {Relevant, Irrelevant, None} None: annotation should not be considered. Relevant: Segment is relevant for query. Irrelevant: segment is irrelevant for query.

If you make use of this dataset in your research, we ask that you please cite our paper:

```  
@inproceedings{ravichander-etal-2019-question,
    title = "Question Answering for Privacy Policies: Combining Computational and Legal Perspectives",
    author = "Ravichander, Abhilasha  and
      Black, Alan W  and
      Wilson, Shomir  and
      Norton, Thomas  and
      Sadeh, Norman",
    booktitle = "Proceedings of the 2019 Conference on Empirical Methods in Natural Language Processing and the 9th International Joint Conference on Natural Language Processing (EMNLP-IJCNLP)",
    month = nov,
    year = "2019",
    address = "Hong Kong, China",
    publisher = "Association for Computational Linguistics",
    url = "https://www.aclweb.org/anthology/D19-1500",
    doi = "10.18653/v1/D19-1500",
    pages = "4949--4959",
    abstract = "Privacy policies are long and complex documents that are difficult for users to read and understand. Yet, they have legal effects on how user data can be collected, managed and used. Ideally, we would like to empower users to inform themselves about the issues that matter to them, and enable them to selectively explore these issues. We present PrivacyQA, a corpus consisting of 1750 questions about the privacy policies of mobile applications, and over 3500 expert annotations of relevant answers. We observe that a strong neural baseline underperforms human performance by almost 0.3 F1 on PrivacyQA, suggesting considerable room for improvement for future systems. Further, we use this dataset to categorically identify challenges to question answerability, with domain-general implications for any question answering system. The PrivacyQA corpus offers a challenging corpus for question answering, with genuine real world utility.",
}
```


