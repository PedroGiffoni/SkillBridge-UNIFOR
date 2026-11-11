# Registro da configuração de gestão — 11/11/2026

## Escopo autorizado

Somente planejamento, Issues, Project nº 2 e documentação. Nenhuma funcionalidade da aplicação implementada, nenhum teste com usuário declarado e nenhuma Issue marcada como concluída.

O destino inicial da missão era `PedroGiffoni/skillbridge`. Durante a execução, o titular corrigiu o destino para **PedroGiffoni/SkillBridge-UNIFOR**, que estava sem arquivos e com uma única Issue, SB-01. Essa Issue foi reaproveitada. A SB-01 criada no destino anterior foi desvinculada do Project e encerrada como não planejada, preservando seu histórico; ela não representa trabalho concluído.

## Campos e quadro

- Project preservado: `PVT_kwHODj1b184BrN7c`, número 2, proprietário PedroGiffoni.
- Status normalizado para Backlog, A fazer, Em desenvolvimento, Em revisão e Concluído, preservando IDs existentes.
- Sprint normalizado para Sprint 1, Sprint 2 e Sprint 3; os IDs das duas opções existentes foram preservados.
- Categoria normalizada, incluindo Front-end; opções existentes preservadas.
- Repositório SkillBridge-UNIFOR vinculado ao Project nº 2.
- Kanban Geral existente verificado: Board com colunas por Status e sem filtro.
- Assignees e Effort não preenchidos: equipe e estimativas não confirmadas.

## Impedimento comprovado

Priority, Start date, Target date e Effort são campos derivados de Issues (`isIssueField: true`), com referência subjacente indisponível à autenticação atual. `updateProjectV2Field` recusou alterar Priority; `updateProjectV2ItemFieldValue` recusou datas, exigindo `updateIssueFieldValue`. A consulta dos campos da conta retornou `FORBIDDEN`: a conta autenticada não tem permissão para recuperar essas informações por essa API.

O token já possui escopo `project`; portanto, `gh auth refresh -s project` não resolve o impedimento observado. É necessário acesso aos campos compartilhados de Issues e opções compatíveis para preencher Priority e datas na interface ou por API autorizada. Não foram removidos nem duplicados campos para contornar a restrição. Prioridades e datas planejadas estão registradas integralmente nas 26 descrições e documentos.

## Documentos

README com ilustração conceitual identificada; backlog, planejamento das sprints, fluxo Kanban e critérios de conclusão; para cada sprint, planejamento, relatório de execução pendente e README do diretório de evidências. Este registro e o arquivo de verificação complementam a rastreabilidade.

## Próximos passos

Resolver acesso aos campos Priority e datas, confirmar integrantes e capacidade, selecionar trabalho da Sprint 1 e produzir os entregáveis reais. Registrar início/término reais separadamente das datas planejadas. Validar o MVP com pelo menos 10 usuários e coletar cinco ou mais evidências reais nas atividades apropriadas. Entrega acadêmica prevista no Dream Shape em 27/11/2026.
