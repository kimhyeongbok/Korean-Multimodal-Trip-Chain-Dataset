# Korean Multimodal Trip-Chain Dataset (KMTC)

**KMTC** is a Korean multimodal mobility dataset consisting of **10,000 trip-chain records** collected in the Seoul metropolitan area, including **private-car** and **public-transit** mobility records.

The dataset integrates structured trip attributes, GPS trajectories, voice narratives, transcriptions, generated mobility descriptions, and mobility question-answering annotations. It is designed to support research on personalized mobility intelligence, mobility question answering, Korean speech understanding, and multimodal AI.
![Uploading Korean_Multimodal_Trip_Chain_Dataset_page2_image.png…]()

> **Dataset access is available upon request.**  
> Please submit the request form here:  
> **[KMTC Dataset Request Form](https://forms.gle/2ZsivZjhkUnJpRKw5)**

## Dataset Overview

KMTC contains:

- **10,000 trip-chain records**
  - 5,000 private-car trip chains
  - 5,000 public-transit trip chains
- Data collected from **1,024 crowd-workers**
- Geographic coverage:
  - Seoul
  - Gyeonggi-do
  - Incheon
- Modalities:
  - Structured trip information
  - GPS trajectories where applicable
  - Voice narratives
  - Human-refined transcriptions
  - Generated mobility descriptions
  - Mobility QA annotations

The dataset was collected using a custom-developed mobile application named **Tripchain**, through which participants selected a travel mode, entered structured trip attributes, recorded GPS trajectories where applicable, and provided voice narratives about their route choices, travel preferences, and subjective travel experiences. :contentReference[oaicite:0]{index=0}

## Dataset Components

| Component | Format | Description |
|---|---|---|
| Trip Information | JSON | User demographics, trip purpose, origin/destination, weather, costs, and related metadata |
| GPS Trajectories | CSV | Timestamped GPS points including latitude, longitude, and speed, provided for private-car trips |
| Voice Recordings | MP3 | Raw voice narratives recorded during trips |
| Voice Transcriptions | JSON | Text transcriptions of the voice narratives refined through human review |
| Generated Descriptions | JSON | Multi-sentence mobility descriptions generated from structured trip data and voice narratives |
| Mobility QA Annotations | JSON | Question-answering annotations for mobility-related reasoning and retrieval tasks |

## Research Applications

KMTC can be used for research in:

- Personalized mobility intelligence
- Mobility question answering
- Retrieval-Augmented Generation (RAG)
- Korean automatic speech recognition
- Speech-based travel-context understanding
- Human mobility analysis
- Route-choice behavior modeling
- Multimodal AI
- Urban mobility and transportation research

## Data Collection Area

The dataset covers the Seoul metropolitan area, including **Seoul**, **Gyeonggi-do**, and **Incheon**. This region provides diverse urban, suburban, coastal, and inter-regional mobility environments, making it suitable for studying heterogeneous mobility patterns. :contentReference[oaicite:1]{index=1}

## Quality Validation

The dataset underwent quality assurance and validation, including automated checks, human review, and external verification. Reported quality metrics include:

| Metric | Private Car | Public Transit |
|---|---:|---:|
| Structure Accuracy | 100% | 100% |
| Format Accuracy | 99.99% | 100% |
| Transcription Accuracy | 98.91% | 99.45% |
| QA Appropriateness | 96.20% | 98.92% |
| Trip-Voice Consistency | 99.90% | 100.0% |

## Baseline Experiments

The dataset includes baseline evaluations for two representative downstream tasks:

| Task | Model | Metric | Result |
|---|---|---|---|
| Mobility QA | EEVE 10.8B | Context Precision | 78.16% / 80.55% |
| ASR | Whisper Large-v3 | Character Error Rate (CER) | 5.40% / 11.59% |

Results are reported separately for private-car and public-transit data.

## Privacy and Ethics

All participants provided informed consent prior to data collection. Personal identifiable information was masked or generalized, and voice recordings were processed to reduce speaker identifiability. Address and GPS-related information were handled using privacy-preserving preprocessing measures. :contentReference[oaicite:2]{index=2}

Users of this dataset must not attempt to identify, re-identify, contact, track, or profile any individual, participant, vehicle, household, or location from the dataset.

## Access

The dataset is available upon request for **non-commercial research and academic purposes**.

To request access, please complete the following form:

**[KMTC Dataset Request Form](https://forms.gle/2ZsivZjhkUnJpRKw5)**

After your request is reviewed and approved, we will provide the download link or access instructions by e-mail.

Please note that access may be denied, suspended, or terminated if the intended use does not comply with the dataset Terms of Use, privacy requirements, or applicable data-use restrictions.

## Terms of Use

The dataset is provided solely for **non-commercial research and academic purposes**.

Users must not:

- Use the dataset for commercial purposes without written permission
- Redistribute, sell, sublicense, publish, or transfer the dataset
- Attempt to re-identify individuals or sensitive locations
- Use the dataset for surveillance, profiling, targeted advertising, credit scoring, employment screening, insurance evaluation, or other privacy-invasive purposes
- Release derived data that can reconstruct or substitute for the original dataset

By accessing the dataset, users agree to comply with the applicable Terms of Use.

## Citation

If you use KMTC in your research, please cite:

```bibtex
@article{kim2026kmtc,
  title={KMTC: A Korean Multimodal Trip-Chain Dataset with GPS Trajectories, Voice Narratives, and Mobility QA Annotations},
  author={Kim, Hyeongbok and Kim, Sung Jin and Dong, Gilmu},
  journal={Preprint submitted to Elsevier},
  year={2026}
}
