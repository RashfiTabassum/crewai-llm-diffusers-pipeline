# Multi-Agent Instagram Content Pipeline

A multi-agent AI system that automates the creation of Instagram-ready content, including research, caption writing, review, and image generation.

---

## Overview

This project demonstrates an end-to-end **agentic AI system** that integrates **LLMs and diffusion models** to produce complete Instagram posts.  
The pipeline automates research, caption generation, semantic prompt compression, and high-quality visual generation.

---

## What the System Does

- Accepts a user-provided topic  
- Researches key facts, trends, and insights  
- Generates short and long Instagram captions with hashtags and CTA  
- Reviews and edits content for clarity, grammar, tone, and engagement  
- Compresses image prompts semantically to CLIP-safe token limits (≤77 tokens)  
- Produces 2–3 high-quality images per topic using a text-to-image API  

---

## Agents

| Agent | Responsibility |
|-------|----------------|
| Research Agent | Gathers key points and insights about the topic |
| Content Writer Agent | Creates engaging Instagram captions (short + long) |
| Reviewer Agent | Edits and approves content for quality and engagement |
| Image Prompt Generator Agent | Produces detailed prompts for image generation |

---

## Technical Requirements

- Define and orchestrate agents using **CrewAI**  
- Each agent must have:  
  - Role definition (e.g., Researcher, Writer, Reviewer, Designer)  
  - Goal (specific output)  
  - Tools/models they can access  
- Integrate at least one **external text-to-image API** (e.g., Stable Diffusion, Nano Banana, Segmind)  
- Deliver a complete Instagram post package:  
  - Short + long caption text  
  - Final reviewed hashtags  
  - 2–3 generated images  

---

## Tech Stack

- Python  
- CrewAI  
- LangChain / ChatOpenAI  
- Stable Diffusion / Diffusers / Nano Banana / Segmind  
- PyTorch  
- tiktoken  

---

## Key Features

- Multi-agent task decomposition  
- LLM-based semantic prompt compression  
- CLIP-safe image prompts  
- GPU-optimized image generation  
- Modular and extensible design  
