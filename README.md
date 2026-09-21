# ⚡ PULSO AIOps — Camada de Inteligência em Resposta Real

> **FIAP × Locaweb — Enterprise Challenge | Sprint 4 (Solução Final)**  
> *Camada de AIOps Serverless para Ingestão, Filtragem de Ruído, Predição de SLA e Proteção dos KPIs Operacionais.*

---

## 📌 Sumário
- [Visão Geral](#-visão-geral)
- [Integrantes da Equipe Fluxo](#-integrantes-da-equipe-fluxo)
- [Arquitetura da Solução](#-arquitetura-da-solução)
- [Recursos do Azure em Produção](#-recursos-do-azure-em-produção)
- [Modelos de Machine Learning & Métricas](#-modelos-de-machine-learning--métricas)
- [Dashboard & Links da Solução](#-dashboard--links-da-solução)
- [Estrutura do Repositório](#-estrutura-do-repositório)
- [Como Executar a Solução](#-como-executar-a-solução)
- [Próximos Passos & Evolução](#-próximos-passos--evolução)

---

## 🌌 Visão Geral

O **PULSO** é uma solução de AIOps *serverless* e orientada a eventos construída no Microsoft Azure para a Locaweb. A plataforma resolve a sobrecarga operacional do gerenciamento de serviços de TI causada pelo crescimento de **1.273% no volume de chamados** (saltando de ~56/dia para ~766/dia).

### 🎯 Principais Destaques
- **Filtragem Automática de Ruído:** Identifica e descarta chamados de monitoramento sem intervenção manual (que representam ~65,5% do volume total).
- **Deduplicação Inteligente:** Agrupa falhas recorrentes sob um único **Incidente Pai**.
- **Alertas Proativos de SLA:** Notificação automatizada via Webhook/Teams ao atingir **85% do tempo de SLA (3h24min para P1/P2)**.
- **Predição de Volumetria (D+1 / D+7):** Previsão da demanda futura para melhor dimensionamento de equipes técnicas.

---

## 👥 Integrantes da Equipe Fluxo (Turma 2TSCOA)

| Nome | RM | Papel / Responsabilidades |
| :--- | :--- | :--- |
| **Vinícius Mugnes** | RM 563106 | **Líder de Projeto** & Arquiteto |
| **Gabriel Victor Santos Torriciello** | RM 564683 | Backend Developer & Data Engineer |
| **Isack Rafael** | RM 561943 | Analyst & ML Engineer |
| **Tiphany Nemet** | RM 566355 | Data Analyst & Documentação |
| **Nicole Lourival** | RM 563762 | UI/UX & Quality Assurance |

---

## 🏗️ Arquitetura da Solução

O pipeline processa eventos em tempo real, sem dependência de servidores dedicados, garantindo escala por demanda e custo *serverless*:
