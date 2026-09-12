# How to make your models fast

A slowly growing collection of CUDA kernel worklogs for understanding inference
performance from first principles. The focus is currently narrow: write one
kernel, count its work and memory traffic, inspect what the GPU actually does,
and improve one bottleneck at a time.

## Read locally

```bash
quarto preview
```

Quarto renders the complete book into `_book/`.

## Current chapters

- [Making GEMV Fast](chapters/making-gemv-fast.qmd)
- [Making Softmax Fast](chapters/optimizing-softmax.qmd)

## CUDA implementations

- [GEMV kernels](kernels/gemv/)
- [Softmax kernels](kernels/softmax/)
