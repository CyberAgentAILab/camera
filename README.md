# 📷CAMERA dataset
CAMERA (CyberAgent Multimodal Evaluation for Ad Text GeneRAtion) is the Japanese ad text generation dataset.
We hope that our dataset will be useful in research for realizing more advanced ad text generation models.
The dataset is splitted into `train.csv`, `dev.csv`, and `test.csv`. LP (Landing Pages) images are stored in the `lp-screenshot/` and are associated with the text data (`*.csv`) by asset ids (`asset_id`).



# Dataset
- [Download the CAMERA dataset w/o LP images (ver.1.0.0 | 126.2 MiB)](https://storage.googleapis.com/camera-public/camera-v1-minimal.tar.gz)
- [Download the CAMERA dataset w/ LP images (ver.1.0.0 | 61.5 GiB)](https://storage.googleapis.com/camera-public/camera-v1.tar.gz)

Note: The `wget` command is not available.

You can also access this dataset via the [Hugging Face Hub](https://huggingface.co/datasets/shunk031/CAMERA). 

|  Name  |  Description  |
| ---- | ---- |
|  asset_id  |  ids (associated with LP images)  |
|  kw  |  search keyword  |
|  lp_meta_description  |  meta description extracted from LP (i.e., LP Text)|
|  title_org  |  ad text (original gold reference) |
|  title_ne{1-3}  |  ad text (additonal gold references for multi-reference evaluation |
|  domain  |  industry domain (HR, EC, Fin, Edu) for industry-wise evaluation |
|  parsed_full_text_annotation  |  OCR results for LP images  |





# Citation
Thank you for your interest in our dataset. If you use it in your research, please cite:

```
@inproceedings{mita-et-al:nlp2023,
	author =	"三田 雅人 and 村上 聡一朗 and 張 培楠",
	title =		"広告文生成タスクの規定とベンチマーク構築", 
	booktitle =	"言語処理学会 第29回年次大会",
	year =		2023,
	}
```

# License
This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License.](https://creativecommons.org/licenses/by-nc-sa/4.0/)
