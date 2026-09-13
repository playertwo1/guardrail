# Guardrails para Agentes de IA

Este repositório reúne um pacote reutilizável de controle para projetos desenvolvidos ou mantidos por agentes de inteligência artificial.

## Arquivos

- **AGENTS_GUARDRAILS.md** — instruções principais que todo agente deve ler antes de trabalhar no projeto. Define o fluxo obrigatório, limites de escopo, preservação do trabalho existente, validação e prevenção de desvios.
- **WATCHDOG.md** — guardião operacional. Mantém o agente dentro do pedido, reduz riscos de regressão e determina quando ele deve parar diante de uma decisão perigosa ou incerta.
- **AUDIT.md** — auditoria final independente. Deve ser aplicada antes de considerar uma alteração relevante concluída, verificando escopo, diff, regressões, qualidade, segurança e validações.

## Como usar em outro projeto

1. Copie os três arquivos para a raiz do repositório.
2. Leia `AGENTS_GUARDRAILS.md` antes de iniciar qualquer alteração.
3. Durante o planejamento e a execução, siga `WATCHDOG.md`.
4. Antes de finalizar uma tarefa relevante, execute o checklist de `AUDIT.md`.
5. Se o projeto já usar o nome `AGENTS.md`, incorpore o conteúdo de `AGENTS_GUARDRAILS.md` nele ou mantenha uma referência explícita para este arquivo.

## Princípio

**READ → UNDERSTAND → PLAN → CHANGE → TEST → AUDIT → FINISH**

O pacote permite autonomia proporcional na execução, mantendo mudanças conservadoras, rastreáveis e dentro do escopo autorizado.
