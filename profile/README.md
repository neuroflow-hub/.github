# Neuroflow Labs

Welcome to the Neuroflow Labs monorepo! This organization encompasses the core products and experiences that make up the Neuroflow ecosystem—a high-performance visual IDE for building and training machine learning models from first principles.

## Ecosystem Repositories

This organization is divided into three primary projects to ensure modularity and separation of concerns:

### 1. [neuroflow-client](./neuroflow-client)
The frontend user interface and Electron desktop wrapper for the visual node editor.
- **Stack**: React, Vite, TypeScript, TailwindCSS, Shadcn UI, React Flow.
- **Role**: Provides the Drag-and-Drop canvas where users design their ML workflows, configure nodes, and visualize results in real-time.

### 2. [neuroflow-logic](./neuroflow-logic)
The computational backend API that powers the data processing and machine learning models.
- **Stack**: Python, Flask, NumPy.
- **Role**: Implements algorithms from scratch (White-Box Machine Learning) and handles the heavy mathematical lifting behind the scenes without relying on opaque ML black-box libraries.

### 3. [neuroflow-folks](./neuroflow-folks)
The sleek, minimalistic landing/marketing page for the Neuroflow application.
- **Stack**: Svelte, Vite, TailwindCSS.
- **Role**: Designed with an ultra-clean "Zen Interface" aesthetic (Catppuccin Light/Pastel theme) to showcase the application's capabilities and provide download links.

<br>

## Key Features

- **White-Box Machine Learning**: Algorithms implemented from scratch using pure mathematics for maximum transparency.
- **Visual Workflow Editor**: Design complex data flows visually, linking nodes like neurons.
- **Real-time Evaluation**: Visualize model performance metrics and dendrograms instantly.
- **Aesthetic First**: A native desktop experience built for speed and designed with a minimal, Notion-like UI.

## Getting Started Locally

Each repository has its own isolated development environment.

**Start the Logic Engine (Backend)**:
```bash
cd neuroflow-logic
uv sync && uv run app.py
```

**Start the Client (Desktop IDE)**:
```bash
cd neuroflow-client
npm install
npm run dev:electron
```

**Start the Landing Page (Web)**:
```bash
cd neuroflow-folks
npm install
npm run dev
```

<br>

## Contributing & Licensing

We welcome contributions! Please refer to the specific `README.md` files located in each respective microservice directory for detailed contribution guidelines.

This project is licensed under the MIT License.
