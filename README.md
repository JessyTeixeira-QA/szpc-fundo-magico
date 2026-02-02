# 🪄 Gerador de Background Mágico

[![n8n](https://img.shields.io/badge/Automated%20by-n8n-FF6D5A?style=for-the-badge&logo=n8n)](https://n8n.io/)
[![JS](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=for-the-badge&logo=javascript)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![CSS3](https://img.shields.io/badge/CSS3-Animated-1572B6?style=for-the-badge&logo=css3)](https://developer.mozilla.org/en-US/docs/Web/CSS)

Transforme descrições textuais em backgrounds animados.
Este projeto utiliza **n8n** e **IA** para criar e injetar estilos dinamicamente.

---

## 📋 Sobre o Projeto

Aplicação interativa que une **Front-end** e **Automação**.
O usuário descreve um cenário (ex: *"espaço sideral"*) e a IA gera o código **HTML/CSS**, que é aplicado instantaneamente ao fundo do site.

---

## 🚀 Funcionalidades

- **Prompt-to-Style:** IA gera animações baseadas em texto
- **Preview em tempo real:** Injeção dinâmica de CSS no DOM
- **Visualização de código:** HTML e CSS disponíveis para cópia
- **Responsivo:** Interface adaptada para mobile e desktop

---

## 🛠️ Tecnologias

- **Frontend:** HTML5, CSS3, JavaScript (Vanilla)
- **Integração:** Fetch API
- **Backend / Automação:** [n8n](https://n8n.io/) + Google Gemini AI

---

## ⚙️ Configuração (n8n)

O workflow consiste em:

1. **Webhook** – Recebe o prompt do usuário
2. **AI Agent** – Gera um JSON contendo `html` e `css`
3. **Code Node** – Limpa a resposta (remove markdown e caracteres extras)
4. **Respond to Webhook** – Retorna os dados ao frontend

---

## 📂 Estrutura do Projeto

```text
├── src/
│   ├── css/          # estilos, reset e responsivo
│   ├── js/           # index.js (lógica da API)
├── index.html        # página principal
└── README.md         # documentação

---

## 🔧 Como Executar

Siga os passos abaixo para rodar o projeto localmente:

---

### 1️⃣ Clone o repositório

```bash
git clone https://github.com/seu-usuario/fundo-magico.git

---

2️⃣ Configure o Webhook do n8n

No arquivo src/js/index.js, ajuste a URL do Webhook:

const URL = "http://localhost:5678/webhook-test/fundo-magico";

---


3️⃣ Execute o projeto

Abra o arquivo index.html utilizando a extensão Live Server no VS Code.

---

👨‍💻 Autor

Desenvolvido por Jessica Ferreira Teixeira
Projeto criado durante a Semana do Zero ao Programador Contratado

---

💡 Dica Extra

Caso o VS Code apresente erro com acentuação ou caracteres especiais, verifique se o arquivo está salvo com a codificação UTF-8.

---


### ✅ Por que essa versão é ideal
- ✔️ Texto explicativo **fora** de blocos de código
- ✔️ Apenas comandos e código **dentro** dos blocos
- ✔️ Leitura clara para humanos e robôs (GitHub / ATS)
- ✔️ Padrão usado em projetos profissionais e portfólios QA/Dev

Se quiser, eu posso:
- Ajustar o README para **nível empresa**
- Adaptar para **portfólio QA**
- Criar a **descrição perfeita do repositório**
- Revisar como se fosse um **tech lead**

Só dizer o próximo passo 🚀
