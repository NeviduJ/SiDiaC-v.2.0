## SiDiaC-v.2.0: Sinhala Diachronic Corpus Version 2.0

A curated collection of Sinhala literary texts and related resources with OCR outputs and basic metadata for each work. This repository organizes original PDFs alongside finalized OCR text and machine-readable `metadata.json` files per title.

Paper: [https://aclanthology.org/2026.lrec-1.537/](https://aclanthology.org/2026.lrec-1.537/) (DOI: [10.63317/2ybff4o55vrq](https://doi.org/10.63317/2ybff4o55vrq))

**Hugging Face Dataset:** [https://huggingface.co/datasets/Nevidu/SiDiaC-v.2.0](https://huggingface.co/datasets/Nevidu/SiDiaC-v.2.0)

### Repository structure
- `Books_PDF/`: Original source PDFs for each title.
- `OCR_Final/`: Finalized OCR results per title, each directory containing:
  - `metadata.json`: Minimal bibliographic and processing metadata
  - `<title>.txt`: Plain text content extracted via OCR

### Example metadata.json
```json
{
  "title": "පන්සිය පනස් ජාතක පොත",
  "title_en": "Pansiya Panas Jathaka Potha",
  "author": "Unknown",
  "author_en": "Unknown",
  "genre": "Fiction; Religious",
  "issued_date": "1881",
  "written_date": "1303 - 1333",
  "ocr_confidence": 0.9987
}
```


### Notes
- Filenames and directory names may include Sinhala characters.
- `ocr_confidence` is a heuristic score from the OCR process and may vary by work.

### Citation

```bibtex
@inproceedings{jayatilleke-etal-2026-sidiac,
    title = "{S}i{D}ia{C}-v.2.0: {S}inhala Diachronic Corpus Version 2.0",
    author = "Jayatilleke, Nevidu  and
      de Silva, Nisansa  and
      Sooriya-Arachchi, Uthpala Nimanthi  and
      Kulathilaka, Gagani Kasundhi  and
      Safrullah, Azra  and
      Sofalas, Johan Nevin",
    editor = "Piperidis, Stelios  and
      Bel, N{\'u}ria  and
      van den Heuvel, Henk  and
      Ide, Nancy  and
      Krek, Simon  and
      Toral, Antonio",
    booktitle = "Proceedings of the Fifteenth Language Resources and Evaluation Conference",
    month = may,
    year = "2026",
    address = "Palma de Mallorca, Spain",
    publisher = "ELRA Language Resource Association",
    url = "https://aclanthology.org/2026.lrec-1.537/",
    doi = "10.63317/2ybff4o55vrq",
    pages = "6740--6763",
    abstract = "SiDiaC-v.2.0 is the largest comprehensive Sinhala Diachronic Corpus to date, covering a period from 1800 CE to 1955 CE in terms of publication dates, and a historical span from the 5th to the 20th century CE in terms of written dates. The corpus consists of 244k words across 185 literary works that underwent thorough filtering, preprocessing, and copyright compliance checks, followed by extensive post-processing. Additionally, a subset of 59 documents totalling 70k words was annotated based on their written dates. Texts from the National Library of Sri Lanka were selected from the SiDiaC-v.1.0 non-filtered list, which was digitised using Google Document AI OCR. This was followed by post-processing to correct formatting issues, address code-mixing, include special tokens, and fix malformed tokens. The construction of SiDiaC-v.2.0 was informed by practices from other corpora, such as FarPaHC, SiDiaC-v.1.0, and CCOHA. This was particularly relevant for syntactic annotation and text normalisation strategies, given the shared characteristics of low-resource language status between Faroese and the similar cleaning strategies utilised in CCOHA. This corpus is categorised into two layers based on genres: primary and secondary. The primary categorisation is binary, assigning each book to either Non-Fiction or Fiction. The secondary categorisation is more detailed, grouping texts under specific genres such as Religious, History, Poetry, Language, and Medical. Despite facing challenges due to limited resources, SiDiaC-v.2.0 serves as a comprehensive resource for Sinhala NLP, building upon the work previously done in SiDiaC-v.1.0.",
}
```
