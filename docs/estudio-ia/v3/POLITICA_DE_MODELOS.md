# Estúdio de IA — Política de modelos da V3 aprovada (08/11/2026)

> Complemento ao Plano Operacional V3. O usuário aprovou a arquitetura do estúdio, mas a instalação ou alteração efetiva de modelos/agentes continua dependente de autorização. O PDF V3 completo, com esta seção, será enviado separadamente pelo usuário.

## Três níveis diferentes de seleção

1. **Modelo da conversa principal:** selecionado no menu do Antigravity, sujeito à disponibilidade da conta. Thinking Low/Medium/High regula o esforço de raciocínio; uma mudança durante um turno não substitui o modelo da execução em andamento.
2. **Modelo de subagente:** o frontmatter do agente aceita `model: inherit`, `model: flash` ou `model: pro`. São classes/tier; não garantem um nome comercial específico.
3. **Política de roteamento:** A1 Diretor-Geral pode classificar a tarefa, designar especialista e recomendar/escolher o tier entre agentes ou mecanismos de invocação realmente disponíveis. Troca automática de modelo comercial da conversa não está comprovada; requer ferramenta e ensaio, não apenas instrução textual.

## Matriz A1–A10

| Agente | Tier inicial sugerido | Escalar para maior capacidade quando... |
|---|---|---|
| A1 Diretor-Geral | pro / inherit | houver conflito entre áreas, planejamento complexo e risco alto |
| A2 Arquitetura | pro | mudanças estruturais, persistência e integração de redes |
| A3 Regras e requisitos | inherit | fontes contraditórias, critérios ambíguos |
| A4 UI mobile | flash / inherit | acessibilidade, estados de interface complexos |
| A5 Sistemas | inherit / pro | bugs entre módulos e regressões difíceis |
| A6 Godot/Engine | pro | shaders, geometria, física, performance, câmera, navegação |
| A7 Arte/UX | inherit / pro | fidelidade entre várias referências, geometria/materiais |
| A8 Ambientação | inherit | mudanças de clima, zonas, fauna, áudio, lore |
| A9 Relator independente | inherit / pro | análise longa de logs, conflito ou retrabalho |
| A10 QA | pro / inherit | regressão, desempenho, verificação de cenas e validação complexa |

Somente A1 (`studio_director`), A6 (`godot_specialist`) e A10 (`qa_specialist`) foram relatados como configurados no Antigravity. A7 e A9 são prioridades futuras e **não devem ser instalados automaticamente**.

## Roteamento e exemplos

- **Flash / rápido:** inventário, leitura curta de arquivos, busca de cenas, listagem de recursos, normalização de relatórios.
- **Inherit / normal:** requisitos, inspeção simples, planejamento de pequenas mudanças, revisão de sprites e casos regulares.
- **Pro / complexo:** geometria e materiais, shaders da água, câmera do barco, colisões, falhas persistentes, QA difícil.
- **Escalonamento:** registrar falha observada, risco, justificativa, tier anterior e novo tier disponível. Se precisar mudar modelo comercial ou incorrer em custo, pedir confirmação ao usuário e não fingir que a troca já ocorreu.
- **Fallback:** se a classe proposta não estiver disponível, usar a suportada, reduzir escopo e informar a limitação.

## Comparação de modelos nominais

Exemplos sujeitos a disponibilidade do menu: Gemini 3.8 Flash para respostas rápidas; Gemini 4 Argon ou Claude Thinking para tarefas exigentes, se disponíveis. A lista e os limites dependem do plano. Não afirmar que a classe `pro` significa um produto específico. Anotar o modelo nominal efetivamente exibido e a classe do subagente em cada relatório.

## Teste obrigatório antes de mudar configurações

1. A1 faz inventário de agentes/skills/modelos sem editar projeto.
2. Repetir tarefa fictícia em `inherit` e `pro` (ou `flash` quando permitido) e verificar resultados e logs.
3. A10 valida qualidade; A9 audita as decisões de A1 e identifica retrabalho.
4. Registrar: tarefa, agente, tier solicitado, modelo observado, tempo, resultado, evidência, custo/quota visíveis e limitações.
5. Confirmar frontmatter, permissões, funções disponíveis e se o modelo foi realmente usado. Nenhum merge, instalação, publicação ou alteração do WorldForge antes da aprovação.

## Exemplos de uso no WorldForge

- Rocha piloto: A7 define critério visual; A6 usa classe maior para material/mesh; A10 verifica captura real; A9 audita o processo.
- Mar e barco: A6 pro para shaders/colisões; A5 inherit para lógica de gameplay, se instalado; A10 testa.
- Criaturas: A7 verifica estilo de macho/fêmea; A6 implementa animações dentro de Godot; A8 só se necessário.

## Fontes verificadas

- https://antigravity.google/docs/models
- https://antigravity.google/docs/subagents
- https://antigravity.google/docs/rules
- Plano Operacional V2 e V3 aprovados pelo diretor criativo.

**Este arquivo é documentação, não uma configuração de execução.**