# Olá, eu sou o Daniel Pereira (`AxionDev`) 👋

**Desenvolvedor de Software Júnior (Full-Stack & Backend) | Análise e Desenvolvimento de Sistemas (74% concluído — UniCesumar)**  
📍 Congonhas, MG — Disponível para atuação **100% Remota**  
📫 Contato Dev: `axiondev0@gmail.com` | Contato Pessoal: `dnpereirajunior2@gmail.com`

---

## Sobre Mim e Metodologia de Trabalho

Desenvolvedor de software em fase final da graduação em **Análise e Desenvolvimento de Sistemas (UniCesumar)**, com foco prático em **Programação Orientada a Objetos e Funcional**, **Arquitetura em Camadas (`Controller / Service / Repository / Model`)**, **Desenvolvimento Web & Mobile (`React / Next.js / TypeScript / Flutter`)**, **Back-end (`Java / Spring Boot`, `Python / FastAPI`, `Node.js`)** e **Bancos de Dados Relacionais e NoSQL (`SQL`, `PostgreSQL`, `JPA`, `Drizzle ORM`, `Redis`, `Firestore`)**.

Adoto práticas modernas de **Engenharia de Software Assistida por IA (*AI-Augmented Development / Pair Programming*)** fundamentadas em uma diretriz inegociável: **auditoria técnica linha a linha**. Utilizo ferramentas de IA para acelerar a escrita de *boilerplate*, mas toda decisão arquitetural, modelagem de banco de dados, indexação, testes automatizados e regra de segurança passa por validação e compreensão integral do funcionamento interno.

---

## Projetos em Destaque & Cases de Arquitetura

> **Nota de Governança e Segurança:** Projetos comerciais desenvolvidos para clientes ou em fase de homologação possuem seus repositórios de produção mantidos como **privados** por responsabilidade com propriedade intelectual, LGPD e segurança de credenciais. Abaixo estão documentadas suas arquiteturas e o repositório **público** de referência técnica.

### 1. 🟢 [Público] [Catalog, Search & Purchase Order API — Java 21 + Spring Boot 3 + PostgreSQL + Redis + JUnit 5](https://github.com/axion-dev0/catalog-search-api-java)
API RESTful construída para demonstrar arquitetura de **Catálogo, Busca Otimizada e Gestão de Pedidos de Compra** no ecossistema Java/Spring:
- **Stack:** Java 21, Spring Boot 3, Spring Data JPA (`JpaSpecificationExecutor`), PostgreSQL 16, Redis 7, Spring Scheduling (Jobs), JUnit 5 & Mockito, Docker Compose.
- **Destaques Técnicos:**
  - Busca textual e filtros combinados dinâmicos (`category`, `brand`, `minPrice`, `maxPrice`, `onlyInStock`) com paginação e ordenação via `Specification`.
  - Gestão transacional de **Pedidos de Compra (`PurchaseOrder`)** com reserva atômica de estoque e **Job agendado (`@Scheduled`)** para expiração automática de pedidos pendentes.
  - Cache distribuído no **Redis** (`@Cacheable` / `@CacheEvict`) e **Testes Unitários (`JUnit 5` + `Mockito`)**.

---

### 2. 🔒 [Case Full-Stack React/TS/SQL] **Soberania Country — Plataforma de E-commerce & Gestão** *(Repositório Privado)*
E-commerce completo com painel administrativo, gestão de pedidos/estoque e motor de catálogo e busca de produtos.
- **Stack:** TypeScript, React 19, Next.js 16 (App Router), **SQL Relacional (Cloudflare D1)**, **Drizzle ORM**, Cloudflare R2 (Object Storage), NextAuth (OAuth + RBAC), Mercado Pago SDK (PIX e Cartão), Zod, Tailwind CSS.
- **Arquitetura & Funcionalidades:**
  - Modelagem de banco de dados **relacional (SQL)** mapeada via **ORM**, com controle transacional de estoque e pedidos.
  - **Catálogo e Busca de Produtos** com filtragem por categorias, variantes e paginação.
  - Segurança em profundidade (validação de schemas com `Zod`, proteção de rotas administrativas e webhooks autenticados).

---

### 3. 🔒 [Case Mobile — Google Play Console] **Cidadão Informado — Direitos e Serviços Públicos** *(Em Teste Fechado na Google Play Store)*
Aplicativo móvel voltado à democratização do acesso a direitos constitucionais, serviços públicos e jurisprudência traduzida para linguagem acessível.
- **Stack:** Dart, Flutter, Cloud Firestore, Provider, Material 3.
- **Arquitetura & Funcionalidades:**
  - Estrutura desacoplada em **Models** (`DireitoModel`, `TemaModel`) e **Repositories** (`DireitoRepository`, `TemaRepository`).
  - **Motor de Catálogo Categorizado e Busca Textual Instantânea:** Filtragem reativa por temas (Saúde, Educação, Assistência Social, Serviços Públicos, Trabalho).
  - Publicado em **Teste Fechado oficial no Google Play Console** (conta de desenvolvedor verificada, pacote `.aab` assinado e ciclo ativo de 12 testadores simultâneos).

---

### 4. 🔒 [Case Multiplataforma Cloud] **Hardware House — Gestão de Ordem de Serviço e Catálogo de Setup** *(Repositório Privado)*
Sistema multiplataforma (Web, Android e Windows) para gestão de assistência técnica, ordens de serviço e catálogo de componentes de hardware.
- **Stack:** Dart, Flutter, Firebase Auth, Cloud Firestore (`Security Rules` + `Composite Indexes`), Cloud Functions (`Node.js`), Riverpod, GoRouter, geração de PDF e leitura de QR Code.
- **Arquitetura & Funcionalidades:**
  - Controle de acesso baseado em papéis (Admin / Cliente) com guarda de rotas reativa no `GoRouter`.
  - **Busca e filtragem em tempo real** de Ordens de Serviço (`OS-YYYYMMDD-XXXX`) e clientes, suportada por índices compostos no banco de dados.

---

### 5. 🔒 [Cases Python Back-end, Automação & Testes] **Robô de Protocolo Jurídico (FastAPI) & WhatsApp AI Bot (Pytest)** *(Repositórios Privados)*
Soluções em **Python** voltadas para automação de processos, integração de APIs e atendimento inteligente:
- **Robô de Protocolo Jurídico (API REST & RPA):** Orquestrador em **Python + FastAPI (`Uvicorn`) + Playwright** para validação de PDFs, automação em portais judiciais (PJe, e-SAJ, Eproc) e notificações via webhook/API.
- **WhatsApp AI Bot:** Serviço de integração com WhatsApp e LLMs em Python estruturado de forma modular (`ai.py`, `whatsapp.py`, `config.py`, `logger.py`) com suíte de **testes unitários automatizados em `pytest`** (`test_ai.py`, `test_whatsapp.py`, `test_config.py`).

---

## Tecnologias e Ferramentas

- **Linguagens:** Java, TypeScript, JavaScript, Python, SQL, Dart, HTML5, CSS3
- **Front-end & Mobile:** React, Next.js, Tailwind CSS, Flutter (Android/Web/Windows)
- **Back-end, ORM & Persistência:** Spring Boot, Spring Data JPA, Node.js, FastAPI (Python), PostgreSQL, Redis, Drizzle ORM, Cloud Firestore
- **Qualidade, DevOps & Cloud:** JUnit 5, Mockito, Pytest, Git, GitHub CLI (`gh`), Docker Compose, Cloudflare (D1/R2/Wrangler), Firebase, Google Play Console
