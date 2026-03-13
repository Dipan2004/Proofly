# Proofly 

Proofly is a proof-of-existence application that allows users to create and verify cryptographic proofs for digital content such as text, images, and documents.

The system is designed to be privacy-first: original user content is never stored. Instead, Proofly generates a deterministic cryptographic hash, assigns a unique proof ID, and records a trusted timestamp. Anyone can later verify the proof using the proof ID along with the original content or hash.

## What Proofly Does

- Creates cryptographic proof of existence for digital content
- Generates a unique proof ID, SHA-256 hash, and timestamp
- Allows verification days or months later using the same proof ID
- Does not store original content
- Works without blockchain or wallets
- Designed to support text, images, documents, and OCR-based proofs

## Current Features 

- Text proof creation (live)
- Proof verification by text or hash (live)
- Proof metadata retrieval (read-only)
- Image and document proof flows (UI ready, backend supported)
- OCR and AI-assisted extraction.

## How Verification Works

1. A proof is created from content, generating a hash and proof ID.
2. The original content is discarded.
3. To verify later, the user provides:
   - Proof ID
   - Original content or hash
4. The backend recomputes the hash and validates it against the stored proof.

## Live Demo

https://asyh5b3gr2jxvju818bj.share.dreamflow.app/

## Tech Stack

- Flutter for frontend
- FastAPI backend
- SHA-256 cryptographic hashing
- Supabase storage
- OCR (Tesseract)
- AI sidecar (Gemini)

## Project Status

Proofly is an active prototype built for demonstration and evaluation purposes. The system architecture supports future expansion without storing user data or weakening cryptographic guarantees.
