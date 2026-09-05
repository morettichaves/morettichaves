# AGENTS.md

## Fluxo obrigatório de trabalho

Estas regras se aplicam a qualquer agente, modelo ou colaborador que trabalhe neste repositório.

1. Crie uma GitHub Issue antes de iniciar qualquer correção, melhoria ou nova funcionalidade.
2. Classifique claramente a tarefa como correção, melhoria, documentação ou nova funcionalidade.
3. Crie uma branch específica a partir da branch principal. Use nomes como fix/12-descricao, feat/18-descricao ou docs/21-descricao.
4. Nunca envie alterações diretamente para a branch principal.
5. Abra um Pull Request para toda mudança.
6. Mencione a Issue na descrição do PR usando Closes #numero quando o PR concluir a tarefa ou Refs #numero quando houver trabalho pendente.
7. Execute testes, lint e validações disponíveis antes de solicitar merge.
8. Atualize a documentação quando o comportamento, a instalação ou a arquitetura forem alterados.
9. Use merge somente após revisar o diff e confirmar que os critérios de aceite da Issue foram atendidos.

## Interfaces e movimento

Quando o projeto possuir interface:

- Siga os princípios aplicáveis de Motion Principles.
- Forneça skeletons para carregamentos perceptíveis.
- Use lazy loading para recursos pesados.
- Aplique animações suaves de entrada, saída, carregamento e progresso.
- Respeite prefers-reduced-motion e mantenha acessibilidade por teclado.
- Evite animações decorativas que prejudiquem desempenho ou clareza.

## Observabilidade e qualidade

- Defina logs estruturados, tratamento de erros e métricas adequadas ao tamanho do projeto.
- Quando houver produção, escolha uma solução de observabilidade compatível, como Sentry, Datadog, New Relic ou OpenTelemetry.
- Use lint, análise estática e verificação de dependências compatíveis com a stack.
- Para JavaScript/TypeScript, considere Biome, Commitlint, Knip e Stryker.
- Para outras stacks, utilize ferramentas equivalentes em vez de adicionar dependências incompatíveis.
- Mantenha testes unitários e de integração. Adicione testes end-to-end quando existir um fluxo completo de usuário ou API.
- Publique cobertura com Codecov quando a integração estiver configurada.
- Use Playwright para testes end-to-end de interfaces web quando aplicável.
