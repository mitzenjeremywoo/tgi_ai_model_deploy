# Use the official Hugging Face TGI image
FROM ghcr.io/huggingface/text-generation-inference:latest

# Let the container accept an env var for the model ID
ENV MODEL_ID=tiiuae/falcon-40b-instruct

# Override the default entrypoint with a small script
ENTRYPOINT ["bash", "-c"]
CMD ["text-generation-launcher --model-id $MODEL_ID"]
