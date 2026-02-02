# 🪄 Fundo Mágico - Gerador de Backgrounds com IA

<p align="center">
  <img src="src/images/bg.JPG" alt="Fundo Mágico" width="100%">
</p>

[![n8n](https://img.shields.io/badge/Automated%20by-n8n-FF6D5A?style=for-the-badge&logo=n8n)](https://n8n.io/)
[![JS](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=for-the-badge&logo=javascript)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![CSS3](https://img.shields.io/badge/CSS3-Animated-1572B6?style=for-the-badge&logo=css3)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)

O **Fundo Mágico** é uma aplicação interativa que utiliza Inteligência Artificial para transformar descrições textuais em backgrounds animados e estilizados em tempo real. O projeto une o poder do desenvolvimento **Front-end** com a flexibilidade da automação via **n8n**.

---

## 📋 Sobre o Projeto

Este projeto foi desenvolvido durante a **Semana do Zero ao Programador Contratado (SZPC)**. A ideia central é permitir que o usuário descreva um cenário ou estilo (ex: *"um gradiente espacial com estrelas cadentes"*) e a IA gere automaticamente o código HTML e CSS necessário para criar esse efeito visual, aplicando-o instantaneamente ao fundo da página.

---

## 🚀 Funcionalidades

- **Prompt-to-Style:** Geração de animações e estilos baseados em descrições naturais.
- **Preview em Tempo Real:** Injeção dinâmica de CSS no DOM para visualização imediata.
- **Exibição de Código:** Mostra o código HTML e CSS gerado pela IA para que possa ser copiado e usado em outros projetos.
- **Design Responsivo:** Interface adaptada para diferentes tamanhos de tela (Mobile e Desktop).

---

## 🛠️ Tecnologias Utilizadas

- **Frontend:**
  - HTML5
  - CSS3 (Variáveis, Flexbox, Animações)
  - JavaScript Vanilla (ES6+)
- **Integração & Backend:**
  - [n8n](https://n8n.io/) (Plataforma de automação low-code)
  - Google Gemini AI (Modelo de linguagem para geração de código)
  - Fetch API para comunicação assíncrona

---

## 📂 Estrutura de Pastas

```text
├── src/
│   ├── css/          # Arquivos de estilização (reset, estilos globais e responsividade)
│   ├── images/       # Ativos visuais e imagens de fundo
│   ├── js/           # Lógica da aplicação e integração com a API
├── index.html        # Estrutura principal da página
└── README.md         # Documentação do projeto
```

---

## ⚙️ Configuração do Workflow (n8n)

Para que o projeto funcione, é necessário um workflow no n8n configurado da seguinte forma:

1. **Webhook Node:** Recebe o prompt do usuário via método POST.
2. **AI Agent / Google Gemini:** Processa o texto e gera um objeto JSON contendo as chaves `html` e `css`.
3. **Code Node:** Limpa a resposta da IA, garantindo que apenas o código puro seja retornado (removendo blocos de markdown).
4. **Respond to Webhook:** Retorna os dados processados para o frontend.

---

## 🔧 Como Executar

### 1. Clone o Repositório
```bash
git clone https://github.com/JessyTeixeira-QA/szpc-fundo-magico.git
```

### 2. Configure a URL da API
No arquivo `src/js/index.js`, localize a constante de URL e substitua pelo seu endpoint do n8n:
```javascript
const resposta = await fetch("SUA_URL_DO_WEBHOOK_AQUI", { ... });
```

### 3. Rode o Projeto
Você pode abrir o arquivo `index.html` diretamente no navegador ou utilizar a extensão **Live Server** no VS Code para uma melhor experiência de desenvolvimento.

---

## 👨‍💻 Autor

Desenvolvido por **Jessica Ferreira Teixeira**.
Projeto criado com foco em aprendizado de integração de APIs e manipulação dinâmica de DOM.

---

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes (se disponível).

---

<p align="center">Feito com 💜 por Jessica Ferreira Teixeira</p>
