# 🪄 Magic Background: AI-Driven Dynamic Styling Engine

<p align="center">
  <img src="src/images/bg.JPG" alt="Magic Background Banner" width="100%" style="border-radius: 10px;">
</p>

<p align="center">
  <a href="https://n8n.io/"><img src="https://img.shields.io/badge/Backend-n8n-FF6D5A?style=for-the-badge&logo=n8n" alt="n8n"></a>
  <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript"><img src="https://img.shields.io/badge/Frontend-JavaScript_ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JS"></a>
  <a href="https://ai.google.dev/"><img src="https://img.shields.io/badge/AI-Google_Gemini-4285F4?style=for-the-badge&logo=google-gemini&logoColor=white" alt="Gemini"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License"></a>
</p>

---

## 🚀 Overview

**Magic Background** is a sophisticated proof-of-concept demonstrating the seamless integration of **Generative AI** with modern **Web Technologies**. By leveraging a low-code automation backend (n8n) and advanced LLMs (Google Gemini), this application translates natural language prompts into production-ready CSS animations and HTML structures, injected dynamically into the DOM.

This project showcases a robust **Event-Driven Architecture** where the frontend acts as a thin client, delegating complex logic and creative generation to a scalable cloud-based workflow.

---

## 🏗️ Architecture & Workflow

The system follows a decoupled architecture, ensuring separation of concerns between the presentation layer and the logic engine.

### System Flow:
1.  **Client Layer:** A responsive Vanilla JS interface captures user intent via a specialized prompt engine.
2.  **Transport Layer:** Asynchronous communication via `Fetch API` transmits payload to a secure Webhook endpoint.
3.  **Logic Engine (n8n):**
    *   **Validation:** Incoming data is sanitized.
    *   **Inference:** Google Gemini AI processes the prompt to generate context-aware CSS/HTML.
    *   **Post-Processing:** A JavaScript node cleanses the AI output, removing markdown artifacts and ensuring valid syntax.
4.  **Injection Layer:** The client receives the JSON payload and performs a live DOM update, mounting the new styles without page refresh.

---

## 🛠️ Technical Stack

### Frontend
*   **HTML5 & CSS3:** Semantic structure with advanced CSS features (Custom Properties, Keyframe Animations, Flexbox).
*   **JavaScript (ES6+):** Modular logic, async/await patterns, and dynamic DOM manipulation.
*   **Responsive Design:** Mobile-first approach using media queries for cross-device compatibility.

### Backend & Automation
*   **n8n:** Orchestration of the API workflow.
*   **Google Gemini AI:** Large Language Model utilized for code generation.
*   **REST API:** Webhook-based integration.

---

## 📂 Project Structure

```bash
.
├── src/
│   ├── css/
│   │   ├── estilos.css      # Core application styling
│   │   ├── reset.css        # CSS normalization
│   │   └── responsivo.css   # Breakpoints and mobile optimization
│   ├── images/
│   │   └── bg.JPG           # Default fallback assets
│   └── js/
│       └── index.js         # API integration and DOM logic
├── index.html               # Main entry point
├── LICENSE                  # MIT License
└── README.md                # Technical documentation
```

---

## 🔧 Installation & Setup

### Prerequisites
*   A local or cloud instance of **n8n**.
*   An API Key for **Google Gemini AI**.

### Local Development
1.  **Clone the repository:**
    ```bash
    git clone https://github.com/JessyTeixeira-QA/szpc-fundo-magico.git
    cd szpc-fundo-magico
    ```
2.  **Configure Environment:**
    Open `src/js/index.js` and update the `fetch` URL with your active n8n Webhook:
    ```javascript
    const API_URL = "https://your-n8n-instance.com/webhook/fundo-magico";
    ```
3.  **Launch:**
    Serve the project using a local server (e.g., VS Code Live Server) to avoid CORS issues during development.

---

## 🤝 Contributing

Contributions are welcome! If you'd like to improve the prompt engineering, UI/UX, or backend logic:
1.  Fork the Project.
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`).
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`).
4.  Push to the Branch (`git push origin feature/AmazingFeature`).
5.  Open a Pull Request.

---

## 👨‍💻 Author

**Jessica Ferreira Teixeira**
*   [GitHub](https://github.com/JessyTeixeira-QA)
*   *Project developed during the SZPC Intensive Program.*

---

## 📄 License

Distributed under the **MIT License**. See `LICENSE` for more information.

<p align="center">
  Developed with precision and 💜
</p>
