# Mimicking AI

## Project Team
- **Ali AKKOYUN**
- **Alaaeddin KHEİTİ**
- **Hüseyin ELİBOL**
- **Esat Yusuf DALBUDAK**

## Supervisor
- **Dr. Öğr. Üyesi Kadriye Filiz BALBAL**

## Objective
The goal of this project is to generate poetry that mimics a selected poet's style using artificial intelligence and natural language processing.

## Goals
1. Process and classify texts written by humans to create new works in the same style.
2. Achieve high accuracy in mimicking the selected poet's thought process.

## Analysis
- **Model Selection**: RNN was not suitable due to high data requirements and context inadequacies. GPT-2 was considered but discarded due to lack of Turkish support and high training costs.
- **Final Model**: Fine-tuned GPT-3.5 model using transformer architecture for good performance with less data.

## Methodology
1. **Data Preparation**:
    - Collected a dataset of 1273 poems.
    - Removed very short poems to ensure the model doesn't generate too short poems.
    - Balanced the data by poets and ensured the poems' format was preserved.
2. **Model Training**:
    - Fine-tuned GPT-3.5 TURBO model with 4 epochs.
    - Developed a classification model using Turkish BERT with 61 epochs, achieving 88% accuracy.
3. **Evaluation**:
    - Extracted a sample of 99 poems to measure mimicking performance.
    - Developed a website using Java Spring and React JS, storing outputs in PostgreSQL.
4. **User Interaction**:
    - Users can select a poet, propose a poem title, choose a theme, and generate a poem.

## Results
- **Mimicking Performance**: Average of 62%, with up to 80-85% for well-represented poets.
- **Comparison with Original GPT Model**: The fine-tuned model performed significantly better in mimicking.

## References
- Sawicki, P., Grzes, M., Góes, L. F., Brown, D., Peeperkorn, M., Khatun, A., & Paraskevopoulou, S. (2023).
- Kurt, U., & Çayir, A. (2023). "A Modern Turkish Poet: Fine-Tuned GPT-2."
- OpenAI. "Documentation for GPT Finetuning Service"
- Dbmdz repo Turkish BERT model huggingface
- GitHub Repository: [Fine-tuning GPT-3 for Poetry Generation and Evaluation](https://github.com/PeterS111/Fine-tuning-GPT-3-for-Poetry-Generation-and-Evaluation/tree/main/Code)
- Data Sources: www.antoloji.com, siir.sitesi.web.tr, buyuksiirbelediyesi.com

## Project Flowchart
![Project Flowchart](path/to/flowchart.png)

## System Architecture
![System Architecture](path/to/system_architecture.png)

## User Interface
![Data Collection and Preparation](path/to/data_collection.png)
