This file describes a sample of our Table2Text dataset.

If you use this dataset, plese cite
@article{bao2018table,
  title={Table-to-Text: Describing Table Region with Natural Language},
  author={Bao, Junwei and Tang, Duyu and Duan, Nan and Yan, Zhao and Lv, Yuanhua and Zhou, Ming and Zhao, Tiejun},
  journal={arXiv preprint arXiv:1805.11234},
  year={2018}
}


Our dataset contains training/dev/test files. The format of each file is as follows.

Number of columns + “\t” + column names + “\t” + cell values + “\t” + descriptive sentence
"_||_" is used to split different column names/cell values.
