# Prashant Saini

**Lead LLMOps Engineer at [Zeblok Computational](https://www.zeblok.com)** · AI/LLM infrastructure · Kubernetes & GPU platforms

I build and run the infrastructure that serves large language models in production — from H100/A100 GPU clusters to edge nodes on ships and fully air-gapped on-prem sites. 6+ years across DevOps, MLOps and LLMOps.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-princeprashantsaini-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/princeprashantsaini/)
[![Email](https://img.shields.io/badge/Email-princeprashantsaini%40gmail.com-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:princeprashantsaini@gmail.com)

## What I work on

- **LLM serving in production.** 16 Kubernetes clusters (~150 nodes, 40 NVIDIA GPUs: H100/A100 with NVLink, RTX 6000 Blackwell Pro) serving Llama 70B, Qwen 72B and a 4B vision-language model to 400–600 concurrent users, ~1M tokens a day, on vLLM, llama.cpp and Ollama.
- **Inference internals.** A custom vLLM connector that offloads KV cache and model weights to NVMe SSD and CPU RAM. Multi-node serving that pairs tensor parallelism inside a node with pipeline parallelism across nodes, so 70B+ models run on commodity PCIe GPUs without NVLink.
- **Cloud-to-edge AI.** KubeEdge hubs managing edge nodes at universities and aboard ships, plus fully air-gapped, on-premises installations on a zero-trust architecture.
- **Platform and security.** A custom API gateway with API-key auth and Istio routing for multi-tenant inference endpoints; MCP servers and LLM agents for automated infrastructure root-cause analysis.
- **Fine-tuning and RAG.** LoRA, QLoRA and full fine-tuning on the GPU fleet; Ray-based document ingestion into ChromaDB that cut processing time 6× (90 → 15 min per 4 MB document).

## Tech stack

| Area | Tools |
| --- | --- |
| LLM inference | vLLM · llama.cpp · Ollama · Hugging Face · tensor & pipeline parallelism · KV-cache offloading |
| LLM apps & fine-tuning | LangChain · LlamaIndex · RAG · MCP · ChromaDB · LoRA / QLoRA · Ray · MLflow |
| Kubernetes & GPUs | Kubernetes (EKS, AKS, k3s) · KubeEdge · Helm · Istio · NVIDIA GPU Operator · DCGM |
| Cloud & IaC | AWS · Azure · Terraform · Ansible |
| CI/CD & observability | Docker · GitHub Actions · Jenkins · Prometheus · Grafana |
| Languages & OS | Python · Bash · SQL · Linux |

## Experience

**Zeblok Computational** · Ai-MicroCloud®, a cloud-to-edge AI PaaS · *Oct 2021 – present*
- Lead LLMOps Engineer · *Apr 2023 – present* · leading a 7-member platform team
- Lead DevOps Engineer · *Oct 2021 – Apr 2023*

**RedCarpet Tech** · DevOps Engineer · *Oct 2020 – Oct 2021*
- AWS and k3s infrastructure for a Y Combinator-backed payments and lending platform (~400K daily users, ~50K transactions a day)

---

<sub>Most of my day-to-day work is in private company repositories, so the public projects here are mostly earlier DevOps work.</sub>
