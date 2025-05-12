# 📘 Plano de Gerenciamento de Configuração – TTF DIET

## 📅 Histórico de Modificações

| Data       | Versão | Descrição                            | Autor                |
|------------|--------|--------------------------------------|----------------------|
| 06/05/2025 | 1.0    | Criação do plano de configuração     | Felipe Sousa Gomes   |

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
 - Commits colaborativos devem usar --author ou -s:
 - git commit -m "Refactor planner engine" --author="Tiago Marques <tiago@email.com>"
ou
 - git commit -s -m "Fix nutritional calculator rounding bug"
### 4.2 - Política de Branches
- A main (ou master) conterá apenas versões estáveis.

- A branch devel conterá o código de desenvolvimento.

- Nenhum commit direto será feito nas branches main ou devel.

- Novas branches devem ser criadas a partir da devel.

### 4.3 - Padrões para Criação e Uso de Branches
Seguindo o modelo GitFlow, utilize os seguintes padrões:

### 4.3.1 - Casos de Uso
- Prefixo: UC_

- Formato: UC_RegisterUser

### 4.3.2 - Histórias de Usuário
- Prefixo: US_

- Formato: US_CalculateMacros

### 4.3.3 - Correções e Configurações
- Prefixo: FIX_

- Formato: FIX_FixLoginBug

### 4.3.4 - Issues
- Prefixo: ISSUE_XX_

- Formato: ISSUE_08_FixConnectionWithDatabase

### 4.4 - Política de Aprovação
- Pull requests devem ser revisados por outro membro da equipe.

- A aprovação requer:

- Build "passing" no Travis CI.

- Análise positiva nas ferramentas de qualidade.

- Conformidade com o plano de testes e estilo de código.

### 4.5 - Versionamento de Código
- Adota-se o Semantic Versioning 2.0.0:

MAJOR.MINOR.PATCH
MAJOR: alterações incompatíveis.

MINOR: novas funcionalidades compatíveis.

PATCH: correções de bugs compatíveis.

### 5 - Repositório de Documentação
- A documentação será mantida na pasta /docs ou em um repositório dedicado.
- Estrutura sugerida:

docs/
├── plano_gerenciamento_configuracao.md
├── requisitos/
│   ├── requisitos_funcionais.md
│   └── requisitos_nao_funcionais.md
├── diagramas/
│   └── arquitetura.drawio
└── atas/
    └── ata_reuniao_2025-04-10.md
    
### 5.1 - Versionamento de Documentos
- Versão no formato MAJOR.MINOR.
- Exemplo:

- Correção leve → incrementa MINOR

- Adição/modificação relevante → incrementa MAJOR

### 6 - Monitoramento e Controle
- A equipe de gerenciamento é responsável por:

- Garantir conformidade com este plano.

- Orientar contribuintes quanto ao uso correto do repositório.

- Avaliar pull requests e padrões de qualidade.

- Remover ou ajustar conteúdo fora dos padrões.

### 7 - Referências
- PMI. Um guia do conhecimento em gerenciamento de projetos – PMBOK®, 5ª ed., 2013.

- Semantic Versioning 2.0.0

- Plano de Configuração - Plataforma Jogos UnB
