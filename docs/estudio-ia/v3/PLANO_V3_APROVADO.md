# Estúdio de IA — Plano Operacional V3 APROVADO (08/11/2026)

> **Status:** planejamento editorial aprovado pelo diretor criativo. **Não é autorização para instalar agentes, escrever em projetos, alterar permissões, ativar serviços pagos ou realizar merge.**
>
> **PDF completo:** \`Estudio_IA_Antigravity_V3_APROVADA_08-11-2026.pdf\` (arquivo gerado e revisado; será anexado separadamente à pasta quando publicado no GitHub).
>
> **Documento de aplicação:** \`WorldForge_Plano_Atualizacao_Ilhota_045_08-11-2026.pdf\` pertence ao repositório privado do WorldForge, não a este.

## Propósito

O estúdio é um **catálogo reutilizável de agentes e skills**, não dez agentes agindo ao mesmo tempo. O usuário é **diretor criativo**, com decisão final sobre mudanças significativas. O A1 Diretor-Geral coordena, seleciona especialistas, explicita alternativas e pede aceite; o A9 Relator/Auditor é independente e pode avaliar também A1.

O repositório original de Claude Code Game Studios pode servir de inspiração, mas **não** substitui o catálogo A1–A10, nem autoriza copiar configurações externas sobre as personalizações atuais. Preservar os arquivos existentes deste repositório.

## Catálogo aprovado (papéis, não instalações)

| ID | Especialidade | Situação conhecida |
|---|---|---|
| A1 | Diretor-Geral / Mentor, \`studio_director\` | Relatado como configurado no Antigravity |
| A2 | Arquitetura de software e projetos | Planejado |
| A3 | Regras, requisitos e especificações | Planejado |
| A4 | Interface e experiência mobile | Planejado |
| A5 | Sistemas, gameplay e integrações | Planejado |
| A6 | Godot, indie game e motor gráfico, \`godot_specialist\` | Relatado como configurado |
| A7 | Arte/UX, fidelidade visual e arte técnica | **Prioridade de expansão, após autorização** |
| A8 | Ambientação, áudio e narrativa ambiental | Planejado |
| A9 | Relator / Auditor operacional independente | **Prioridade de expansão, após autorização** |
| A10 | QA, regressão e evidência, \`qa_specialist\` | Relatado como configurado |

Não substituir A2–A9 pelos nomes anteriores inventados pelo Antigravity (Game Designer, Release/Community, DevOps etc.) sem deliberação do usuário. O tamanho dez é **catálogo**, não cota obrigatória; o animador dedicado permanece opcional.

## Skills relatadas como existentes — preservar e verificar uso real

- \`studio-project-management\`
- \`godot-development\`
- \`game-qa-testing\`
- \`game-architecture-planning\`
- \`godot-optimization-debugging\`
- \`godot-scene-audit\`

Os caminhos e a ativação devem ser verificados na superfície real do Antigravity (App vs CLI). Indexação/listagem não prova execução.

## Novas skills propostas — ainda não instaladas

| Prioridade | Skill | Responsável sugerido |
|---|---|---|
| N1 | \`auditoria-de-agentes\` | A9, com independência de A1 |
| N2 | \`fidelidade-visual-godot\` | A7+A6+A10 |
| N3 | \`geometria-materiais-ambientes\` | A7+A6 |
| N4 | \`pipeline-sprites-animacoes\` | A6+A7 |
| N5 | \`oceano-mare-profundidade\` | A6+A8 |
| N6 | \`fauna-habitats-comportamentos\` | A5+A6+A8 |
| N7 | \`barco-navegacao-interacoes\` | A5+A6 |

Priorizar N1–N4 conforme diagnóstico. N5–N7 aguardam o início dos módulos correspondentes. Evitar duplicação com skills existentes.

## Pipeline aprovado

1. O diretor criativo aprova referências em Flow/Nano Banana. Podem ser usadas ferramentas novas de imagem **somente após verificação de disponibilidade e eventual custo**.
2. A7 especifica silhueta, geometria, materiais, iluminação, UI e prioridades de fidelidade.
3. A6 adapta as artes e recursos para Godot, inclusive sprites, cenas, animações funcionais e desempenho; A5 apoia sistemas se necessário.
4. A10 testa material implementado, cena em execução, regressões e dispositivo móvel.
5. A9 audita as evidências, delegação, retrabalho, cumprimento de regras e decisões de A1.
6. A1 apresenta resultados, opções e riscos; usuário aceita, pede ajustes ou desfaz.

**Arte conceitual não é spritesheet pronto, screenshot de Godot ou evidência de desempenho.** Seis comportamentos de uma criatura não equivalem a seis frames.

## Pendências obrigatórias

- Conferir manifesto global \`~/.gemini/studio/STUDIO_MANIFEST.md\` — sete futuros agentes divergentes da equipe A1–A10.
- Validar arquivo de regra \`studio_rules.md\`, YAML/frontmatter e trigger; presença em disco não garante que esteja ativa.
- Verificar duplicatas, aliases e diretórios agentes; testar precedência antes de excluir algo; verificar backup \`~/.gemini/backup_studio_initial.tar.gz\`.
- Verificar permissões reais dos três agentes; \`write_tools: true\` não é isolamento.
- Confirmar carregamento das seis skills no App e no CLI.
- Realizar microteste de **somente leitura**, observando invocação, logs, respostas e auditoria independente.
- Confirmar Godot instalado, Compatibility, limites headless e possibilidade de captura de tela.
- Não declarar desempenho no Moto G20 sem teste físico.

## Repositórios e isolamento

- Este repositório: **\`gutshimura1-wq/Meu-Estudio-de-Jogos-IA.\`** (público). Guardar arquitetura, regras e guias sem chaves ou dados privados.
- Jogo: **\`gutshimura1-wq/world-forge-rpg\`** (privado).
- Branch de teste do jogo já criada e verificada: **\`demo/estudio-ia-ilhota-revisao\`**, derivada de **\`update/0.4.4-stage1-closure\`**.
- Não sobrescrever \`main\`, fazer force-push, merge ou publicar builds sem aceite explícito.

## Ordem de adoção do estúdio

1. Inventariar e corrigir, **após autorização específica**, as pendências.
2. Planejar instalação de A9 Relator, A7 Arte/UX e skills N1–N4, cada qual com rollback.
3. Fazer microteste de delegação e auditoria sem tocar no jogo.
4. Planejar piloto de fidelidade em uma rocha do WorldForge na branch de laboratório.
5. Executar piloto só depois de nova aprovação, mostrar capturas, testes e auditoria.
6. Ampliar por áreas, mantendo histórico e portas de aprovação.

**Situação deste registro:** espelho textual de orientação do PDF V3 aprovado. A publicação deste Markdown não instala nem ativa agentes.