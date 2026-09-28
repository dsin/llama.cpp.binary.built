## llama.cpp Binary Release
version: 0.5.0-dev (build 1, commit 4da6337)
https://github.com/ggml-org/llama.cpp/releases/tag/b11223

## Built (on Google Colab)
built with GNU 13.3.0 for Linux x86_64
* Linux: Ubuntu 24.04.5 LTS (Noble Numbat)
* CPU only ( W/O GPU )

## Usage
```
apt-get install -y git
git clone https://github.com/dsin/llama.cpp.binary.built.git
```

## Download Model 
Download Model (e.g. Qwen3-Embedding-0.6B-Q8_0.gguf) and put into /content/Qwen3-Embedding-0.6B-GGUF

## Test
```
! MODEL=$(find /content/Qwen3-Embedding-0.6B-GGUF -name "*Q8_0*.gguf" | head -1)

! echo "Using model: $MODEL"

! /content/llama.cpp.binary.built/bin/llama-embedding \
    -m "$MODEL" \
    -p "ทดสอบจย้า" \
    --pooling last \
    -ngl 99
```
