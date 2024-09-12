# TAFILAT Dataset: Comprehensive Solution Space for Arabic Poetic Meters

 <p align="center"> 
 <img src = "https://raw.githubusercontent.com/droaas/Tafilat/main/images/TafilatLogo.png" width = "200px"/>
 </p>
*A complete dataset offering all possible patterns for Arabic poetic meters, meticulously curated from classical prosody sources. Designed to automate and enhance research in Arabic meter classification and poetry generation.*

## Table of Contents
1. [Introduction](#introduction)
2. [Dataset Summary](#dataset-summary)
3. [Data Description](#data-description)
4. [Methodology](#methodology)
   - [Step 1: Pattern Generation](#step-1-pattern-generation)
   - [Step 2: Database Construction](#step-2-database-construction)
   - [Step 3: Verification and Evaluation](#step-3-verification-and-evaluation)
5. [Importance and Applications](#importance-and-applications)
6. [Sample Data](#sample-data)
7. [How to Use the Dataset](#how-to-use-the-dataset)
8. [Future Work](#future-work)
9. [Contributing](#contributing)
10. [License](#license)

## Introduction
Arabic poetry has long held a profound significance in the cultural fabric of the Arab world, with strict metrical rules ensuring its precision and beauty. Traditional Arabic prosody, known as **‘Ilm al-‘Arud**, employs a well-defined system of meters (taf'ilat) that are crucial for poets to avoid any deviations in meter, known as **taksir** (metrical errors).

However, modern researchers often limit their work to identifying only the main meters, overlooking the intricate details of their various patterns. The **TAFILAT** dataset addresses this gap by providing a comprehensive solution space for all possible taf’ilat patterns across the Arabic poetic meters, drawn from over 1,200 years of prosodic tradition.

This dataset is a powerful resource for scholars and AI researchers aiming to deepen their understanding of Arabic meter classification, automate poetic analysis, or generate metrically accurate Arabic poetry.

## Dataset Summary
**TAFILAT** is a dataset that includes all possible patterns of Arabic poetic meters. The dataset was built following the rigorous traditional rules of Arabic prosody from six authoritative sources and verified by two experts in the field. The dataset encompasses the full range of 16 primary meters introduced by Al-Khalil ibn Ahmad Al-Farahidi, as well as the variations introduced by **zihafat** (substitutions) and **‘ilal** (deviations).

The dataset includes:
- **16 poetic meters** (bahrs)
- **Taf’ilat patterns** with various **modifications** (zihafat and ‘ilal)
- **Prosodic symbols** (0 for consonants and 1 for vowels)
- **Meter-specific patterns** for each poetic verse
- **Details of each taf'ila** and its modifications
- **Rhyme scheme** indicators

By offering a structured solution space for Arabic meter, this dataset enables the automation and deeper understanding of poetic analysis and classification tasks.

## Data Description
The dataset is organized into a table with the following key attributes:
1. **Poetic Meter (Bahr)**: The metrical form of the poem.
2. **Taf’ilat Count**: The number of taf’ilat, which can be 2, 3, 4, 6, or 8.
3. **Modification Status**: Indicates if the pattern has zihafat (substitutions) or ‘ilal (modifications).
4. **Prosodic Symbols**: Binary encoding (0 for consonants, 1 for vowels).
5. **Taf’ilat**: The actual taf’ilat pattern for each poetic meter.
6. **Taf’ila Details**: Specific details about the modifications (zihafat or ‘ilal) for each pattern.
7. **Rhyme Symbol**: Encoded form of the rhyme scheme.
8. **Rhyme Boundaries**: Boundaries of the rhyme pattern.

## Methodology

### Step 1: Pattern Generation
We applied the **Qawafi system** to generate metrical patterns based on four key prosodic traditions:
- **Al-Khalil ibn Ahmad's System**: Covers 16 classical Arabic poetic meters, focusing on classical Arabic poetry known as "Qasidah."
- **Modern Additions to Al-Khalil's System**: Includes new meters used in colloquial Arabic poetry introduced by modern poets.
- **Borrowed Meters**: Includes borrowed meters from other literary traditions, such as the Persian-origin "Dobayti."
- **Free Verse Taf'ilat-Based Poetry**: Focuses on modern free verse poetry that adheres to taf'ilat without strict adherence to a specific meter.

*Note: The current dataset covers only the traditional system of Al-Khalil ibn Ahmad.*

### Step 2: Database Construction
In this step, we built the **TAFILAT** database, carefully cataloging every valid pattern for each meter. Only the classical meters from Al-Khalil's system were used in this phase. The dataset represents a full solution space for metrical analysis, encoding every possible pattern.

### Step 3: Verification and Evaluation
Linguistic experts evaluated the dataset’s accuracy, ensuring its reliability for further research. The taf’ilat were cross-verified against traditional sources and modern interpretations of Arabic poetic meter.

![Methodology Overview](path/to/methodology-image.png)

## Importance and Applications
The **TAFILAT** dataset offers significant benefits to researchers and developers working in Arabic prosody, machine learning, and natural language processing (NLP):
- **Metrical Analysis**: Facilitates the study and analysis of Arabic poetic meters.
- **Automated Poetry Evaluation**: Helps in developing systems for automated evaluation of poetic structure and adherence to classical meters.
- **NLP and Machine Learning**: The dataset can be integrated into NLP or machine learning models for tasks like automated poetry generation, prosodic analysis, and verse classification.
- **Pedagogical Tools**: Useful for teaching Arabic poetry and prosody in both academic and informal settings.
## Sample Data
Here is a brief look at a sample from the **TAFILAT** dataset:

| Bahr       | Taf’ilat Count | Prosodic Symbols | Taf'ilat        | Modifications | Rhyme Symbol | Boundary |
|------------|----------------|------------------|-----------------|---------------|--------------|----------|
| Tawil      | 8              | 1010101010       | Fa'ulun Mafailun | Zihaf: Qabadh  | 0101         | 110      |
| Basit      | 6              | 110110110        | Mustaf'ilun Fa'ilun | Zihaf: Khabn | 1100         | 001      |

## How to Use the Dataset
The **TAFILAT** dataset is available in CSV format and can be integrated into various Natural Language Processing (NLP) or machine learning projects related to Arabic prosody and poetry analysis. To access the dataset:

1. **Clone the repository**:
   You can clone the repository to your local machine using the following command:
   ```bash
   git clone https://github.com/yourusername/TAFILAT.git

2. **Access detailed instructions**:
   For comprehensive guidelines on how to use the dataset, including sample code and practical applications, visit the [Google Colab notebook](https://colab.research.google.com/your-notebook-link), where you’ll find step-by-step instructions.

---

## Future Work
The **TAFILAT** dataset is a foundational tool for Arabic meter research, and we envision several future expansions, including:

- **Incorporating Modern Meters**: Extending the dataset to include modern Arabic meters that are used in free verse and contemporary poetry, allowing a more comprehensive analysis.
- **Enhancing Prosodic Visualization**: Developing visual tools to represent taf’ilat patterns interactively, aiding in the intuitive understanding of complex poetic structures.
- **Integration with Generative AI**: Combining the dataset with AI models to create automated Arabic poem generation systems that follow classical metrical rules.
- **Expansion to Other Dialects**: Including meters from Arabic dialectal poetry and prosodic patterns in non-classical forms, enriching the dataset for broader applications.

## Contributing
We welcome contributions from the community! Whether you are an expert in Arabic prosody, a data scientist, or a developer interested in enhancing this dataset, your input is valuable. To contribute:

1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Make your changes and add tests if applicable.
4. Submit a pull request with a detailed description of your changes.

Please refer to our [CONTRIBUTING.md](CONTRIBUTING.md) file for more information.

## License
The **TAFILAT** dataset is open-source and is licensed under the [MIT License](LICENSE.md). Feel free to use, modify, and distribute the dataset in your research or applications, as long as proper attribution is given.
