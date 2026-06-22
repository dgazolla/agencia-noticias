# Portal IA — Agência de Notícias da Indústria

Protótipos interativos com IA para o portal da CNI.

## Arquivos

| Arquivo | Descrição |
|---|---|
| `index.html` | Landing page com links para os protótipos |
| `Portal IA.dc.html` | Homepage com chat RAG, busca semântica e resumo executivo |
| `Materia IA.dc.html` | Página de matéria com sumário e conexões por IA |
| `POC Busca Semântica.dc.html` | Documento técnico da POC de RAG |
| `support.js` | Runtime dos Design Components |
| `vercel.json` | Configuração de deploy para Vercel |

## Deploy no Vercel

Este projeto é um site estático — basta conectar o repositório no Vercel.

1. Acesse [vercel.com/new](https://vercel.com/new)
2. Importe este repositório GitHub
3. Framework Preset: **Other** (static)
4. Root Directory: `/` (raiz)
5. Clique em **Deploy**

A cada push na branch `main`, o Vercel faz redeploy automático.

## Stack da POC (backend RAG)

- **Embeddings:** OpenAI `text-embedding-3-small`
- **Banco vetorial:** Supabase + pgvector
- **LLM:** Claude 3 Haiku (Anthropic)
- **API:** Python FastAPI no Railway/Vercel
