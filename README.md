# RAG-contabilitate – MVP

## Scop
Construim un MVP RAG (Retrieval-Augmented Generation) care răspunde la întrebări de contabilitate
folosind Codul Fiscal, norme și proceduri interne (10 PDF-uri).

## Stack
| Strat | Tehnologie |
|-------|------------|
| Server | Hetzner CX22 / Ubuntu 22.04 |
| Containere | Docker, docker-compose |
| OCR & extract | Tesseract-OCR, pdfplumber |
| Ingest & RAG | LangChain, OpenAI embeddings (text-embedding-ada-002) |
| Vector DB | Qdrant (Docker) |
| API & UI | Next.js 14 + Clerk (auth) |
| Cache | SQLite |
| Backup | rsync + MinIO (local bucket) |

## Cost-target
| Componentă | Cost lunar estimat |
|------------|--------------------|
| VPS Hetzner CX22 | **3,92 €** |
| Trafic 20 TB | inclus |
| Stocare backup 20 GB | ~2 € |
| OpenAI API | < 1 € |
| **Total** | **≤ 30 €/lună** |

