# Olá, eu sou o Daniel Pereira (`AxionDev`) 👋

**Desenvolvedor de Software Júnior | Análise e Desenvolvimento de Sistemas (74% concluído — UniCesumar)**  
📍 Congonhas, MG — Disponível para atuação **100% Remota**  
📫 Contato Dev: `axiondev0@gmail.com` | Contato Pessoal: `dnpereirajunior2@gmail.com`

---

## Sobre Mim e Metodologia de Trabalho

Desenvolvedor de software em fase final da graduação em **Análise e Desenvolvimento de Sistemas (UniCesumar)**, com foco em **Programação Orientada a Objetos (Java, Dart, TypeScript)**, **Arquitetura em Camadas (`Controller / Service / Repository / Model`)**, **Bancos de Dados Relacionais (`SQL`, `PostgreSQL`, `JPA`, `Drizzle ORM`)** e **Sistemas de Catálogo, Busca e Gestão**.

Adoto práticas modernas de **Engenharia de Software Assistida por IA (*AI-Augmented Development / Pair Programming*)** fundamentadas em uma diretriz inegociável: **auditoria técnica linha a linha**. Utilizo ferramentas de IA para acelerar a escrita de *boilerplate*, mas toda decisão arquitetural, modelagem de banco de dados, indexação, tratamento de exceções e regra de segurança passa por validação e compreensão integral do funcionamento interno.

---

## Projetos em Destaque & Cases de Arquitetura

> **Nota de Governança e Segurança:** Projetos comerciais desenvolvidos para clientes ou em fase de homologação possuem seus repositórios de produção mantidos como **privados** por responsabilidade com propriedade intelectual, LGPD e segurança de credenciais. Abaixo estão documentadas suas arquiteturas e o repositório **público** de referência técnica.

### 1. 🟢 [Público] [Catalog & Search API — Java 21 + Spring Boot 3 + PostgreSQL + Redis](https://github.com/axion-dev0/catalog-search-api-java)
API RESTful construída especificamente para demonstrar arquitetura de **Catálogo e Busca de Alta Performance** no ecossistema Java/Spring:
- **Stack:** Java 21, Spring Boot 3, Spring Data JPA (`JpaSpecificationExecutor`), PostgreSQL 16, Redis 7, Docker Compose.
- **Destaques Técnicos:**
  - Busca textual e filtros combinados dinâmicos (`category`, `brand`, `minPrice`, `maxPrice`, `onlyInStock`) com paginação e ordenação via `Specification`.
  - Índices compostos no PostgreSQL para otimização de leitura.
  - Cache distribuído no **Redis** (`@Cacheable` / `@CacheEvict`) com TTL configurável e invalidação automática na escrita.

---

### 2. 🔒 [Case Mobile — Google Play Console] **Cidadão Informado** *(Em Teste Fechado na Google Play Store)*
Aplicativo móvel voltado à democratização do acesso a direitos constitucionais e jurisprudência traduzida para linguagem acessível.
- **Stack:** Dart, Flutter, Cloud Firestore, Provider, Material 3.
- **Arquitetura & Funcionalidades:**
  - Estrutura desacoplada em **Models** (`DireitoModel`, `TemaModel`) e **Repositories** (`DireitoRepository`, `TemaRepository`).
  - **Motor de Catálogo Categorizado e Busca Textual Instantânea:** Filtragem reativa por temas (Saúde, Educação, Assistência Social, Serviços Públicos, Trabalho), título, problema comum e descrição.
  - Publicado em **Teste Fechado oficial no Google Play Console** (conta de desenvolvedor verificada, pacote `.aab` assinado e ciclo ativo de 12 testadores simultâneos).

---

### 3. 🔒 [Case Full-Stack SQL/ORM] **Soberania Country — Plataforma de E-commerce** *(Repositório Privado)*
E-commerce completo com painel administrativo, gestão de estoque e motor de catálogo e busca de produtos.
- **Stack:** TypeScript, Next.js 16 (App Router), **SQL (Cloudflare D1)**, **Drizzle ORM**, Cloudflare R2 (Object Storage), NextAuth (Google OAuth + RBAC), Mercado Pago SDK (PIX e Cartão).
- **Arquitetura & Funcionalidades:**
  - Modelagem de banco de dados **relacional (SQL)** mapeada via **ORM**, com controle transacional de estoque e pedidos.
  - **Catálogo e Busca de Produtos** com filtragem por categorias, variantes e paginação.
  - Segurança em profundidade (validação de schemas com `Zod`, proteção de rotas administrativas e webhooks autenticados).

---

### 4. 🔒 [Case Multiplataforma Cloud] **Hardware House — Gestão de Ordem de Serviço e Catálogo de Setup** *(Repositório Privado)*
Sistema multiplataforma (Web, Android e Windows) para gestão de assistência técnica, ordens de serviço e catálogo de componentes de hardware.
- **Stack:** Dart, Flutter, Firebase Auth, Cloud Firestore (`Security Rules` + `Composite Indexes`), Cloud Functions (`Node.js`), Riverpod, GoRouter, geração de PDF e leitura de QR Code.
- **Arquitetura & Funcionalidades:**
  - Controle de acesso baseado em papéis (Admin / Cliente) com guarda de rotas reativa no `GoRouter`.
  - **Busca e filtragem em tempo real** de Ordens de Serviço (`OS-YYYYMMDD-XXXX`) e clientes, suportada por índices compostos no banco de dados.
  - Otimização de estado compartilhado via `Riverpod` e regras estritas de segurança no banco (`firestore.rules`).

---

## Tecnologias e Ferramentas

- **Linguagens:** Java, SQL, Dart, TypeScript, Python
- **Backend & Persistência:** Spring Boot, Spring Data JPA, PostgreSQL, Redis, Drizzle ORM, Cloud Firestore, Node.js (Cloud Functions)
- **Frontend & Mobile:** Flutter (Android/Web/Windows), Next.js / React
- **DevOps & Ferramentas:** Git, GitHub CLI (`gh`), Docker Compose, Cloudflare Wrangler, Firebase CLI, Google Play Console
