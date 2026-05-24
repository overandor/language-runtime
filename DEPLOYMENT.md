# Deployment Guide

## Prerequisites

- Python 3.11+
- Node.js 18+ (for JavaScript components)
- Rust stable (for Rust components)

## Local Development

```bash
# Python
pip install -r requirements.txt
python -m language_runtime.main

# JavaScript
npm install
npm start

# Rust
cargo build --release
cargo run
```

## Docker Deployment

```bash
docker build -t language-runtime .
docker run -p 8000:8000 language-runtime
```

## Kubernetes

```bash
kubectl apply -f k8s/
```
