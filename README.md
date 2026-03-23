# Hi, I'm Roni Sutrisno 👋

## 🛠️ Projects | Proyek

### ProxsisLLM | Secure and Entrprise Ready Private LLM Solution
### Copyright 2026 by Roni Sutrisno and Proxsis AI*

> **Default app language / Bahasa default aplikasi:** Bahasa Indonesia

Enterprise-ready LLM Solution Application. FastAPI + React → Open WebUI API → LLM. PostgreSQL, PgBouncer, Docker.

---

## English

### Chat & Conversation
| Feature | Description |
|---------|-------------|
| **Chat streaming** | Real-time token-by-token; multi-model via Admin. ProxsisLLM → Open WebUI API → LLM (filters run in Open WebUI). |
| **RAG** | Upload doc/image/audio as context; drag-drop or paste URL. Integrates with Open WebUI RAG (pgvector) and external data feed. |
| **Fetch URL** | Paste URL → extract webpage text (BeautifulSoup), inject into chat. |
| **Auto title** | Chat title auto-generated (LLM or keyword fallback). |
| **Streaming task queue** | Save/complete/cancel for long streams; avoid timeout. |

### Documents & OCR
| Feature | Description |
|---------|-------------|
| **Document processing** | PDF, DOCX, PPTX, XLSX, TXT, images, audio. OCR for scanned PDFs (Tesseract/Mistral). |
| **OCR Tool** | PDF → searchable PDF async (Tesseract/ocrmypdf); poll job_id. |
| **Repair PDF** | PDF repair via QPDF & Ghostscript. |
| **Audio transcription** | Transcribe via Whisper API (MP3, WAV, M4A, OGG); config from Admin. |

### Memory
| Feature | Description |
|---------|-------------|
| **User memory** | Profile + Facts stored in PostgreSQL; auto-selected per query (Jaccard + trigram). |
| **Memory API** | Markdown table, context by query, save profile/facts, clear all, delete facts only, delete by index. |

### Chat Management
| Feature | Description |
|---------|-------------|
| **Pin chat** | Pin chats in sidebar for quick access. |
| **Share chat** | Public read-only link; recipients can save to history if logged in. |
| **History** | Lazy load messages per chat; rename, delete, metadata-only list. |

### User & Auth
| Feature | Description |
|---------|-------------|
| **User management** | bcrypt, session, admin/user roles; CRUD users, change/reset password, revoke admin. |
| **Role-based models** | Admin creates roles, assigns models to roles, assigns roles to users (local + LDAP). |
| **LDAP** | Enterprise login; configure/test/search users/migrate to local via Admin. |
| **Pending registration** | Approve/reject/batch for pending signups. |
| **OTP email** | Send/verify OTP; test SMTP config. |
| **Online users** | List online users; heartbeat. |

### System & Admin
| Feature | Description |
|---------|-------------|
| **System config** | Context window, allowed models, system prompt, CORS, API keys, smart title model. |
| **Models** | Fetch from Open WebUI; per-model context window; save to DB. |
| **DB optimization** | Auto VACUUM; manual VACUUM/REINDEX/sync index via Admin. |
| **PgVector** | Rebuild/reset/reindex embedding index; embedding status. |

### Open WebUI Integration
| Feature | Description |
|---------|-------------|
| **RAG** | Open WebUI pgvector + Ollama embedding; ProxsisLLM injects doc context. |
| **Web Search** | News/website queries via Ollama web search and News RSS. |
| **Function Calling** | Open WebUI filters for tool invocation. |
| **External data feed** | Connect to external APIs (e.g. law/regulation), inject context into chat. |

---

## Bahasa Indonesia

### Chat & Percakapan
| Fitur | Keterangan |
|-------|------------|
| **Chat streaming** | Respons real-time token per token; multi-model via Admin. ProxsisLLM → Open WebUI API → LLM (filter berjalan di Open WebUI). |
| **RAG** | Unggah dokumen/gambar/audio sebagai konteks; drag-drop atau paste URL. Terintegrasi dengan RAG Open WebUI (pgvector) dan external data feed. |
| **Fetch URL** | Paste URL → ekstraksi teks webpage (BeautifulSoup), inject ke chat. |
| **Auto title** | Judul chat di-generate otomatis (LLM atau fallback kata kunci). |
| **Streaming task queue** | Save/complete/cancel untuk streaming panjang; hindari timeout. |

### Dokumen & OCR
| Fitur | Keterangan |
|-------|------------|
| **Document processing** | PDF, DOCX, PPTX, XLSX, TXT, gambar, audio. OCR untuk PDF scan (Tesseract/Mistral). |
| **OCR Tool** | PDF → searchable PDF async (Tesseract/ocrmypdf); poll job_id. |
| **Repair PDF** | Perbaikan PDF via QPDF & Ghostscript. |
| **Audio transcription** | Transkripsi via Whisper API (MP3, WAV, M4A, OGG); konfigurasi dari Admin. |

### Memory
| Fitur | Keterangan |
|-------|------------|
| **User memory** | Profil + Fakta tersimpan di PostgreSQL; otomatis terpilih per query (Jaccard + trigram). |
| **Memory API** | Tabel Markdown, context by query, save profil/fakta, clear all, hapus fakta saja, hapus by index. |

### Chat Management
| Fitur | Keterangan |
|-------|------------|
| **Pin chat** | Pin chat di sidebar untuk akses cepat. |
| **Share chat** | Link publik read-only; penerima bisa simpan ke history jika login. |
| **History** | Lazy load messages per chat; rename, delete, metadata-only list. |

### User & Auth
| Fitur | Keterangan |
|-------|------------|
| **User management** | bcrypt, session, role admin/user; CRUD user, ubah password, reset password, revoke admin. |
| **Role-based models** | Admin buat role, assign model ke role, assign role ke user (lokal + LDAP). |
| **LDAP** | Login enterprise; konfigurasi/test/search user/migrasi ke lokal via Admin. |
| **Pending registration** | Approve/reject/batch untuk pendaftaran tertunda. |
| **OTP email** | Kirim/verifikasi OTP; test konfigurasi SMTP. |
| **Online users** | Daftar user online; heartbeat. |

### System & Admin
| Fitur | Keterangan |
|-------|------------|
| **System config** | Context window, model allowed, system prompt, CORS, API keys (Open WebUI/Mistral/Whisper), smart title model. |
| **Models** | Fetch dari Open WebUI; context window per model; simpan ke DB. |
| **DB optimization** | Auto VACUUM; manual VACUUM/REINDEX/sync index via Admin. |
| **PgVector** | Rebuild/reset/reindex embedding index; status embedding. |

### Integrasi Open WebUI
| Feature | Description |
|---------|-------------|
| **RAG** | Open WebUI pgvector + Ollama embedding; ProxsisLLM injects doc context. |
| **Web Search** | News/website queries via Ollama web search and News RSS. |
| **Function Calling** | Open WebUI filters for tool invocation. |
| **External data feed** | Connect to external APIs (e.g. law/regulation), inject context into chat. |

---

**Tech:** `FastAPI` `React` `PostgreSQL` `PgBouncer` `Docker` `Open WebUI API`

*Repository private. Hubungi saya / Contact me for more info.*

---

## 📫 Contact

- Email: roni.sutrisno@gmail.com, roni.sutrisno@proxsisgroup.com
- GitHub: [@ronisutrisno](https://github.com/ronisutrisno)
