# Contexto e orientações do projeto

## Contexto da empresa e da consultoria

A Próspera é uma empresa especializada no desenvolvimento e na produção de materiais de ponto de venda (PDV), utilizados por marcas para promover e expor seus produtos em estabelecimentos comerciais.

Sua operação abrange todo o ciclo de desenvolvimento e entrega desses materiais, desde a compreensão da necessidade do cliente até a instalação no ponto de venda.

Este projeto apoia uma consultoria de processos realizada para a Próspera. Seu propósito é documentar como a empresa opera atualmente e descrever os processos futuros propostos, criando uma base compartilhada para compreender a operação e discutir melhorias.

## Objetivo

Documentar os processos da Próspera em duas perspectivas:

- **AS-IS — situação atual:** registrar como os processos são executados hoje, incluindo atividades, responsáveis, entradas, saídas, decisões, interações entre áreas e dificuldades identificadas nas fontes.
- **TO-BE — situação futura proposta:** descrever como os processos deverão funcionar após as melhorias discutidas no trabalho de consultoria, explicitando mudanças em relação ao AS-IS, responsabilidades e pontos que ainda dependem de validação.

A documentação deve permitir compreender o funcionamento dos processos e a relação entre a situação atual e a situação futura proposta.

## Escopo e limites

Este projeto é exclusivamente de documentação de processos. Não será desenvolvida nenhuma aplicação, sistema, protótipo de software ou funcionalidade de produto.

O trabalho compreende organizar, descrever, analisar e manter a documentação dos processos. Eventuais necessidades de ferramentas ou sistemas identificadas durante a análise devem ser registradas como necessidades ou propostas de melhoria, sem implementação de software neste projeto.

O ciclo operacional da empresa fornece o contexto geral do trabalho. A delimitação de cada processo e o nível de detalhe de sua documentação devem acompanhar as evidências disponíveis e as definições da consultoria, sem presumir que todas as etapas já foram mapeadas.

## Organização da documentação por área

Os processos serão mapeados e organizados por área da empresa. Cada área terá uma pasta própria dentro de `documentacao_processos`, contendo:

- Um arquivo `AGENTS.MD` com o contexto da área, suas responsabilidades e as orientações específicas para documentar seus processos, complementando as diretrizes gerais deste arquivo.
- Uma pasta própria para cada fluxo, contendo o arquivo `.xml` em conformidade com BPMN 2.0 e um arquivo `process-assessment.md` com a avaliação do processo.

Cada `process-assessment.md` deve conter as quatro seções abaixo, com análise específica do fluxo e referências às fontes utilizadas:

1. **Visão Geral:** resumo do processo, objetivo, áreas envolvidas e contexto operacional.
2. **Problemas Identificados:** falhas, retrabalho, gargalos, ineficiências e dificuldades evidenciadas na situação atual. Quando a prática atual não estiver suficientemente documentada, registrar a lacuna sem presumir uma falha operacional.
3. **Oportunidades de Melhoria:** possibilidades de otimização, automação, padronização e simplificação, relacionadas aos problemas identificados. Distinguir propostas discutidas nas fontes de sugestões analíticas adicionais, sem apresentá-las como decisões aprovadas.
4. **Questões em Aberto:** dúvidas, informações pendentes de validação e decisões a esclarecer com os responsáveis.

Os nomes das pastas e dos arquivos devem identificar claramente a área e o fluxo correspondente. A separação entre AS-IS e TO-BE deve permanecer explícita na documentação dos fluxos.

Exemplo ilustrativo de organização:

```text
documentacao_processos/
├── AGENTS.MD
└── nome_da_area/
    ├── AGENTS.MD
    ├── nome_do_fluxo_1/
    │   ├── nome_do_fluxo_1.xml
    │   └── process-assessment.md
    └── nome_do_fluxo_2/
        ├── nome_do_fluxo_2.xml
        └── process-assessment.md
```

## Fontes de referência

A documentação será construída a partir de duas fontes principais:

- **Fluxos construídos no Miro:** representam os processos mapeados durante a consultoria e orientam a descrição de suas etapas, decisões e conexões.
- **Transcrições das reuniões armazenadas no Google Drive:** registram as discussões que serviram de base para a construção dos fluxos e oferecem contexto, explicações, exceções e decisões relevantes.

As fontes devem ser utilizadas de forma complementar. Os fluxos orientam a leitura da sequência do processo; as transcrições ajudam a compreender o significado das etapas e os motivos das decisões de mapeamento.

## Diretrizes para produzir a documentação

- Escrever em português, com linguagem clara, objetiva e consistente com os termos utilizados pela Próspera.
- Consultar os fluxos e as transcrições pertinentes antes de descrever um processo. Não apresentar conteúdo de uma fonte como verificado sem tê-la consultado.
- Registrar, sempre que disponível, a referência ao quadro ou fluxo do Miro e às reuniões ou transcrições utilizadas, com links e datas que permitam rastrear a origem das informações.
- Separar explicitamente o AS-IS do TO-BE. Uma proposta de melhoria não deve ser descrita como prática atual.
- Diferenciar fatos identificados nas fontes, propostas da consultoria, decisões validadas e questões pendentes de validação.
- Não inventar etapas, responsáveis, regras, prazos, indicadores ou decisões. Quando a informação não estiver disponível, registrar a lacuna ou a dúvida.
- Se houver divergência entre o fluxo e a transcrição, registrar a inconsistência e a necessidade de validação, sem escolher silenciosamente uma das versões.
- Preservar particularidades, exceções e interfaces entre áreas quando estiverem documentadas nas fontes.
- Manter a documentação focada nos processos de negócio, sem transformar o projeto em uma iniciativa de desenvolvimento de software.

## Conteúdo esperado por processo

Conforme as informações disponíveis, a documentação de cada processo deve contemplar:

- Nome, objetivo e limites do processo: evento de início e condição de encerramento.
- Áreas, papéis e responsabilidades envolvidos.
- Entradas, saídas e documentos ou registros utilizados.
- Descrição do AS-IS: etapas, decisões, regras de negócio, exceções e interações.
- Dificuldades, gargalos e oportunidades de melhoria identificados, com sua origem.
- Descrição do TO-BE, quando houver proposta: mudanças, justificativas e impactos esperados.
- Referências às fontes e registro de dúvidas, dependências e validações pendentes.

Esta estrutura orienta a organização do conteúdo; campos sem evidência devem permanecer identificados como pendentes, sem preenchimento por suposição.
