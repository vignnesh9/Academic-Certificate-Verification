# Academic Certificate Verification - Demo

This is a simple demo project for academic certificate verification using a lightweight blockchain and ECDSA digital signatures.

## Features
- Minimal in-memory blockchain (PoW, low difficulty for demo)
- Certificate issuance: upload a certificate, compute SHA-256 hash, sign with issuer private key, store tx on chain
- Verification: upload certificate or paste hash, check chain and verify signature

## Run locally
1. Create a virtual environment (recommended)
   ```bash
   python -m venv venv
   source venv/bin/activate  # or venv\Scripts\activate on Windows
   pip install -r requirements.txt
   ```
2. Run the Flask app
   ```bash
   python app.py
   ```
3. Visit http://localhost:5000

## Tests

Run tests with pytest:
```bash
pytest -q
```

## Notes
- This project is a demo for coursework. Do NOT use in production without fixing key-management, persistence, security, and network design.
