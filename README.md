

# 📷CAMERA dataset
CAMERA (CyberAgent Multimodal Evaluation for Ad Text GeneRAtion) is the Japanese ad text generation dataset.
We hope that our dataset will be useful in research for realizing more advanced ad text generation models.
The dataset is split into `train.csv`, `dev.csv`, and `test.csv`. LP (Landing Pages) images are stored in the `lp-screenshot/` and are associated with the text data (`*.csv`) by asset ids (`asset_id`).

# Updats
- [Our paper](https://aclanthology.org/2024.acl-long.54/) has been accepted to [ACL2024](https://2024.aclweb.org/)🎉[2024-08-13]
  - Major updates have been made to the dataset accordingly (V2.2.0).



# Dataset
- [Download the CAMERA dataset w/o LP images (ver.2.2.0 | 126.2 MiB)](https://storage.googleapis.com/camera-public/camera-v2.2-minimal.tar.gz)
- [Download the CAMERA dataset w/ LP images (ver.2.2.0 | 61.5 GiB)](https://storage.googleapis.com/camera-public/camera-v2.2.tar.gz)

Note: The `wget` command is not available.

You can also access this dataset via the [Hugging Face Hub](https://huggingface.co/datasets/cyberagent/camera). 


|  Name  |  Description  |
| ---- | ---- |
|  asset_id  |  ids (associated with LP images)  |
|  kw  |  search keyword  |
|  lp_meta_description  |  meta description extracted from LP (i.e., LP Text)|
|  title_org  |  ad text (original gold reference) |
|  title_ne{1-3}  |  ad text (additional gold references for multi-reference evaluation |
|  domain  |  industry domain (HR, EC, Fin, Edu) for industry-wise evaluation |
|  parsed_full_text_annotation  |  OCR results for LP images  |





# Citation
Thank you for your interest in our dataset. If you use it in your research, please cite:

```
@inproceedings{mita-etal-2024-striking,
    title = "Striking Gold in Advertising: Standardization and Exploration of Ad Text Generation",
    author = "Mita, Masato  and
      Murakami, Soichiro  and
      Kato, Akihiko  and
      Zhang, Peinan",
    editor = "Ku, Lun-Wei  and
      Martins, Andre  and
      Srikumar, Vivek",
    booktitle = "Proceedings of the 62nd Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers)",
    month = aug,
    year = "2024",
    address = "Bangkok, Thailand and virtual meeting",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2024.acl-long.54",
    pages = "955--972",
    abstract = "In response to the limitations of manual ad creation, significant research has been conducted in the field of automatic ad text generation (ATG). However, the lack of comprehensive benchmarks and well-defined problem sets has made comparing different methods challenging. To tackle these challenges, we standardize the task of ATG and propose a first benchmark dataset, CAMERA, carefully designed and enabling the utilization of multi-modal information and facilitating industry-wise evaluations. Our extensive experiments with a variety of nine baselines, from classical methods to state-of-the-art models including large language models (LLMs), show the current state and the remaining challenges. We also explore how existing metrics in ATG and an LLM-based evaluator align with human evaluations.",
}
```

# License
This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License.](https://creativecommons.org/licenses/by-nc-sa/4.0/)
