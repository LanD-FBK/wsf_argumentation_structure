# WSF argumentative structure annotation
This dataset comprises 227 annotated examples from the [White Supremacy Forum dataset](https://github.com/Vicomtech/hate-speech-dataset/tree/master) (WSF, de Gibert et al., 2018), obtained via human-machine collaboration.

![alt text](https://github.com/LanD-FBK/wsf_argumentation_structure/blob/main/example_wsf_arg.png)

## Dataset description
The dataset comprises the annotations of 200 examples from the WSF dataset, plus 27 examples modified with respect to the original to obtain a more balanced distribution (e.g. more examples where the weak part is not identical to the hateful part).

## File description
We provide the data in json and csv format. Each entry in the dataset has 12 fields: the ``file_id`` from the original WSF dataset, a unique index for each example in this dataset (``idx``), the text of the posts, which in some cases was edited from the original as explained in the paper (``text_ed``), the Implied Statement (``IS``), the extracted premises (``premise0``, ``premise1``, ``premise2``) and conclusion (``conclusion``), the concatenation of premises and conclusion (``concat``), the weak part (``weak``), and the annotation of whether each extracted element is hateful (``premise0_hate``, ``premise1_hate``, ``premise2_hate``, ``conclusion_hate``).

## Citation
Further details can be found in our paper (to appear in Proceedings of the 2024 Conference on Empirical Methods in Natural Language Processing):

Helena Bonaldi, Greta Damo, Nicolás Benjamín Ocampo, Elena Cabrio, Serena Villata and Marco Guerini. 2024. Is Safer Better? The Impact of Guardrails on the Argumentative Strength of LLMs in Hate Speech Countering. Proceedings of the 2024 Conference on Empirical Methods in Natural Language Processing. 2024.

```
@inproceedings{bonaldi-etal-2024-safer,
    title = "Is Safer Better? The Impact of Guardrails on the Argumentative Strength of {LLM}s in Hate Speech Countering",
    author = "Bonaldi, Helena  and
      Damo, Greta  and
      Ocampo, Nicol{\'a}s Benjam{\'\i}n  and
      Cabrio, Elena  and
      Villata, Serena  and
      Guerini, Marco",
    editor = "Al-Onaizan, Yaser  and
      Bansal, Mohit  and
      Chen, Yun-Nung",
    booktitle = "Proceedings of the 2024 Conference on Empirical Methods in Natural Language Processing",
    month = nov,
    year = "2024",
    address = "Miami, Florida, USA",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2024.emnlp-main.201",
    doi = "10.18653/v1/2024.emnlp-main.201",
    pages = "3446--3463"
}


```
