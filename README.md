# Pretraining a GPT Model from Scratch

Training a GPT model from scratch on an extremely small sample of the [fineweb](https://huggingface.co/datasets/nampdn-ai/mini-fineweb) dataset. The implementation is inspired from [Karpathy’s nanoGPT](https://github.com/karpathy/nanoGPT) project. The goal is to gain some intuition on the inner workings of LLMs. The model is called SmolGPT since it only contains 20M parameters.

## Training hyperparameters

```
architecture: "gpt2"
batch_size: 64
bias: false
block_size: 128
dropout :0.2
eval_interval: 500
eval_iters: 200
learning_rate: 0.0003
max_iter: 20,000
n_embd: 192
n_head: 6
n_layer: 6
vocab_size: 50,257
weight_init: "xavier_uniform_"
```

## Training results

![alt text](.\assets\train_loss_curve.png)
