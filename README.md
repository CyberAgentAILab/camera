# 📷CAMERA dataset
CAMERA (CyberAgent Multimodal Evaluation for Ad Text GeneRAtion) is the Japanese ad text generation dataset.
We hope that our dataset will be useful in research for realizing more advanced ad text generation models.
The dataset is splitted into `train.csv`, `dev.csv`, and `test.csv`. LP (Landing Pages) images are stored in the `lp-screenshot/` and are associated with the text data (`*.csv`) by asset ids (`asset_id`).



# Dataset
- [Download the CAMERA dataset w/o LP images (ver.2.2.0 | 126.2 MiB)](https://storage.googleapis.com/camera-public/camera-v2.2-minimal.tar.gz)
- [Download the CAMERA dataset w/ LP images (ver.2.0.0 | 61.5 GiB)](https://storage.googleapis.com/camera-public/camera-v2.tar.gz)

Note: The `wget` command is not available.


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
@misc{mita2024striking,
      title={Striking Gold in Advertising: Standardization and Exploration of Ad Text Generation}, 
      author={Masato Mita and Soichiro Murakami and Akihiko Kato and Peinan Zhang},
      year={2024},
      eprint={2309.12030},
      archivePrefix={arXiv},
      primaryClass={id='cs.CL' full_name='Computation and Language' is_active=True alt_name='cmp-lg' in_archive='cs' is_general=False description='Covers natural language processing. Roughly includes material in ACM Subject Class I.2.7. Note that work on artificial languages (programming languages, logics, formal systems) that does not explicitly address natural-language issues broadly construed (natural-language processing, computational linguistics, speech, text retrieval, etc.) is not appropriate for this area.'}
}
```

# License
This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License.](https://creativecommons.org/licenses/by-nc-sa/4.0/)
