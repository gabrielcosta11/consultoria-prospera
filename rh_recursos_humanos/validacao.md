# Validação da documentação de RH

Conferência final em **05/11/2026**, no fuso America/Sao_Paulo.

**Resultado:** 13 pastas de fluxo, cada uma com seu XML e seu `process-assessment.md`; 23 processos/diagramas, 196 nós e 189 conexões. Nenhum erro estrutural, link local ausente ou alerta geométrico encontrado nas verificações abaixo.

## Verificações executadas

- Validação de todos os arquivos com `lxml.etree.XMLSchema` e os cinco esquemas oficiais da OMG (`BPMN20.xsd`, `Semantic.xsd`, `BPMNDI.xsd`, `DC.xsd` e `DI.xsd`), disponíveis na [especificação BPMN 2.0.2](https://www.omg.org/spec/BPMN/2.0.2).
- IDs únicos por arquivo, referências resolvidas, fluxos contidos no respectivo processo e consistência entre `sequenceFlow`, `incoming` e `outgoing`.
- Todos os nós de fluxo alcançáveis desde um início e com caminho até um fim; decisões exclusivas com saídas identificadas.
- Todos os processos marcados como não executáveis; documentação presente em cada processo; um plano BPMN DI por processo, com posições para todos os nós e rotas para todas as conexões.
- Rotas verificadas geometricamente: nenhum segmento atravessa o interior de um nó alheio à conexão. Os diagramas também passaram por revisão cruzada dos agentes.
- Referências a widgets dos XMLs encontradas nas fontes locais; links locais dos arquivos Markdown resolvidos.
- União dos seis recortes SVG: 109 IDs únicos, igual ao inventário de 109 itens retornado pelo Miro.
- Conteúdo da transcrição comparado ao DOCX obtido do Drive: 86 parágrafos preservados, considerando apenas a adaptação de títulos e listas para Markdown.
- Revisão cruzada das fontes e dos modelos por três subagentes, além da revisão de integração: limites do AS-IS/TO-BE, variantes contratuais, divergências, responsáveis pendentes e sequência das interfaces.
- Conferência das 13 avaliações: presença e ordem exatas de `1. Visão Geral`, `2. Problemas Identificados`, `3. Oportunidades de Melhoria` e `4. Questões em Aberto`, conteúdo em todas as seções, referências locais existentes e IDs do Miro encontrados nos recortes preservados.
- Reorganização em pastas próprias: nenhum XML de fluxo permaneceu na raiz de RH. Os modelos foram preservados; somente referências textuais da documentação XML foram ajustadas para os novos caminhos. A estrutura BPMN e os diagramas foram comparados antes e depois dessa alteração e permaneceram iguais.
- Índice, referências entre fluxos, caminhos para fontes compartilhadas e orientações `AGENTS.MD` atualizados para a estrutura por fluxo.

A validação verifica estrutura e coerência documental. Não equivale à aprovação dos processos pelo RH. A importação/renderização em um editor BPMN específico não foi testada; o comportamento de seleção entre os múltiplos diagramas depende da ferramenta.

## Resultado por arquivo

| Arquivo | Processos/diagramas | Nós | Conexões | XSD |
| --- | ---: | ---: | ---: | --- |
| [acoes_brindes.xml](acoes_brindes/acoes_brindes.xml) | 2/2 | 11 | 9 | Válido |
| [captacao_admissao.xml](captacao_admissao/captacao_admissao.xml) | 2/2 | 40 | 40 | Válido |
| [contratacao_freelancers.xml](contratacao_freelancers/contratacao_freelancers.xml) | 2/2 | 21 | 19 | Válido |
| [contratacao_pj.xml](contratacao_pj/contratacao_pj.xml) | 2/2 | 9 | 7 | Válido |
| [desenvolvimento_pdi.xml](desenvolvimento_pdi/desenvolvimento_pdi.xml) | 1/1 | 5 | 5 | Válido |
| [desligamento.xml](desligamento/desligamento.xml) | 2/2 | 31 | 35 | Válido |
| [dinamicas_equipe.xml](dinamicas_equipe/dinamicas_equipe.xml) | 2/2 | 10 | 8 | Válido |
| [feedback_avaliacao.xml](feedback_avaliacao/feedback_avaliacao.xml) | 2/2 | 7 | 5 | Válido |
| [gestao_beneficios.xml](gestao_beneficios/gestao_beneficios.xml) | 1/1 | 5 | 5 | Válido |
| [gestao_epis.xml](gestao_epis/gestao_epis.xml) | 1/1 | 5 | 4 | Válido |
| [planejamento_endomarketing.xml](planejamento_endomarketing/planejamento_endomarketing.xml) | 2/2 | 14 | 14 | Válido |
| [planejamento_ferias.xml](planejamento_ferias/planejamento_ferias.xml) | 2/2 | 25 | 24 | Válido |
| [solicitacoes_internas.xml](solicitacoes_internas/solicitacoes_internas.xml) | 2/2 | 13 | 14 | Válido |

## Integridade da transcrição

SHA-256 de `transcricao.md`: `fd8b6548ad928a6a5ce9ac9428b5b5de6075f96377e21f2d9268d8a9fed89d3c`.

Os scripts e dependências auxiliares de geração/validação ficaram em diretório temporário, fora do projeto. Os entregáveis do projeto são a documentação, os modelos e os recortes das fontes.
