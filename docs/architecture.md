# Arquitetura do Projeto: Portal da Aldeia (Justes)

## 1. Stack Tecnológica Core
- **Framework:** Next.js 15 (App Router)
- **CMS/Backend:** Payload CMS 3.0 (Rodando nativamente no Next.js)
- **Base de Dados:** PostgreSQL via Neon.tech (Serverless)
- **ORM:** Drizzle (Default do Payload 3.0)
- **Storage de Imagens:** Vercel Blob (Para fotos de produtos, notícias e galeria)
- **Deployment:** Vercel

## 2. Modelagem de Dados (Payload Collections)

### Globals (Conteúdo Único)
- **Configuração do Site:** Nome da aldeia, slogan, contactos, links de redes sociais.
- **Página de História:** Conteúdo RichText (Markdown), Timeline de eventos, Galeria principal.

### Collections (Conteúdo Repetível)
- **Notícias:** Título, Slug (automático), Conteúdo, Imagem de Capa, Data de Publicação.
- **Produtos:** Nome, Descrição, Preço (Decimal), Stock (Número), Fotos (Upload direto para Vercel Blob).
- **Pontos de Interesse:** Nome, Descrição, Localização (Texto para Google Maps), Galeria de Fotos.
- **Analytics:** Timestamp, PagePath (Para o contador de visitas interno).
- **Media:** Coleção centralizada para uploads (configurada com Vercel Blob adapter).

## 3. Segurança e Auditoria
- **Autenticação:** Sistema nativo do Payload para acesso ao `/admin`.
- **Versioning:** Todas as coleções e globals devem ter `versions: { drafts: true }` para histórico de alterações e recuperação de dados.

## 4. Padrões de Desenvolvimento
- **Frontend:** React Server Components (RSC) sempre que possível para performance.
- **Componentes UI:** Tailwind CSS + ShadcnUI para um look limpo e moderno.
- **Commits:** Seguir o padrão Conventional Commits (`feat:`, `fix:`, `docs:`, `style:`).