# Neuroflow Labs

Welcome to the Neuroflow Labs! This organization encompasses the core products and experiences that make up the Neuroflow ecosystem — a simple, visual IDE for building and training machine learning models from first principles.

To download and play around with the application, download it from: https://neuroflow-ebon.vercel.app/

## Ecosystem Repositories

This organization is divided into two primary projects to ensure modularity and separation of concerns:

### 1. [neuroflow-client](./neuroflow-client)
The frontend user interface and Electron desktop wrapper for the visual node editor.
- **Stack**: React, Vite, TypeScript, TailwindCSS, Shadcn UI, React Flow.
- **Role**: Provides the Drag-and-Drop canvas where users design their ML workflows, configure nodes, and visualize results in real-time.

### 2. [neuroflow-logic](./neuroflow-logic)
The computational backend API that powers the data processing and machine learning models.
- **Stack**: Python, Flask, NumPy.
- **Role**: Implements algorithms from scratch (White-Box Machine Learning) and handles the heavy mathematical lifting behind the scenes without relying on opaque ML black-box libraries.

<br>

## Key Features

- **White-Box Machine Learning**: Algorithms implemented from scratch for maximum transparency.
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

<br>

## Contributing & Licensing

We welcome contributions! Please refer to the specific `README.md` files located in each respective microservice directory for detailed contribution guidelines.

This project is licensed under the MIT License.
