# LLaMA.go

Part of this code is borrowed from [llama.go](github.com/gotzmann/llama.go)


## How to Run

First, obtain and convert original LLaMA models on your own, or just download ready-to-rock ones:

LLaMA-7B: [llama-7b-fp32.bin](https://nogpu.com/llama-7b-fp32.bin)

This model stores FP32 weights, so you'll needs at least 32Gb of RAM (not VRAM or GPU RAM) for LLaMA-7B.

Please make sure that the LLaMA model is saved in path `mlgo/examples/llama/models/llama-7b-fp32.bin`

```shell
go build
./llama --threads 8 --model ./models/llama-7b-fp32.bin --temp 0.80 --context 128 --predict 128 --prompt "How to combine AI and blockchain?"
```

