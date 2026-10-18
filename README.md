# Twi-to-English Neural Machine Translation Engine (`Twi-English-Translator`)

A custom sequence-to-sequence (Seq2Seq) neural machine translation model built from first principles using **Python**, **PyTorch**, and parallel text corpora sourced from the [Hugging Face GhanaNLP Community Dataset](https://huggingface.co/datasets/ghananlpcommunity/pristine-twi-english-parallel-sentences). Designed for low-resource African language NLP tasks and featured in portfolio evaluations for AI startup accelerator programs.

## Project Architecture
- **Encoder & Decoder:** Custom PyTorch `nn.Module` classes utilizing Gated Recurrent Units (`nn.GRU`) and word embedding layers.
- **Preprocessing:** Custom tokenizers handling word-level mappings with special control tokens (`<PAD>`, `<UNK>`, `<BOS>`, `<EOS>`) and sequence padding (`MAX_LEN = 10`).
- **Training Engineering:** Integrated PyTorch DataLoaders, Adam optimizer, Cross-Entropy Loss with padding masking (`ignore_index=0`), and gradient clipping (`torch.nn.utils.clip_grad_norm_`) to ensure training stability.
- **Inference:** Autoregressive token-by-token generation supporting interactive CLI/notebook translation.

## Repository Structure
- `twi_english_translator.ipynb`: Step-by-step interactive Jupyter notebook.
- `twi_english_sample.csv`: Cleaned parallel text dataset subset.
- `twi_english_translator_weights.pth`: Pre-trained model weights.

## Getting Started
Clone the repository and run the notebook or script to load weights instantly without retraining:
```bash
git clone [https://github.com/Tidjani-Adeniran/Twi-English-Translator.git](https://github.com/Tidjani-Adeniran/Twi-English-Translator.git)
cd Twi-English-Translator# Twi-to-English Neural Machine Translation Engine (`Twi-English-Translator`)

A custom sequence-to-sequence (Seq2Seq) neural machine translation model built from first principles using **Python**, **PyTorch**, and parallel text corpora sourced from the [Hugging Face GhanaNLP Community Dataset](https://huggingface.co/datasets/ghananlpcommunity/pristine-twi-english-parallel-sentences). Designed for low-resource African language NLP tasks and featured in portfolio evaluations for AI startup accelerator programs.

## Project Architecture
- **Encoder & Decoder:** Custom PyTorch `nn.Module` classes utilizing Gated Recurrent Units (`nn.GRU`) and word embedding layers.
- **Preprocessing:** Custom tokenizers handling word-level mappings with special control tokens (`<PAD>`, `<UNK>`, `<BOS>`, `<EOS>`) and sequence padding (`MAX_LEN = 10`).
- **Training Engineering:** Integrated PyTorch DataLoaders, Adam optimizer, Cross-Entropy Loss with padding masking (`ignore_index=0`), and gradient clipping (`torch.nn.utils.clip_grad_norm_`) to ensure training stability.
- **Inference:** Autoregressive token-by-token generation supporting interactive CLI/notebook translation.

## Repository Structure
- `twi_english_translator.ipynb`: Step-by-step interactive Jupyter notebook.
- `twi_english_sample.csv`: Cleaned parallel text dataset subset.
- `twi_english_translator_weights.pth`: Pre-trained model weights.

## Getting Started
Clone the repository and run the notebook or script to load weights instantly without retraining:
```bash
git clone [https://github.com/Tidjani-Adeniran/Twi-English-Translator.git](https://github.com/Tidjani-Adeniran/Twi-English-Translator.git)
cd Twi-English-Translator