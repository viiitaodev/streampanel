[English](README.md)

# Stream Panel

<div align="center">
  <img src="./assets/logo.png" alt="Stream Panel" width="120" />
  <h3>Central de Controle Unificada para Criadores</h3>
  <p>Um workspace desktop profissional para gerenciar chat, eventos e operações da live em múltiplas plataformas.</p>
</div>

<p align="center">
  <img src="./assets/hero.png" alt="Banner do Stream Panel" />
</p>

---

## O que é o Stream Panel?

O **Stream Panel** é uma aplicação desktop criada para centralizar o fluxo operacional de um criador: **chat unificado**, **feed de atividades**, **controles de metadados da transmissão** e uma base escalável para **integrações multi-plataforma** (Twitch, YouTube, Kick, TikTok).

O projeto é construído com uma arquitetura **em tempo real** e **modular**, permitindo que novas funcionalidades sejam entregues como painéis independentes, mantendo uma UX consistente.

<p align="center">
  <img src="./assets/mockup-dashboard.png" alt="Mockup fictício do dashboard" />
</p>

---

## Capacidades Principais

- **Chat Unificado**: uma única superfície para ler, filtrar e moderar mensagens das plataformas suportadas.
- **Feed de Atividades**: eventos normalizados (follow, sub, resgate, alertas) exibidos em um fluxo consistente.
- **Controles do Criador**: edição de título/categoria e execução de ações operacionais via comandos rápidos.
- **UX orientada a painéis**: layout escalável onde recursos são construídos como módulos composáveis.

---

## Arquitetura Técnica

O Stream Panel segue uma separação clara de responsabilidades em três camadas:

- **Shell Desktop (Electron)**: janelas, comportamentos nativos, bridges seguras e ciclo de vida no desktop.
- **UI (React)**: evolução rápida de painéis e telas com uma abordagem moderna baseada em componentes.
- **Backend (NestJS)**: integrações, normalização de eventos e entrega em tempo real via WebSockets.

<p align="center">
  <img src="./assets/architecture.png" alt="Visão geral da arquitetura" />
</p>

---

## Stack de Tecnologias

### Frontend
- **React 18 + TypeScript**
- **Vite** para builds rápidos e DX
- **Tailwind CSS** como design system
- **Socket.io Client** para updates em tempo real

### Backend
- **NestJS** para uma camada de API estruturada e escalável
- **Socket.io Gateway** para streaming de eventos com baixa latência
- **Prisma ORM** para persistência previsível
- **PostgreSQL** como system of record

### Desktop
- **Electron** como runtime desktop
- Padrões de **IPC seguro** para operações frontend ↔ desktop

---

## Princípios de Design

- **Clareza operacional**: informações críticas ficam sempre visíveis, com prioridade por urgência.
- **Feedback de baixa latência**: ações refletem instantaneamente via propagação em tempo real.
- **Modularidade escalável**: novos recursos devem ser painéis — não reescritas.
- **UI profissional**: espaçamento, tipografia e semântica de cores consistentes para navegação rápida.

---

## Direção do Projeto

O Stream Panel é construído para evoluir para uma **plataforma completa de operações do criador**, incluindo:

- Workflows mais profundos de **moderação**
- Gestão **multi-conta** e multi-canal
- **Automações** e ações baseadas em regras (alertas, triggers, workflows)
- Expansão da cobertura e normalização **multi-plataforma**

---

<div align="center">
  <sub>Desenvolvido pela Nyxis Studio • Stream Panel</sub>
</div>
