# Mini GPT

A miniature autoregressive GPT-style model implemented with Keras. It trains on the IMDB movie-review dataset and generates text from a prompt using top-k sampling.

## Requirements

Install Keras with the JAX backend, TensorFlow for the input pipeline, and NumPy:

```bash
python -m pip install keras jax tensorflow numpy
```

The script downloads and extracts IMDB using `curl` and `tar`; make sure both commands are available on your system. A GPU is recommended, but CPU execution is possible and will be slower.

## Run

```bash
python mini_gpt.py
```

Training runs for 25 epochs and may take a while. Adjust the epoch count or model settings in the script as needed.
