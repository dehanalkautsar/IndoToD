# IndoToD: A Multi-Domain Indonesian Benchmark For End-to-End Task-Oriented Dialogue Systems

This is the dataset repository of IndoToD, presented at SEALP 2023, colocated with AACL 2023, where our paper was honored with the Best Paper Award 🏆 [[ACL Anthology]](https://aclanthology.org/2023.sealp-1.7.pdf).

This code has been written using PyTorch. If you use source codes or datasets included in this toolkit in your work, please cite the following paper:
<pre>
@inproceedings{kautsar2023indotod,
  title={IndoToD: A Multi-Domain Indonesian Benchmark For End-to-End Task-Oriented Dialogue Systems},
  author={Kautsar, Muhammad and Nurdini, Rahmah and Cahyawijaya, Samuel and Winata, Genta and Purwarianti, Ayu},
  booktitle={Proceedings of the First Workshop in South East Asian Language Processing},
  pages={85--99},
  year={2023}
}
</pre>

We introduce two Indonesian ToD datasets, comprising four different domains by delexicalization to efficiently reduce the size of annotations. To ensure a high-quality data collection, we hire native speakers to manually annotate the dialogues. We annotated the data from existing English ToD datasets: CamRest and SMD. Along with the original English datasets, these new Indonesian datasets serve as an effective benchmark for evaluating Indonesian and English ToD systems as well as exploring the potential benefits of cross-lingual and bilingual transfer learning approaches.

## IndoCamRest

IndoCamRest is a synthetic task-oriented dialogue system dataset that translated from Cambridge Restaurant 676 (CamRest) dataset (Wen et al., 2016) into the new Indonesian parallel dataset. The statistics of IndoCamRest can be seen below:

| Statistics | Value |
| ------ | ------ |
| \# of dialogues | 676 |
| \# of domains | 1; restaurant search |
| \# of intents | 2; inform, request |
| \# of informable slot types | 3; area, food, pricerange |
| \# of requestable slot types | 6; area, food, pricerange, postcode, phone, address |
| \# of distinct entities | 110 |
| Avg. \# of turns per dialogue | 4.06 |
| Avg. \# of tokens per utterance | 9.54 |
| Distinct slot values | 88 |
| Vocabulary size (Lexicalized) | 1103 |
| Vocabulary size (Delexicalized) | 829 |

## IndoSMD

IndoSMD is a synthetic task-oriented dialogue system dataset that translated from In-Car Assistant (SMD) dataset (Eric et al., 2017) into the new Indonesian dataset. The statistics of IndoSMD can be seen below:

| Statistics | Value |
| ------ | ------ |
| \# of dialogues | 323 |
| \# of domains | 3; POI Navigation, Calendar Scheduling, Weather Information Retrieval |
| \# of slot types | 15 |
| \# of distinct entities | 325 |
| Avg. \# of Turns per dialogue | 2.63 |
| Avg. \# of Tokens per utterance | 8.14 |
| Vocabulary size (Lexicalized) | 883 |
| Vocabulary size (Delexicalized) | 577 |

Per-domain in detail:
| Statistic | POI Navigation Domain | Calendar Scheduling Domain | Weather Information Retrieval Domain |
| ----- | ----- | ----- | ----- |
| # of dialogues | 100  | 114 | 109 |
| # of slot types | 5 (POI name, traffic info, POI category, address, distance) | 6 (event, time, date, party, room, agenda) | 4 (location, weekly time, temperature, weather attribute) |
| # of distinct slot values | 131 | 79 | 78 |

# License
The datasets are under CC-BY-SA 4.0 and the code is license under Apache 2.0.
