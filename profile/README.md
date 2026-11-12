<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/wordmark-dark.svg">
  <img src="./assets/wordmark.svg" alt="Vilare" width="260">
</picture>

### Gestão simples para comunidades que cuidam de pessoas.

[usevilare.com.br](https://usevilare.com.br)

</div>

---

## O que é a Vilare

A **Vilare** é um SaaS B2B que organiza o dia a dia de comunidades: condomínios, associações de bairro, escolas, empreendimentos mistos e empresas com operação presencial.

Hoje essa rotina vive espalhada entre grupos de WhatsApp, planilhas e softwares legados difíceis de usar. A Vilare junta tudo em um só lugar, com duas frentes no mesmo produto:

- **Painel web** para síndicos, gestores, administradoras e equipe
- **App (PWA)** para moradores e membros, instalável e com notificações push

## O que o produto resolve

| | |
|---|---|
| 🛠️ **Ordens de serviço** | O morador abre o chamado com foto, a gestão acompanha e todos são avisados a cada mudança de status |
| 🏘️ **Estrutura** | Propriedades, unidades, áreas comuns e o vínculo de cada morador com sua unidade |
| 💰 **Financeiro** | Cobranças regulares, extras e multas, com acompanhamento de pagamentos |
| 📣 **Comunicação** | Feed de comunicados, avisos e discussões da comunidade |
| 📋 **Reuniões e documentos** | Convocação, presença, atas, regimento e convenções sempre à mão |
| 👥 **Equipe** | Funcionários, escalas e permissões por papel |

## Objetivos

1. **MVP em produção** com uma associação de bairro como primeiro cliente real, validando o fluxo principal: ordem de serviço, comunicação e cobrança.
2. **Crescer no B2B** com administradoras de condomínio, nosso mercado principal.
3. **Uma plataforma multi-tenant** que atende vários tipos de comunidade sem virar um produto diferente para cada uma.
4. **Experiência simples de verdade**: densa onde precisa (tabelas de OS e de cobrança), leve onde importa (o morador no celular).

## Stack

**Backend**

![Java](https://img.shields.io/badge/Java_25-1F5E5B?style=flat-square&logo=openjdk&logoColor=FBF9F5)
![Spring Boot](https://img.shields.io/badge/Spring_Boot_4-1F5E5B?style=flat-square&logo=springboot&logoColor=FBF9F5)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL_16-1F5E5B?style=flat-square&logo=postgresql&logoColor=FBF9F5)
![Flyway](https://img.shields.io/badge/Flyway-1F5E5B?style=flat-square&logo=flyway&logoColor=FBF9F5)
![Maven](https://img.shields.io/badge/Maven-1F5E5B?style=flat-square&logo=apachemaven&logoColor=FBF9F5)

- Spring Web MVC com virtual threads
- Arquitetura em camadas, um módulo Maven por camada (application, usecase, domain, repository…)
- Spring Data JPA e migrations em SQL puro com Flyway
- Auth com JWT (Spring Security) e refresh token
- Contrato da API em OpenAPI, com client TypeScript gerado para o front
- Testes com JUnit 5, AssertJ, Mockito e Testcontainers

**Frontend**

![Next.js](https://img.shields.io/badge/Next.js-14110D?style=flat-square&logo=nextdotjs&logoColor=FBF9F5)
![React](https://img.shields.io/badge/React-14110D?style=flat-square&logo=react&logoColor=FBF9F5)
![TypeScript](https://img.shields.io/badge/TypeScript-14110D?style=flat-square&logo=typescript&logoColor=FBF9F5)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-14110D?style=flat-square&logo=tailwindcss&logoColor=FBF9F5)

- Next.js (App Router) como PWA: painel admin e app do morador no mesmo projeto
- Design system próprio: tons terrosos, um acento teal e tipografia Manrope / JetBrains Mono

**Infra e serviços**

![Docker](https://img.shields.io/badge/Docker-6A6354?style=flat-square&logo=docker&logoColor=FBF9F5)
![Vercel](https://img.shields.io/badge/Vercel-6A6354?style=flat-square&logo=vercel&logoColor=FBF9F5)
![Resend](https://img.shields.io/badge/Resend-6A6354?style=flat-square&logo=resend&logoColor=FBF9F5)

## Como trabalhamos

- **Decisões registradas** em ADRs: o porquê fica escrito, não só o quê
- **Contrato primeiro**: a API é documentada em OpenAPI e o front consome o client gerado
- **Testes de integração com banco real** (Testcontainers), sem mock de Postgres
- **Simplicidade antes de abstração**: começamos pelo que o MVP precisa

## Quer construir com a gente?

Estamos no começo, e quem chega agora ajuda a definir o produto e a engenharia.
Se você é dev e se interessou, ou se quer conversar sobre investimento, fale com a gente pelo site **[usevilare.com.br](https://usevilare.com.br)**.

<div align="center">
<br>
<sub>Feito com cuidado no Brasil 🇧🇷</sub>
</div>
