# Crypto Hash Toolkit 🔐

![CI Pipeline](https://github.com/Mdsoare/cripto-hash-toolkit/actions/workflows/ci-pipeline.yml/badge.svg)
[![Security Rating](https://img.shields.io/badge/Security-DevSecOps%20Hardened-green?style=flat&logo=github)](https://github.com/Mdsoare/cripto-hash-toolkit/security/code-scanning)
![Security: CSP Compliant](https://img.shields.io/badge/Security-CSP--Compliant-success.svg)
![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)

<!-- Badges de Linguagens, Ecossistema e DevSecOps -->
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![NPM](https://img.shields.io/badge/NPM-CB3837?style=for-the-badge&logo=npm&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![ESLint](https://img.shields.io/badge/ESLint-4B32C3?style=for-the-badge&logo=eslint&logoColor=white)
![Dependabot](https://img.shields.io/badge/Dependabot-025E8C?style=for-the-badge&logo=dependabot&logoColor=white)
![SAST & SCA](https://img.shields.io/badge/DevSecOps-SAST%20%26%20SCA-red?style=for-the-badge&logo=shield&logoColor=white)

---

Uma aplicação web leve, moderna e segura para **geração e análise heurística de hashes criptográficos**. Desenvolvida para rodar 100% no lado do cliente (*client-side*), garantindo a privacidade dos dados processados.

---

## 🎯 Funcionalidades

- **Aba 1 — Gerador de Hashes**:
  - **Suporte Nativo**: Algoritmos seguros via Web Crypto API (`SHA-256`, `SHA-512`).
  - **Família SHA-3**: Implementação completa (`SHA3-224`, `SHA3-256`, `SHA3-384`, `SHA3-512`).
  - **Uso Forense / Legacy**: Suporte local a `SHA-1` e `MD5`.
  - **Ações Rápidas**: Botão de limpeza de campos e redefinição de estado.

- **Aba 2 — Identificador Heurístico**:
  - Análise de assinaturas de hashes hexadecimais com base no comprimento de caracteres (bits).
  - Validação estrita de entradas em formato hexadecimal.
  - Mapeamento de compatibilidade para algoritmos comuns (`MD5`, `SHA-1`, `SHA-2`, `SHA-3`, `NTLM`, `BLAKE2`, etc.).

---

## 🔒 Segurança e Privacidade

- **Privacidade Total**: Nenhum dado digitado é enviado a servidores externos. Todo o processamento ocorre localmente no navegador.
- **Politica de Segurança de Conteúdo (CSP)**:
  - Implementação de **Content Security Policy estrita** via Meta Tag.
  - Bloqueio de scripts não autorizados (`default-src 'self'`).
  - Mitigação de ataques Cross-Site Scripting (XSS) e Clickjacking.

---

## 🛠️ Tecnologias Utilizadas

- **HTML5 & CSS3**: Interface responsiva baseada em CSS Variables e Flexbox.
- **JavaScript (Vanilla ES6+)**:
  - `Web Crypto API` (`crypto.subtle.digest`) para algoritmos padrão.
  - Algoritmo `MD5` (RFC 1321) otimizado em JS puro.
- **Biblioteca Externa**:
  - [`js-sha3`](https://github.com/emn178/js-sha3) para cálculo de variantes do SHA-3/Keccak.

---

## 📂 Estrutura do Projeto

  ```text
  .
  ├── assets/
  │   ├── css/
  │   │   └── style.css       # Estilização global e componentes
  │   └── js/
  │       ├── script.js      # Lógica principal, abas e manipuladores
  │       └── sha3.js        # Módulo local para SHA-3 (js-sha3)
  ├── .gitignore             # Arquivo de configuração do git
  ├── index.html             # Interface principal da aplicação
  ├── LICENSE                # Licença do projeto
  └── README.md              # Documentação do projeto
  ```

---

## 🚀 Como Executar

Por ser uma aplicação web estática e client-side, não é necessária a instalação de dependências ou servidores Node.js.

### 1. Clone o repositório

  ```bash
  git clone https://github.com/Mdsoare/cripto-hash-toolkit.git
  ```

### 2. Acesse a pasta do projeto

  ```bash
  cd cripto-hash-toolkit
  ```

### 3. Abra o arquivo `index.html` diretamente em qualquer navegador moderno

---

## 📜 Licença

Este projeto está sob a licença [MIT](LICENSE).

---

*Desenvolvido por **Marcelo Soares** | Especialista em Segurança da Informação e Computação Forense.*
