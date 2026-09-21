## 🌌 Visão Geral

O **PULSO** é uma solução de AIOps *serverless* e orientada a eventos construída no Microsoft Azure para a Locaweb. A plataforma resolve a sobrecarga operacional do gerenciamento de serviços de TI causada pelo crescimento de **1.273% no volume de chamados** (saltando de ~56/dia para ~766/dia).

### 🎯 Principais Destaques
- **Filtragem Automática de Ruído:** Identifica e descarta chamados de monitoramento sem intervenção manual (que representam ~65,5% do volume total).
- **Deduplicação Inteligente:** Agrupa falhas recorrentes sob um único **Incidente Pai**.
- **Alertas Proativos de SLA:** Notificação automatizada via Webhook/Teams ao atingir **85% do tempo de SLA (3h24min para P1/P2)**.
- **Predição de Volumetria (D+1 / D+7):** Previsão da demanda futura para melhor dimensionamento de equipes técnicas.
---

## 🏗️ Arquitetura da Solução

O pipeline processa eventos em tempo real, sem dependência de servidores dedicados, garantindo escala por demanda e custo *serverless*:
