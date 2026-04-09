# OCR Cloud Worker

![Python](https://img.shields.io/badge/Python-3.9+-blue)
![Cloud](https://img.shields.io/badge/Cloud-Worker-orange)
![License](https://img.shields.io/badge/License-MIT-green)

A cloud-native OCR worker service that extracts text from images and scanned documents at scale. Designed as a distributed worker that processes OCR jobs from a queue, making it suitable for high-throughput document digitization pipelines.

---

## Features

- **Text Extraction** -- Accurate OCR processing for printed and handwritten text
- **Document Layout Analysis** -- Preserves document structure including tables and columns
- **Queue-Based Processing** -- Consumes jobs from message queues for horizontal scaling
- **Multi-Format Input** -- Processes PDF, PNG, JPEG, TIFF, and BMP files
- **Language Detection** -- Automatically detects and processes text in multiple languages
- **Structured Output** -- Returns extracted text with bounding boxes and confidence scores

---

## Tech Stack

| Technology | Purpose |
|---|---|
| Python 3.9+ | Core runtime |
| Tesseract / OCR Engine | Text recognition |
| Cloud Queue Service | Job distribution |
| CSS3 | Dashboard theming |
| Makefile | Build and test automation |

---

## Quick Start

```bash
# Clone the repository
git clone https://github.com/razinahmed/ocr-cloud-worker.git
cd ocr-cloud-worker

# Install dependencies
pip install -r requirements.txt

# Start the worker
python main.py --queue ocr-jobs
```

---

## Project Structure

```
ocr-cloud-worker/
├── styles/
│   └── theme.css           # Dashboard theme configuration
├── Makefile                # Build and test commands
├── LICENSE                 # MIT License
├── SECURITY.md             # Security policy
└── README.md
```

---

## Usage

```bash
# Build the project
make build

# Run tests
make test
```

---

## Contributing

1. Fork the repository
2. Create a feature branch -- `git checkout -b feature/your-feature`
3. Commit your changes -- `git commit -m "feat: add new feature"`
4. Push and open a Pull Request

---

## License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

**Built by [Razin Ahmed](https://github.com/razinahmed)**
