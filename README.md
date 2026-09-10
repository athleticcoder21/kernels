# Making Models Fast

**A Systems View of LLM Inference on GPUs**

This repository contains a work-in-progress book about learning inference optimization from first principles. The chapters develop the performance model, the diagrams explain what the hardware sees, and the CUDA implementations live beside the writing so every claim can eventually be measured.

The book is a standalone inference-optimization site built from the Scaling Book's [Distill/Jekyll](https://jekyllrb.com/) layout: a full-width chapter header, part navigation, and a sticky contents rail. The cloned `scaling-book/` directory remains an untouched reference.

## Read locally

```bash
bundle install
bundle exec jekyll serve
```

Open `http://127.0.0.1:4000/kernels/` and start with the GEMV chapter. The site is rendered to `_site/`.

## Current chapter

- [Making GEMV Fast](gemv.md)

## Source code

The implementations discussed in the GEMV chapter are in [`gemv/`](gemv/):

- [`naive_kernel.cu`](gemv/naive_kernel.cu)
- [`fast_kernel.cu`](gemv/fast_kernel.cu)
