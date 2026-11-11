# RH — documentação dos fluxos

Os arquivos abaixo documentam os fluxos identificados na [transcrição](transcricao.md) e no [board RH do Miro](https://miro.com/app/board/uXjVHmYGPIM=/). A consulta ao board foi realizada em **05/11/2026**, no fuso America/Sao_Paulo. A data da reunião não foi informada na fonte.

Cada fluxo tem uma pasta própria com seu arquivo **BPMN 2.0 XML** e um **process-assessment.md** com a avaliação do processo, conforme as orientações do projeto. Os cenários AS-IS e TO-BE ficam em processos e diagramas separados dentro do arquivo. Todos são descritivos e não executáveis. A documentação de cada processo e atividade contém fontes, responsabilidades, entradas, saídas, regras relatadas, limitações e dúvidas. Os diagramas têm informações de posição (BPMN DI) para abertura em um modelador compatível; dependendo da ferramenta, é necessário selecionar cada diagrama do arquivo.

Os **13 arquivos**, com **23 processos/diagramas**, passaram pela validação XSD oficial e pela conferência das conexões e posições dos diagramas. Consulte o [registro de validação e seus limites](validacao.md).

**AS-IS** significa prática relatada nas fontes, ainda sujeita à conferência do setor. **TO-BE** significa proposta discutida, ainda não validada. Nos temas que não possuem sequência atual suficiente, há somente o TO-BE e a lacuna do AS-IS fica expressa na documentação. Um evento final de “limite do recorte” indica onde termina a evidência disponível; não comprova resolução ou implantação do processo.

```text
rh_recursos_humanos/
├── transcricao.md
├── fontes/miro/
└── nome_do_fluxo/
    ├── nome_do_fluxo.xml
    └── process-assessment.md
```

Cada avaliação contém **1. Visão Geral**, **2. Problemas Identificados**, **3. Oportunidades de Melhoria** e **4. Questões em Aberto**, com referências à transcrição, aos recortes do Miro e ao modelo do próprio fluxo. Propostas e informações pendentes permanecem identificadas como tal.

## Inventário e limites

| Modelo BPMN | Avaliação do processo | Conteúdo e limites | Base principal |
| --- | --- | --- | --- |
| [Captação e admissão](captacao_admissao/captacao_admissao.xml) | [Avaliação](captacao_admissao/process-assessment.md) | Pedido da vaga, recrutamento, entrevista, teste quando aplicável, aprovação, documentos, exame/cadastro, integração e ponto. Interface com PJ. AS-IS e TO-BE. | Transcrição §§1–3, 5 e 11; Miro Captação/Admissão. |
| [Contratação de freelancers](contratacao_freelancers/contratacao_freelancers.xml) | [Avaliação](contratacao_freelancers/process-assessment.md) | Solicitação temporária, indicação/histórico, contato, condições, prestação e pagamento por recibo relatado. AS-IS e TO-BE. | Transcrição §4; Miro Prestadores. |
| [Contratação PJ](contratacao_pj/contratacao_pj.xml) | [Avaliação](contratacao_pj/process-assessment.md) | Variante após aprovação: documentação, contrato e integração pertinente; condições específicas a validar. AS-IS e TO-BE parcial. | Transcrição §5; notas de Captação/Admissão e Férias. |
| [Desligamento](desligamento/desligamento.xml) | [Avaliação](desligamento/process-assessment.md) | Iniciativa da empresa ou do colaborador, avaliação/reversão, documentos, pagamentos, devoluções e propostas para acessos/entrevista de saída. AS-IS e TO-BE. | Transcrição §§6 e 8; Miro Demissão. |
| [Planejamento de férias](planejamento_ferias/planejamento_ferias.xml) | [Avaliação](planejamento_ferias/process-assessment.md) | Relatório, proposta do RH, aval do líder, confirmação e registro; proposta de preferência do colaborador, calendário e avisos. AS-IS e TO-BE. | Transcrição §7; Miro Férias. |
| [Planejamento de endomarketing](planejamento_endomarketing/planejamento_endomarketing.xml) | [Avaliação](planejamento_endomarketing/process-assessment.md) | Levantamento anual de ações/custos, aprovação do CEO e revisão do orçamento; planejamento de feriados relacionado. AS-IS e TO-BE. | Transcrição §9; Miro Endomarketing. |
| [Ações com brindes](acoes_brindes/acoes_brindes.xml) | [Avaliação](acoes_brindes/process-assessment.md) | Pesquisa, personalização pela criação e distribuição; proposta de controle de recebimento e preparação antecipada. AS-IS e TO-BE. | Transcrição §9; Miro Endomarketing. |
| [Dinâmicas de equipe](dinamicas_equipe/dinamicas_equipe.xml) | [Avaliação](dinamicas_equipe/process-assessment.md) | Planejamento, ajuste de turnos e comunicação; recorte parcial das rotinas em construção. Frequência trimestral é proposta. AS-IS parcial e TO-BE. | Transcrição §§8–9; Miro Endomarketing. |
| [Feedback e avaliação](feedback_avaliacao/feedback_avaliacao.xml) | [Avaliação](feedback_avaliacao/process-assessment.md) | Conversas atuais sem ciclo regular documentado; proposta de conversas periódicas e registros com acesso por papel. AS-IS parcial e TO-BE. | Transcrição §§6 e 8; notas de Demissão e Endomarketing. |
| [Desenvolvimento e PDI](desenvolvimento_pdi/desenvolvimento_pdi.xml) | [Avaliação](desenvolvimento_pdi/process-assessment.md) | Registro de pontos, metas, cursos de interesse e possíveis sugestões. Somente TO-BE parcial; não há aprovação, custeio ou acompanhamento detalhados. | Transcrição §8; notas sobre PDI e ausência de plano de carreira. |
| [Gestão de EPIs](gestao_epis/gestao_epis.xml) | [Avaliação](gestao_epis/process-assessment.md) | Proposta de controle por função, entrega/troca e confirmação. Somente TO-BE parcial; itens, periodicidade e responsáveis ainda a definir. | Transcrição §§3, 4 e 10; nota sobre troca de EPIs. |
| [Solicitações internas](solicitacoes_internas/solicitacoes_internas.xml) | [Avaliação](solicitacoes_internas/process-assessment.md) | Recebimento atual pelo RH; proposta de categorias, triagem, aceite/recusa/encaminhamento e direcionamento de tecnologia à TI. O recorte termina na decisão/encaminhamento. | Transcrição §10; notas sobre chamados e concentração de pedidos no RH. |
| [Gestão de benefícios](gestao_beneficios/gestao_beneficios.xml) | [Avaliação](gestao_beneficios/process-assessment.md) | Registro de fixos/opcionais e escolha ou solicitação de alteração. Somente TO-BE parcial; não representa concessão ou desconto efetivado. | Transcrição §§3 e 10; notas sobre benefícios. |

## Divergências e informações a confirmar

| Tema | Evidências e tratamento adotado |
| --- | --- |
| Pagamento e uniforme | O Miro condiciona liberação à devolução (widget `3458764683994572199`). A transcrição §6 diz que essa sugestão foi descartada. O fluxo registra o conflito e mantém pagamento independente da devolução. |
| Férias e liderança | O Miro diz que o RH define férias, não os líderes (`3458764683995247715`). A transcrição §7 descreve proposta do RH, aval do líder e confirmação com funcionário. Esse relato detalha o AS-IS; a divergência continua pendente de validação. |
| Feedback | O Miro diz “não há feedbacks” (`3458764683994213097`); a transcrição §8 relata conversas sem ciclo regular documentado. O AS-IS registra conversas informais e explicita a divergência. |
| Integração | O Miro diz “Não tem onboarding” (`3458764683992659509`), mas contém etapa de integração e a transcrição §3 descreve apresentação, manual e orientação. A lacuna é de estrutura e consistência, sem apagar a integração existente. |
| Teste operacional | O Miro pergunta “Área de produção?” e não desenha continuidade após o teste. A transcrição §3 diz que pode haver teste e descreve avaliação/aprovação. A complementação do desenho e a aplicabilidade estão identificadas, sem tornar teste obrigatório para toda a produção. |
| Nome dos sistemas | “Contmatic” aparece no Miro (`3458764683994924148`). A transcrição pede confirmar nomes/fornecedores e menciona “Ágora” para ponto. Não há integração técnica verificada. |
| Dia das Crianças | O Miro registra filhos menores de 13 anos e R$ 100 (`3458764683996268714`). A transcrição §9 apenas se refere à faixa definida pela empresa. Valor e elegibilidade permanecem como relato do board a confirmar. |
| Descanso PJ | Miro e transcrição citam condições anuais de descanso; a transcrição restringe o relato a determinados contratos. Não foi generalizada uma política única nem usado o cálculo de férias CLT para PJ. |

Os prazos citados — quinze dias para recrutamento, uma semana entre aprovação e início, duração do teste, antecedência de férias e frequências de feedback/dinâmicas — mantêm seu contexto de referência ou proposta. Não foram convertidos em SLAs, temporizadores obrigatórios ou regras legais verificadas. As descrições de contratos e obrigações registram o que foi dito na reunião.

## Temas sem fluxo completo nas fontes

- **Ponto, folha e integrações:** são contexto e interfaces dos fluxos. Não há sequência suficiente para documentar processamento de folha ou apuração de ponto como processos próprios.
- **Pesquisa de clima:** a frequência semestral foi mencionada e seus resultados podem apoiar dinâmicas; aplicação, tratamento, responsáveis e devolutiva não foram detalhados.
- **Vagas internas, promoções e mudanças de função:** ideias registradas junto ao desenvolvimento; critérios, decisões e aprovações não foram definidos.
- **Perfil e comunicação entre setores:** nome, foto, função, equipe, chegada e aniversário foram propostas sem rotina detalhada de manutenção e publicação.
- **Denúncias e sugestões anônimas:** necessidade identificada, com receptor, sigilo, acesso e tratamento pendentes. Não foram inseridas automaticamente na triagem genérica do RH.
- **Atendimento de TI e outras áreas:** o fluxo de solicitações descreve encaminhamento, sem inventar resolução, prazo ou escalonamento dos destinatários.

## Fontes preservadas

- [Transcrição integral](transcricao.md), proveniente do [documento revisado no Drive](https://docs.google.com/document/d/15Bmqzj7P4mctLZawF8BEQuLMBYOq9F0_/edit).
- [Registro da consulta ao Miro](fontes/miro/consulta.json), com inventário de áreas e resultados das leituras.
- Recortes do board: [Captação/Admissão](fontes/miro/area_0.svg), [Endomarketing](fontes/miro/area_1.svg), [Demissão](fontes/miro/area_2.svg), [Prestadores](fontes/miro/area_3.svg), [Férias](fontes/miro/area_4.svg) e [notas gerais](fontes/miro/area_5.svg). São cópias técnicas em SVG do conteúdo retornado pelo conector; o board é a referência para visualização original.

Os arquivos preservam IDs dos widgets para rastreamento. `skipped_count` em cada recorte indica conectores cujo outro extremo não está naquela seleção; não equivale a fluxo interno omitido. A união das seis leituras contém **109 IDs únicos**, igual aos **109 itens** do inventário do board, incluindo grupos, atividades, notas e conectores.
