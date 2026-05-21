# Critérios de Aceite (Acceptance Criteria) — RouteSync

Este documento define as regras de negócio e os cenários de teste necessários para homologar as Histórias de Usuário da Sprint.

---

### 📍 Critérios para US01 — Visualização de Rota pelo Motorista

**Cenário 01: Motorista acessa a rota do dia com sucesso**
* **Dado que** o motorista está logado no aplicativo móvel e possui entregas atribuídas para o dia;
* **Quando** ele acessar a tela inicial de rotas;
* **Então** o sistema deve exibir o mapa com o trajeto otimizado e a lista ordenada de endereços de entrega.

**Cenário 02: Atualização de rota por tráfego**
* **Dado que** o motorista está seguindo a rota sugerida;
* **Quando** houver um congestionamento crítico detectado no trajeto à frente;
* **Então** o aplicativo deve emitir um alerta visual e recalcular automaticamente uma rota alternativa mais rápida.

---

### 💻 Critérios para US02 — Painel de Monitoramento do Supervisor

**Cenário 01: Visualização do status dos motoristas**
* **Dado que** o supervisor está na tela principal do Dashboard Web;
* **Quando** ele selecionar a visão do mapa geral;
* **Então** o sistema deve mostrar ícones coloridos representando cada motorista (Verde: No prazo | Amarelo: Alerta | Vermelho: Atrasado).

**Cenário 02: Alerta de desvio de rota**
* **Dado que** um motorista está ativo em uma entrega;
* **Quando** ele se desviar do trajeto planejado por mais de 2 km sem justificativa;
* **Então** o painel do supervisor deve disparar uma notificação de alerta em tempo real.
