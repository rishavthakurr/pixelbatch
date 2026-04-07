# PIXELBATCH | Image Processor

PixelBatch is a high-performance, hardware-grade image processing suite. It features a modern React-based web interface for interactive batch processing and a multi-threaded Python CLI script for industrial-scale automation.

## 🚀 Features

- **Web Interface:** Interactive queue management, live image monitor with transformation analytics, and ZIP exports.
- **CLI Script:** Multi-threaded Python script using Pillow for maximum performance on large datasets.
- **Smart Resizing:** Maintains aspect ratio while fitting within target dimensions.
- **Multiple Formats:** Supports JPEG, PNG, WebP, GIF, ICON, BMP, and TIFF.
- **Hardware Aesthetic:** Clean, industrial-themed UI with system logs and configuration exports.

---

## 💻 Web Application Setup

The web application is built with **React 19**, **Vite**, and **Tailwind CSS**.

### Prerequisites
- [Node.js](https://nodejs.org/) (v18.0 or higher)
- npm (comes with Node.js)

### Installation
1. Navigate to the project root directory:
   ```bash
   cd pixelbatch
   ```
2. Install the required dependencies:
   ```bash
   npm install
   ```

### Running Locally
1. Start the development server:
   ```bash
   npm run dev
   ```
2. Open your browser and navigate to `http://localhost:3000`.

---

## 🐍 Python CLI Script Setup

The CLI version is designed for power users who need to process thousands of images efficiently.

### Prerequisites
- [Python 3.8+](https://www.python.org/)
- pip (Python package manager)

### Installation
1. Navigate to the `cli` directory:
   ```bash
   cd cli
   ```
2. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```

### Usage
Run the script with the `--help` flag to see all available options:
```bash
python processor.py --help
```

**Common Example:**
Process all images in a folder, resize to 1080p, and convert to WebP:
```bash
python processor.py --input ./raw_images --output ./processed --width 1920 --height 1080 --format WEBP
```

---

## 📂 Project Structure

- `src/`: React source code and components.
- `cli/`: Python CLI script and requirements.
- `public/`: Static assets.
- `package.json`: Web app dependencies and scripts.
- `metadata.json`: Application metadata.

## 🛠 Tech Stack

- **Frontend:** React, Tailwind CSS, Motion, Lucide Icons.
- **Processing (Web):** Canvas API, JSZip.
- **Processing (CLI):** Python, Pillow (PIL), Concurrent Futures.

---

## 📄 License

This project is provided for professional image processing workflows. Refer to the project settings for specific licensing details.
