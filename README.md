# 📘 Plano de Gerenciamento de Configuração – TTF DIET

## 📅 Histórico de Modificações

| Data       | Versão | Descrição                            | Autor                |
|------------|--------|--------------------------------------|----------------------|
| 12/05/2025 | 1.0    | Criação do plano de configuração     | Felipe Sousa Gomes   |

---

## 📑 Sumário

1. [Introdução](#1---introdução)  
2. [Itens de configuração](#2---itens-de-configuração)  
3. [Ferramentas](#3---ferramentas)  
4. [Repositório de código](#4---repositório-de-código)  
   - [Política de Commits](#41---política-de-commits)  
   - [Política de Branches](#42---política-de-branches)  
   - [Padrões para criação e uso das branches](#43---padrões-para-criação-e-uso-das-branches)  
   - [Política de aprovação](#44---política-de-aprovação)  
   - [Versionamento de código](#45---versionamento-de-código)  
5. [Repositório de documentação](#5---repositório-de-documentação)  
   - [Versionamento de documentos](#51---versionamento-de-documentos)  
6. [Monitoramento e controle](#6---monitoramento-e-controle)  
7. [Referências](#7---referências)  

---

## 1 - Introdução

Este documento tem como objetivo orientar os integrantes e colaboradores do projeto **TTF DIET** quanto às práticas de configuração, versionamento, contribuição e organização dos artefatos do projeto, como código-fonte e documentação. O objetivo é garantir consistência, rastreabilidade e controle das mudanças ao longo do desenvolvimento.

---

## 2 - Itens de configuração

- **Código-fonte:** Scripts, APIs, interfaces e lógica de negócio.  
- **Documentação:** Planejamento, atas, escopo, requisitos, e manuais.  
- **Ambientes de configuração:** Arquivos Docker, .env e scripts de build.

---

## 3 - Ferramentas

| Ferramenta | Uso |
|-----------|-----|
| Git       | Controle de versão e histórico de alterações |
| GitHub    | Repositório de código, issues e pull requests |
| Docker    | Containerização de aplicações e ambientes |
| CI/CD (GitHub Actions) | Integração e entrega contínua |
| Code Climate (opcional) | Análise de qualidade do código |

---

## 4 - Repositório de código

### 4.1 - Política de Commits

- Idioma: **Inglês**  
- Padrão: Mensagens claras, objetivas e iniciadas com verbo no infinitivo.  
- Exemplo:  
  ```bash
  git commit -m "Create user login screen"
