# Framework de Decisão — Baseado em Ciência Comportamental

> Um framework de decisão baseado em ciência comportamental, para ajudar a responder uma pergunta difícil: persistir ou encerrar um projeto, ideia ou plano em andamento? A entrega inclui a ferramenta interativa **Bifurcar — Um caminho, duas direções**.

## Índice
- [Contexto e Objetivos](#contexto-e-objetivos)
- [Curadoria de Fontes](#curadoria-de-fontes)
- [Fluxo de Trabalho](#fluxo-de-trabalho)
- [Engenharia de Prompts e Cicatrizes](#engenharia-de-prompts-e-cicatrizes)
- [Miniguia de Estudo Final](#miniguia-de-estudo-final)
- [Ferramenta Interativa: Bifurcar](#ferramenta-interativa-bifurcar)
- [Lições Aprendidas](#lições-aprendidas)
- [Licenciamento e Uso](#licenciamento-e-uso)

---

## Contexto e Objetivos

**Desafio:** este projeto foi desenvolvido como parte do desafio "Treinando uma IA de Aprendizagem: Explore o Poder do NotebookLM", usando o NotebookLM como ferramenta central de organização e síntese das fontes acadêmicas ao longo de todo o fluxo de trabalho (ver seção Fluxo de Trabalho).

**Tema escolhido:** ciência da decisão de persistir ou encerrar projetos — unindo a psicologia da escalada de comprometimento (sunk cost, dissonância cognitiva, silêncio organizacional) com a ciência da persistência saudável (grit).

**Motivação:** este caderno nasceu do interesse por entender por que é tão difícil abandonar um curso de ação que já não faz sentido, despertado pela leitura de Quit: The Power of Knowing When to Walk Away, de Annie Duke. A partir dessa inquietação inicial, em vez de resumir obras de divulgação sobre o tema (material protegido por direitos autorais), fui direto às **fontes acadêmicas primárias**, construindo meu próprio caderno de estudo a partir delas — e, com isso, desenvolvi uma ferramenta de diagnóstico aplicável.

**Objetivos de estudo:**
- [x] Entender os mecanismos psicológicos por trás do *sunk cost effect* e do *escalation of commitment*
- [x] Compreender o papel da identidade, da dissonância cognitiva e do silêncio organizacional na dificuldade de encerrar algo
- [x] Mapear estratégias reais de de-escalation validadas experimentalmente
- [x] Mapear o contraponto científico: quando persistência é força (grit), não negação
- [x] Construir uma ferramenta prática (framework de decisão) aplicável a contextos reais de gestão de projeto/produto

---

## Curadoria de Fontes

| # | Fonte | Área de estudo | DOI / Link |
|---|---|---|---|
| 1* | Arkes, H. R.; Blumer, C. — "The Psychology of Sunk Cost" (1985) | Psicologia da decisão | [10.1016/0749-5978(85)90049-4](https://doi.org/10.1016/0749-5978(85)90049-4) |
| 2 | Staw, B. M. — "Knee-Deep in the Big Muddy" (1976) | Comportamento organizacional | [10.1016/0030-5073(76)90005-2](https://doi.org/10.1016/0030-5073(76)90005-2) |
| 3* | Brockner, J. et al. — "Escalation of Commitment... Effect on Self-Identity" (1986) | Comportamento organizacional | [10.2307/2392768](https://doi.org/10.2307/2392768) |
| 4* | Sleesman, D. J. et al. — "Cleaning Up the Big Muddy: A Meta-Analytic Review" (2012) | Comportamento organizacional (meta-análise) | [10.5465/amj.2010.0696](https://doi.org/10.5465/amj.2010.0696) |
| 5* | Simonson, I.; Staw, B. — "Deescalation Strategies" (1992) | Comportamento organizacional | [10.1037/0021-9010.77.4.419](https://doi.org/10.1037/0021-9010.77.4.419) |
| 6 | Wrosch, C. et al. — "Goal Disengagement in Adaptive Self-Regulation" (2003) | Motivação e bem-estar | [10.1080/15298860309021](https://doi.org/10.1080/15298860309021) |
| 7* | Duckworth, A. L. et al. — "Grit: Perseverance and Passion" (2007) | Motivação e desempenho | [10.1037/0022-3514.92.6.1087](https://doi.org/10.1037/0022-3514.92.6.1087) |
| 8 | Lucas, G. M. et al. — "When the Going Gets Tough: Grit Predicts Costly Perseverance" (2015) | Motivação e desempenho | [10.1016/j.jrp.2015.08.004](https://doi.org/10.1016/j.jrp.2015.08.004) |
| 9 | Flyvbjerg, B. et al. — "Underestimating Costs in Public Works Projects" (2002) | Estudo de caso aplicado | [10.1080/01944360208976273](https://doi.org/10.1080/01944360208976273) |
| 10 | Ross, J.; Staw, B. M. — "Organizational Escalation and Exit: Shoreham Nuclear Power Plant" (1993) | Estudo de caso aplicado | [10.2307/256756](https://doi.org/10.2307/256756) |
| 11* | Samuelson, W.; Zeckhauser, R. J. — "Status Quo Bias in Decision Making" (1988) | Psicologia da decisão | [10.1007/BF00055564](https://doi.org/10.1007/BF00055564) |

**Critério de seleção:** as 6 fontes marcadas com ⭐ formam o núcleo essencial do caderno temático — uma para cada um dos 6 fatores avaliados pela ferramenta interativa (Sunk Cost → Arkes & Blumer; Status Quo → Samuelson & Zeckhauser; Identidade → Brockner et al.; Segurança de Equipe → Sleesman et al.; Regulação Emocional → Simonson & Staw; Persistência/Grit → Duckworth et al.). As demais compõem o corpus complementar, usado para aprofundar comparações, estudos de caso reais e o contraponto científico do miniguia.

**Nota de transparência:** as fontes acima são estudos científicos originais, não textos de livros de divulgação — respeitando direitos autorais e priorizando fontes primárias com maior rigor acadêmico.

---

## Fluxo de Trabalho

```mermaid
flowchart LR
    A[Curadoria de 11 fontes] --> B[Upload no NotebookLM]
    B --> C[Exploração via Prompts em 8 componentes]
    C --> D[Auditoria contra o PDF original]
    D --> E[Registro de Cicatrizes/Troubleshooting]
    E --> F[Miniguia Final Consolidado]
    F --> G[Ferramenta Interativa: Bifurcar]
```

---

## Engenharia de Prompts e Cicatrizes

Cada prompt estratégico foi construído seguindo um framework de 8 componentes: **Instrução, Exemplos (Few-shot), Contexto/Configuração, Restrições/Limitações, Conteúdo Principal, Indicações, Formato de Saída e Conteúdo de Suporte.** Todas as respostas abaixo foram auditadas manualmente contra o PDF original das fontes antes de entrarem neste README.

### Prompt #1 — Pilar: Status Quo

| Componente | Conteúdo |
|---|---|
| **Instrução** | Explicar o "teste do reset mental" (imaginar decidir do zero, sem nada investido) como ferramenta prática derivada do conceito de viés de status quo. |
| **Exemplos (Few-shot)** | "[a ferramenta] funciona porque [mecanismo psicológico], segundo [fonte]". |
| **Contexto/Configuração** | Assistente de estudo documentando o pilar "Status Quo" de um framework de decisão sobre persistir ou encerrar projetos. |
| **Restrições/Limitações** | Não usar jargão técnico sem explicar. Resposta em até 90 palavras. Não citar exemplos fora da fonte fornecida. |
| **Conteúdo Principal** | Fonte: Samuelson, W.; Zeckhauser, R. J. (1988), "Status Quo Bias in Decision Making". |
| **Indicações** | Focar em por que as pessoas preferem manter o caminho atual mesmo sem motivo racional para isso. |
| **Formato de Saída** | Um parágrafo único, linguagem acessível a leigos. |
| **Conteúdo de Suporte** | Termos do glossário: "status quo bias", "inércia decisória". |

**Resultado obtido:** *(gerado antes da correção da fonte — ver cicatriz abaixo)*

> O teste do reset mental funciona porque neutraliza a inércia decisória — a tendência de manter o caminho atual por ser a escolha padrão, mesmo sem motivo racional —, segundo Samuelson e Zeckhauser (1988). Essa relutância em mudar decorre do viés do status quo, no qual preferimos a situação presente para evitar o custo mental da mudança. Ao imaginar decidir do zero, sem nada investido, você elimina essa trava e avalia a continuação do projeto puramente pelo seu valor futuro.

**Cicatriz/Dificuldade:** Na primeira tentativa, o "Conteúdo Principal" especificava a fonte Samuelson & Zeckhauser (1988) por nome, mas esse documento ainda não havia sido carregado no notebook — ele existia apenas como texto do prompt, não como PDF real no corpus. A resposta veio coerente, bem escrita e citando a fonte corretamente, o que tornou o problema **invisível**: nada indicava que a resposta vinha do conhecimento geral do modelo sobre um estudo famoso, e não de uma leitura real do documento. A falha só foi percebida ao auditar a lista de arquivos efetivamente carregados no notebook. A correção aplicada foi adicionar o PDF real de Samuelson & Zeckhauser como 11ª fonte do corpus. **Lição central:** pedir uma fonte específica no prompt não garante, por si só, que a resposta esteja *grounded* nela — só a lista real de documentos do notebook garante isso.

### Prompt #2 — Pilar: Segurança de Equipe

| Componente | Conteúdo |
|---|---|
| **Instrução** | Listar 3 sinais organizacionais concretos que indicam que uma equipe está sustentando uma decisão ruim por silêncio coletivo, segundo a meta-análise fornecida. |
| **Exemplos (Few-shot)** | "[sinal] indica silêncio coletivo porque [mecanismo]". |
| **Contexto/Configuração** | Assistente de estudo documentando o pilar "Segurança de Equipe" de um framework de decisão sobre persistir ou encerrar projetos. |
| **Restrições/Limitações** | Não inventar estatísticas que não estejam no documento. Se a fonte não quantificar algo, dizer isso explicitamente. Máximo 100 palavras. |
| **Conteúdo Principal** | Fonte: Sleesman, D. J. et al. (2012), "Cleaning Up the Big Muddy: A Meta-Analytic Review". |
| **Indicações** | Priorizar sinais observáveis no dia a dia de uma equipe, não conceitos abstratos. |
| **Formato de Saída** | Lista numerada de 3 itens + uma frase de fechamento prática. |
| **Conteúdo de Suporte** | Termos do glossário: "escalation of commitment", "dissenso organizacional". |

**Resultado obtido:**

> 1. Alta coesão do grupo indica silêncio coletivo porque gera conformidade de julgamento e inibe o dissenso organizacional (ρ = 0,307).
> 2. Autoridade de decisão compartilhada indica silêncio coletivo porque intensifica a pressão de autoapresentação para proteger a reputação, elevando a escalation of commitment (ρ = 0,490).
> 3. Ausência de resistência de terceiros indica silêncio coletivo porque reduz a contestação; contudo, a fonte não quantifica um efeito estatisticamente significativo para essa variável (ρ = -0,176).
>
> Para mitigar esse cenário, estabeleça revisões baseadas em processos objetivos para expor falhas sem ameaçar a reputação da equipe.

**Cicatriz/Dificuldade:** A resposta priorizou fidelidade estatística à fonte (respeitando bem a restrição de não inventar dados — os três coeficientes de correlação conferem exatamente com as Tabelas 2 e 3 do artigo original) em detrimento da linguagem cotidiana pedida em "Indicações": os fatores vieram nomeados como variáveis de pesquisa, com coeficientes técnicos, em vez de comportamentos visíveis do dia a dia de uma equipe. Isso mostra que, quando duas partes do framework pedem coisas em tensão (rigor técnico vs. acessibilidade), o modelo tende a priorizar a restrição mais explícita ("não inventar estatísticas") em vez da mais qualitativa ("focar em sinais observáveis"). Para corrigir, o prompt precisaria reforçar ainda mais o componente "Indicações", pedindo explicitamente para "traduzir cada fator estatístico em um comportamento observável numa reunião real, sem usar coeficientes ou termos técnicos".

### Prompt #3 — Pilar: Regulação Emocional

| Componente | Conteúdo |
|---|---|
| **Instrução** | Explicar por que criar distância temporal (esperar 24-48h) antes de uma decisão importante melhora sua qualidade, segundo o estudo sobre estratégias de de-escalation. |
| **Exemplos (Few-shot)** | "Esperar antes de decidir ajuda porque [mecanismo psicológico], segundo [fonte]". |
| **Contexto/Configuração** | Assistente de estudo documentando o pilar "Regulação Emocional" de um framework de decisão sobre persistir ou encerrar projetos. |
| **Restrições/Limitações** | Não recomendar prazos diferentes dos mencionados na fonte. Resposta em até 90 palavras. |
| **Conteúdo Principal** | Fonte: Simonson, I.; Staw, B. (1992), "Deescalation Strategies: A Comparison of Techniques for Reducing Commitment to Losing Courses of Action". |
| **Indicações** | Focar no mecanismo psicológico da distância temporal, não em técnicas genéricas de gestão do tempo. |
| **Formato de Saída** | Parágrafo único. |
| **Conteúdo de Suporte** | Termos do glossário: "de-escalation", "pressão emocional aguda". |

**Resultado obtido:**

> A redução da ameaça em estratégias de de-escalation melhora a qualidade decisória porque atenua a pressão emocional aguda ao diminuir a necessidade de autojustificação, segundo Simonson e Staw (1992). Esse processo reduz os custos psicológicos e sociais de reconhecer falhas, permitindo abandonar um curso de ação mal-sucedido. Contudo, a fonte analisada aborda a redução de ameaça em geral e não menciona o conceito de distância temporal nem especifica o prazo de 24 a 48 horas.

**Cicatriz/Dificuldade:** Essa foi a descoberta mais importante de todo o processo de engenharia de prompts: o NotebookLM sinalizou corretamente que a fonte **não sustenta** a afirmação específica de "24 a 48 horas" que eu já havia atribuído a Simonson & Staw (1992) na própria ferramenta interativa, antes de verificar contra o PDF real. Auditei o artigo completo e confirmei: a expressão "24 a 48 horas" e o conceito de "distância temporal" não aparecem em nenhum lugar do texto. As três técnicas de de-escalation validadas experimentalmente pelo estudo são, na verdade, **redução de ameaça**, **definição de metas mínimas** e **responsabilização pelo processo de decisão**. Como correção, removi a especificidade do prazo do texto da ferramenta em todas as variações afetadas, substituindo pelo mecanismo real de redução de ameaça sustentado pela fonte.

### Tabela-resumo de Troubleshooting Geral

| Problema encontrado | Onde apareceu | Correção aplicada |
|---|---|---|
| Fonte citada no prompt sem estar carregada no notebook (erro invisível) | Prompt #1 (Status Quo) | Auditar a lista real de documentos do notebook, não confiar apenas na citação da resposta |
| Tensão entre rigor técnico e linguagem acessível | Prompt #2 (Segurança de Equipe) | Reforçar o componente "Indicações" pedindo tradução explícita de estatísticas em comportamentos observáveis |
| Afirmação específica (prazo) atribuída à fonte errada, sem verificação prévia | Prompt #3 (Regulação Emocional) | Auditoria manual do PDF completo antes de publicar qualquer dado específico atribuído a uma fonte |

---

## Miniguia de Estudo Final

### Resumos Estruturados por Subtema

#### A. Vieses Cognitivos e Psicológicos na Manutenção de Decisões
- **Efeito do Custo Afundado (*Sunk Cost Effect*):** tendência de continuar investindo em um empreendimento simplesmente porque recursos de tempo, dinheiro ou esforço já foram aplicados. A motivação central é o desejo de não parecer esbanjador ou evitar a dor de admitir que os recursos foram desperdiçados. Sob a Teoria da Perspectiva, perdas certas são altamente aversivas, levando o tomador de decisão a assumir riscos adicionais na esperança de reverter o cenário.
- **Viés do Status Quo (*Status Quo Bias*):** preferência desproporcional por manter a situação atual ou a opção padrão, alimentada pela inércia, pela percepção de custos de transição e pela evitação do arrependimento — decisões ativas de mudança geram maior remorso em caso de falha do que a inação.

#### B. Determinantes Organizacionais e Modelo Temporal de Escalada
- **Categorias de Determinantes:** a escalada do comprometimento resulta do encadeamento de forças de *projeto* (custos de encerramento e valor de salvamento), *psicológicas* (autojustificação), *sociais* (autoapresentação e aprovação pública) e *estruturais* (problemas de agência).
- **Estratégias de Saída:** a desistência de projetos falhos é facilitada pela substituição da liderança do projeto (removendo os gatilhos de autojustificação) e pela **desinstitucionalização** do projeto — separando-o fisicamente ou tornando-o periférico aos objetivos centrais da empresa, conforme documentado no estudo de caso real da Usina Nuclear de Shoreham (Ross & Staw, 1993).

#### C. Estratégias Práticas de Desescalada (*De-escalation*)
- **Redução de Ameaça:** diminuir as penalidades e o impacto reputacional associados ao insucesso reduz a necessidade defensiva do gestor de salvar o projeto a qualquer custo.
- **Definição de Metas Mínimas (*Goal Setting*):** estabelecer critérios e limites mínimos de desempenho antes do término do projeto força o reconhecimento da falha e aciona mudanças de rota ou cancelamentos estratégicos.
- **Responsabilização pelo Processo (*Process Accountability*):** avaliar os decisores pela qualidade e rigor do processo analítico, e não apenas pelo resultado final do investimento, incentiva a precisão decisória e atenua a autojustificação.

#### D. Perseverança Produtiva vs. Persistência Custosa (*Grit*)
- **Conceito de Garra (*Grit*):** perseverança e paixão por objetivos de longo prazo, com foco na estamina e no esforço contínuo ao longo de anos.
- **Lado Sombrio do Grit:** diante de cenários de falha iminente, indivíduos com elevado grit podem insistir excessivamente em tarefas inviáveis, gastando recursos extras em vez de cortar prejuízos no momento oportuno.

### Glossário

| Termo | Definição |
|---|---|
| Escalation of Commitment (Escalada do Comprometimento) | Padrão comportamental em que um indivíduo ou grupo mantém ou aumenta o aporte de recursos em um curso de ação com feedbacks nitidamente negativos. |
| Sunk Cost Effect (Efeito do Custo Afundado) | Falha de julgamento em que investimentos passados irrecuperáveis motivam a continuidade de um projeto. |
| Status Quo Bias (Viés do Status Quo) | Tendência sistemática de aderir à decisão atual ou à alternativa padrão, desconsiderando opções potencialmente superiores. |
| De-escalation (Desescalada) | Conjunto de técnicas organizacionais para reduzir o comprometimento com projetos falhos e redirecionar recursos de forma racional. |
| Process Accountability (Responsabilização pelo Processo) | Modelo de avaliação focado no rigor e na qualidade da análise decisória, reduzindo defesas reputacionais. |
| Goal Substitution Effect (Substituição de Metas) | Fenômeno no qual o objetivo de concluir a entrega física do projeto substitui as metas econômicas ou estratégicas originais à medida que o projeto se aproxima do fim. |
| Deinstitutionalization (Desinstitucionalização) | Processo de desacoplamento entre um projeto e a identidade ou valores essenciais de uma organização, facilitando o encerramento da iniciativa. |
| Grit (Garra) | Traço de personalidade que combina paixão e estamina para a busca de metas de longo prazo perante adversidades. |

### Prompts Reutilizáveis para Revisão de Projetos

> **Prompt 1 — Teste do Reset Mental (Viés de Status Quo):**
> "Imagine que o projeto [Nome do Projeto] não existe hoje e não temos nenhum valor de tempo ou dinheiro investido nele. Olhando apenas para o cenário atual e projeções futuras, nós escolheríamos iniciar este projeto hoje exatamente como ele está? Se a resposta for 'não', quais fatores não econômicos estão impedindo o encerramento?"

> **Prompt 2 — Auditoria de Justificação e Substituição de Metas:**
> "Ao avaliar a continuidade do projeto [Nome do Projeto], nós estamos buscando alcançar o valor estratégico/financeiro original ou estamos apenas tentando evitar a frustração de admitir perdas passadas / entregar o projeto só porque está perto de acabar?"

> **Prompt 3 — Estabelecimento de Limites Inegociáveis (Goal Setting de Desescalada):**
> "Quais são os 3 indicadores mínimos e objetivos de desempenho do projeto [Nome do Projeto] que, caso não sejam atingidos até [Data X], acionarão automaticamente a interrupção definitiva das atividades sem necessidade de novas justificativas?"

---

## Ferramenta Interativa: Bifurcar

O miniguia inclui uma ferramenta interativa chamada **Bifurcar**, com 7 perguntas (1 de contexto + 6 avaliativas), cada uma mapeada a um dos 6 pilares do corpus essencial acima. Ao final, a ferramenta indica se o cenário pede **Reavaliar** ou **Considerar encerrar**, com um resumo textual que cita a fonte científica mais relevante de acordo com o padrão de respostas.

**Recursos incorporados ao longo do desenvolvimento:**
- Textos com 3 variações de intensidade por pilar (leve, moderado, forte), evitando repetição de conclusão entre respostas diferentes
- Mecanismo de desempate que devolve a decisão ao próprio usuário quando as respostas empatam, com frases próprias (não repetidas das perguntas originais)
- Reflexão baseada em grit (Duckworth et al., 2007) quando o único sinal de alerta aparece isolado dentro de um quadro geral tranquilo — exceto quando o próprio pilar de Persistência é o sinal isolado, para evitar uma citação circular
- Todo o conteúdo textual foi auditado manualmente contra os PDFs originais das fontes, com correções aplicadas sempre que uma afirmação não era sustentada pela fonte citada

**Acesse a ferramenta:** [marsielo-marcos.github.io/Framework_de_Decisao-Baseado_em_Ciencia_Comportamental/bifurcar.html](https://marsielo-marcos.github.io/Framework_de_Decisao-Baseado_em_Ciencia_Comportamental/bifurcar.html)

---

## Lições Aprendidas

1. Curadoria de fontes primárias, em vez de obras de divulgação, fortalece a credibilidade científica do material sem abrir mão de acessibilidade.
2. Engenharia de prompts estruturada (8 componentes) reduz respostas genéricas — mas não substitui a auditoria manual: mesmo prompts bem construídos podem citar fontes não carregadas ou gerar afirmações plausíveis, porém não sustentadas.
3. Transformar um estudo teórico em ferramenta aplicável exige decisões de design (categorias, limiares, desempates) tão importantes quanto o conteúdo científico em si — e revisar essas decisões continuamente é parte do processo, não uma etapa única.

---

## Licenciamento e Uso

Este repositório foi desenvolvido como projeto de estudo e prova de conceito para o Desafio de Projeto da [DIO](https://www.dio.me/).

- **Conteúdo educacional** (resumos, glossário, curadoria de fontes, prompts reutilizáveis): licenciado sob **CC BY 4.0** — veja [LICENSE-CONTENT.md](./LICENSE-CONTENT.md). Uso e adaptação livres, inclusive comercial, mediante atribuição a Marcelo Marcos Pinheiro.
- **Lógica da ferramenta e algoritmo de pontuação**: todos os direitos reservados. © 2026 Marcelo Marcos Pinheiro. Este repositório **não** possui uma licença de código aberto — nenhum uso, cópia, modificação ou distribuição do código da ferramenta é permitido sem autorização prévia por escrito do autor.
- Este projeto pode evoluir futuramente para um produto/SaaS independente. A publicação neste repositório não constitui cessão de direitos sobre a ideia, marca ou lógica de negócio associada.

Para dúvidas sobre uso ou parcerias, entre em contato via https://www.linkedin.com/in/marcelo-marcos-pinheiro-941b57b8

---

*Projeto desenvolvido para o Desafio de Projeto da [DIO](https://www.dio.me/) — Caderno Temático com NotebookLM.*
