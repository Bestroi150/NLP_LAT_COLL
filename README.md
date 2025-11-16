# NLP_LAT_COLL

A Natural Language Processing collection for Latin texts, featuring the *Satyricon* corpus with tokenized data and XML markup.

## Overview

This project contains annotated Latin text data from the *Satyricon* by Petronius, processed for computational linguistic analysis. The collection includes both complete and selected text versions with corresponding tokenized data and schema definitions.

## Contents

- **SatyriconFullText.txt** - Complete text of the Satyricon
- **SatyriconSelectedText.txt** - Curated selection of Satyricon excerpts
- **corpus_sermo_vulgaris.xml** - XML-formatted corpus with linguistic annotations
- **corpus_sermo_vulgaris_token.csv** - Tokenized data in CSV format for analysis
- **corpus_sermo_vulgaris.xsd** - XML Schema Definition for corpus validation

## Project Structure

```
NLP_LAT_COLL/
├── SatyriconFullText.txt
├── SatyriconSelectedText.txt
├── corpus_sermo_vulgaris.xml
├── corpus_sermo_vulgaris_token.csv
├── corpus_sermo_vulgaris.xsd
├── README.md
└── LICENSE
```

## Usage

### Working with XML Data
The XML corpus follows the schema defined in `corpus_sermo_vulgaris.xsd`. Load the corpus using XML parsers:

```python
import xml.etree.ElementTree as ET
tree = ET.parse('corpus_sermo_vulgaris.xml')
root = tree.getroot()
```

### Analyzing Tokenized Data
The CSV file contains tokenized Latin text. Load it with pandas or similar tools:

```python
import pandas as pd
df = pd.read_csv('corpus_sermo_vulgaris_token.csv')
```

### Text Analysis
Use the provided text files for direct text analysis and processing tasks.

## Data Format

### XML Format
- Structured linguistic annotations
- Compliant with schema in `corpus_sermo_vulgaris.xsd`
- Suitable for validation and complex queries

### CSV Format
- One token per row
- Columns for lemmatization, part-of-speech, and morphological features
- Efficient for statistical analysis

## Requirements

- Python 3.7+
- Libraries: pandas, lxml (optional for advanced XML processing)

## Installation

Clone the repository:
```bash
git clone https://github.com/Bestroi150/NLP_LAT_COLL.git
cd NLP_LAT_COLL
```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Author

Bestroi150

## Citation

If you use this corpus in academic work, please cite:

```bibtex
@dataset{nlp_lat_coll,
  title={NLP Latin Collection: Satyricon Corpus},
  author={Kristiyan Simeonov},
  year={2025},
  url={https://github.com/Bestroi150/NLP_LAT_COLL}
}
```

## Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues for improvements and suggestions.

## Disclaimer

This corpus is provided for educational and research purposes. Users are responsible for complying with any applicable licensing restrictions related to classical texts and their derivatives.
