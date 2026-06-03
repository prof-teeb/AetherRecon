# AetherRecon

AetherRecon is a modern reconnaissance automation platform designed to simplify the information gathering phase of security assessments and bug bounty workflows. The project combines multiple reconnaissance tools into a centralized pipeline, providing subdomain discovery, live host detection, and scan management through an intuitive web interface.

## Features

- Automated reconnaissance pipeline
- Subdomain enumeration
- Live host detection
- FastAPI-powered backend
- Modern Next.js frontend
- Docker support for easy deployment
- Modular architecture for integrating additional security tools

## Tech Stack

### Frontend
- Next.js
- React
- TypeScript
- Tailwind CSS
- Radix UI

### Backend
- FastAPI
- Python

### Infrastructure
- Docker
- Docker Compose

---

## Project Structure

```bash
AetherRecon/
│
├── Frontend/          # Next.js frontend
├── backend/           # FastAPI backend
├── data/              # Scan outputs and temporary files
├── infra/             # Infrastructure configurations
└── docker-compose.yml
```

---

## Installation

### Clone Repository

```bash
git clone https://github.com/prof-teeb/AetherRecon.git
cd AetherRecon
```

### Run with Docker

```bash
docker-compose up --build
```

---

## Backend Setup

```bash
cd backend

pip install -r requirements.txt

uvicorn main:app --reload
```

---

## Frontend Setup

```bash
cd Frontend

npm install

npm run dev
```

---

## API Endpoints

### Full Recon Scan

```http
GET /api/scan?target=example.com
```

### Single Tool Scan

```http
GET /api/scan/{tool_id}?target=example.com
```

---

## Workflow

1. Target domain is provided.
2. Subdomain enumeration is performed.
3. Results are consolidated and filtered.
4. Live hosts are identified.
5. Findings are returned through the API and dashboard.

---

## Future Enhancements

- DNS Enumeration
- Port Scanning
- Screenshot Collection
- Vulnerability Detection
- Reporting Dashboard
- Historical Scan Tracking

---

## Security Notice

This project is intended for authorized security testing, educational purposes, and research activities only. Users are responsible for complying with applicable laws and regulations.

---

## Project Members

- **Shahjahan**
- **Muteeb**

---

## License

This project is released for educational and research purposes.

---

### Built with ❤️ by Shahjahan & Muteeb
