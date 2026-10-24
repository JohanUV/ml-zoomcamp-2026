# Homework 5 - Deploying ML Models

## Q1 - uv version
uv 0.13.5

## Q2 - Scikit-Learn version
1.7.2 (declarado en `pyproject.toml` y `uv.lock`)

## Q3 - Modelo cargado con pickle
Script: `q3.py`, ejecutado con `uv run python q3.py`
Resultado: 0.533

## Q4 - API con FastAPI
    uv run uvicorn predict:app --host 0.0.0.0 --port 9696
    uv run python q6_test.py
Resultado: 0.770

## Q5 - Imagen base del Dockerfile
python:3.11.15-slim-bookworm

## Q6 - Contenedor Docker
    docker build -t zoomcamp-model:2026-hw5 .
    docker run --rm -p 9696:9696 zoomcamp-model:2026-hw5
    python3 q6_test.py
Resultado: 0.770
