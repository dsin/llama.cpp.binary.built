## llama.cpp Binary Release
version: 0.5.0-dev (build 1, commit 4da6337)
https://github.com/ggml-org/llama.cpp/releases/tag/b11223

## Built
built with GNU 13.3.0 for Linux x86_64 (Ubuntu 24.04.5 LTS (Noble Numbat))
* CPU only ( W/O GPU )

## Usage
```
apt-get install -y git

git clone https://github.com/dsin/llama.cpp.binary.built.git
```

## Download AI Model 
Download AI Model 

## Test
```
MODEL=$(find /path-to/your-ai-model -name "*whatever-ai-model*.whatever-ai-model-extension" | head -1)

echo "Using model: $MODEL"

/path-to/llama.cpp.binary.built/bin/llama-embedding \
    -m "$MODEL" \
    -p "น้ำปลาร้า" \
    --pooling last \
    -ngl 99
```
