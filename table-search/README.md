This file describes a sample of our WebQueryTable dataset.

If you use this dataset, plese cite
@article{yan2017content,
  title={Content-Based Table Retrieval for Web Queries},
  author={Yan, Zhao and Tang, Duyu and Duan, Nan and Bao, Junwei and Lv, Yuanhua and Zhou, Ming and Li, Zhoujun},
  journal={arXiv preprint arXiv:1706.02427},
  url={https://arxiv.org/pdf/1706.02427.pdf},
  year={2017}
}


Our dataset contains 3 files:

1) WQT.dataset.query.tsv lists queries in the dataset
Each line in this file denotes a <QueryID, Query> pair, and the format is
QueryID \t QueryText


2) WQT.dataset.table.tsv lists tables in the dataset
A table includes {TableID, Source, Caption, Sub-Caption, ColumnStr, CellStr, URL}. 
Source: WebQuery or Wiki
ColumnStr: joined by " _|_ "
CellStr: Adjacent cells are joined by " _|_ ".  Adjacent lines are joined by " _||_ ".


For example:
[Table]:
+----+------+
| ID | Name |
| 0  | A    |
| 1  | B    |
+----+------+

==>

[ColumnStr]: "ID _|_ Name"
[CellStr]: "0 _|_ A _||_ 1 _|_ B"


3) WQT.dataset.query-table.tsv lists triples of <queryID, TableID, label>.
The label "1" means the table is relevant to the query, and "0" means the table is irrelevant.
