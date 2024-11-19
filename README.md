# End-to-End Speech-to-Text Model Using Wav2Vec2 and TIMIT Corpus

This project demonstrates the implementation of an advanced **Automatic Speech Recognition (ASR)** pipeline leveraging the **Wav2Vec2 model** and the **TIMIT dataset**. The goal is to create an accurate, robust speech-to-text system evaluated through the **Word Error Rate (WER)** metric and deployable for real-world applications.

---

## 🚀 Features
- **State-of-the-art ASR**: Built on the self-supervised Wav2Vec2 model.
- **Fine-Tuned on TIMIT**: Adapted to diverse accents and dialects for improved accuracy.
- **Performance Metrics**: Evaluated using WER for reliable transcription accuracy.
- **Ready for Deployment**: Model hosted on Hugging Face for seamless integration.

---

## 📂 Project Goals
1. Develop a robust ASR pipeline using **Wav2Vec2**.
2. Fine-tune the model on the **TIMIT dataset** for accurate transcription.
3. Evaluate performance using **Word Error Rate (WER)**.
4. Deploy the ASR system for real-world usability.

---

## 📚 What is Automatic Speech Recognition (ASR)?
ASR is the technology enabling machines to convert spoken language into text. It’s widely applied in:
- **Voice assistants**
- **Real-time language translation**
- **Call center automation**
- **Assistive technologies for the hearing impaired**

---

## 🛠 Libraries and Tools Used
- [Transformers](https://huggingface.co/transformers): For Wav2Vec2 model and tokenizer.
- [Datasets](https://huggingface.co/docs/datasets): To manage and preprocess the TIMIT dataset.
- [JiWER](https://pypi.org/project/jiwer/): For calculating Word Error Rate (WER).
- [Librosa](https://librosa.org): Audio analysis and preprocessing.

---

## 🗂 Dataset: TIMIT Corpus
The **TIMIT dataset** is a benchmark in ASR systems, featuring:
- Phonetic and word-level transcriptions.
- Samples from various dialect regions.
- High-quality, standardized audio recordings.

---

## ⚙️ Workflow
### 1. **Setup**
- Check for GPU availability for efficient processing.
- Install and authenticate with Hugging Face libraries.

### 2. **Data Preprocessing**
- Load and clean TIMIT dataset transcriptions.
- Extract unique characters to build a custom vocabulary.
- Tokenize text and upload the tokenizer to Hugging Face.

### 3. **Feature Extraction**
- Normalize audio inputs with a feature extractor.
- Use a custom data collator for dynamic padding during batching.

### 4. **Model Training**
- Configure Wav2Vec2 with **CTC loss** for speech-to-text alignment.
- Fine-tune the model with tailored training parameters.

### 5. **Evaluation**
- Calculate **WER** to measure transcription accuracy.
- Compare transcriptions against the ground truth.

### 6. **Deployment**
- Upload the fine-tuned model to Hugging Face for public access.

---

## 📈 Results
- **Word Error Rate (WER):** Achieved a WER of **19.5%**, reflecting high transcription accuracy.
- **Example Transcriptions:** Model output transcriptions for selected audio samples demonstrate its effectiveness.

---

## 🛠 How to Use
1. Clone this repository:

   ```bash
   git clone https://github.com/TejalOmA/SpeechDecoder-wav2vec2.git
   ```

2. Install dependencies:

  ```bash
   pip install -r requirements.txt
   ```

3. Run the script:
   
  ```bash
   jupyter notebook SpeechDecoder-wav2vec2.ipynb
   ```
4. Run cells sequentially to preprocess data, train the model, and evaluate its performance.

---

## 🌟 Acknowledgments
-Hugging Face
-TIMIT Dataset
-The open-source ASR community.

---
