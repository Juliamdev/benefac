## 3. Modelagem dos Processos de Negócio

Os processos de negócio do BENEFAC foram identificados a partir do ciclo completo da doação da criação da campanha até a entrega ao beneficiado, e classificados conforme sua função na cadeia de valor da instituição:
 
**Processos Primários**:
* **P1 — Gestão de Campanhas de Doação**
* **P2 — Recebimento e Entrada em Estoque**
* **P3 — Distribuição de Benefícios**
* **P4 — Gestão de Usuários e Permissões**
* **P5 — Acompanhamento, Indicadores e Transparência**
 
| Processo | Classificação | Entradas | Saídas | Onde ocorre | Participantes | Produto de Informação |
|---|---|---|---|---|---|---|
| P1 — Gestão de Campanhas de Doação | Primário | Dados da campanha (nome, objetivo, datas de início e fim, produtos necessários, pontos de coleta) | Campanha publicada, editada ou encerrada; notificação aos doadores no encerramento da campanha | Plataforma web, acessada pelo gestor | Gestor, Doador (participante externo), Sistema | Registro de campanha; produtos necessários; pontos de coleta |
| P2 — Recebimento e Entrada em Estoque | Primário | Itens físicos doados; dados do doador; campanha relacionada | Registro de recebimento criado; saldo de estoque atualizado | Galpão/sede da instituição | Estoquista, Sistema | Registro de recebimento; saldo de estoque atualizado |
| P3 — Distribuição de Benefícios | Primário | Solicitações de assistência aprovadas; saldo de itens disponíveis em estoque | Produtos entregues; comprovante de entrega; saldo de estoque abatido | Galpão/sede ou ponto de retirada combinado | Estoquista, Sistema | Registro de entrega; comprovante digital |
| P4 — Gestão de Usuários e Permissões | Suporte | Dados cadastrais dos colaboradores e demais usuários | Perfis e permissões de acesso configurados | Plataforma web (área administrativa) | Gestor, Sistema | Cadastro de usuários e perfis de acesso |
| P5 — Acompanhamento, Indicadores e Transparência | Gerencial | Dados consolidados de doações, estoque e entregas | Painel de indicadores; relatórios de transparência | Plataforma web (painel do gestor) | Gestor, Sistema | Relatórios de impacto |

### 3.1. Modelagem da situação atual (Modelagem AS IS)

Atualmente, a maior parte das instituições do Terceiro Setor e das empresas que realizam ações sociais conduz o ciclo da doação de forma manual e fragmentada, sem o apoio de um sistema dedicado. O registro de interesse em doar costuma ocorrer por meio de grupos de WhatsApp, redes sociais ou contato telefônico direto com a instituição, sem nenhum controle formal — o que faz com que doações combinadas informalmente às vezes nem cheguem a se concretizar, e que o doador não tenha nenhum retorno sobre o destino do que ofereceu.
 
No recebimento, a conferência dos itens é feita visualmente, e o controle de estoque é mantido em cadernos ou planilhas eletrônicas desconectadas entre si, atualizadas manualmente pelo estoquista ao final do expediente. Essa defasagem entre o recebimento físico e o registro gera divergências frequentes entre o que existe fisicamente no galpão e o que consta nos controles da instituição, além de dificultar a identificação de itens perecíveis próximos do vencimento.
 
A triagem das solicitações de assistência e a definição de quem será atendido também seguem critérios pouco padronizados, muitas vezes baseados na ordem de chegada ou no conhecimento informal da equipe sobre as famílias da região — o que aumenta o risco de duplicidade no atendimento (a mesma família recebendo o mesmo benefício mais de uma vez) e de famílias com necessidades mais urgentes não serem priorizadas. A confirmação da entrega ao beneficiado raramente é registrada de forma padronizada, dificultando a comprovação posterior.
 
Por fim, a geração de relatórios para prestação de contas a doadores e parceiros é feita manualmente a partir das planilhas de controle, consumindo tempo da coordenação e resultando em indicadores desatualizados, o que compromete a transparência da instituição e o planejamento de novas campanhas.
 
O BENEFAC propõe substituir esse conjunto de controles paralelos por um fluxo único e centralizado: o doador consulta as campanhas, os produtos necessários e os pontos de coleta diretamente na plataforma; o estoquista confirma o recebimento em um único registro, que já atualiza o estoque em tempo real; a distribuição aos beneficiados é reservada e confirmada no sistema, gerando comprovante digital; e os indicadores e relatórios de transparência são gerados automaticamente a partir desses registros, sem a necessidade de consolidação manual.

### 3.2. Descrição geral da proposta (Modelagem TO BE)

A proposta do BENEFAC é concentrar, em uma única plataforma web, as três etapas do ciclo primário da doação (campanhas, recebimento/estoque e distribuição) junto com o acompanhamento gerencial desse ciclo, eliminando os controles paralelos hoje mantidos em planilhas, cadernos e aplicativos de mensagens. O processo de apoio **Gestão de Usuários e Permissões** (P4) não é detalhado em um modelo TO-BE próprio nesta seção por ser um processo transversal, comum a qualquer sistema com múltiplos perfis de acesso — seus requisitos já estão descritos na [Especificação do Projeto](./2-Especificação.md).
 
Como limite da proposta, o sistema não automatiza a etapa de transporte físico das doações (coleta, entrega por terceiros), que segue sendo uma atividade executada pela equipe da instituição; o papel do sistema é registrar e controlar essa etapa, não executá-la. A proposta está diretamente alinhada ao objetivo geral do projeto — automatizar e integrar o registro de doações, o controle de estoque, a triagem de solicitações e a comprovação de entregas — e às ODS 1 e 2 apresentadas na Documentação de Contexto, na medida em que reduz o tempo de atendimento às famílias e o desperdício de itens perecíveis.

### 3.3. Modelagem dos processos



[Processo 1 – GESTÃO DE CAMPANHAS DE DOAÇÃO](./processos/processo-1-nome-do-processo.md "Detalhamento do Processo 1.")

[Processo 2 – RECEBIMENTO E ENTRADA EM ESTOQUE](./processos/processo-2-nome-do-processo.md "Detalhamento do Processo 2.")

[PROCESSO 3 - Nome do Processo](./processos/processo-3-nome-do-processo.md "Detalhamento do Processo 3.")

[Processo 4 – GESTÃO DE USUÁRIOS E PERMISSÕES](./processos/processo-4-nome-do-processo.md "Detalhamento do Processo 4.")

[Processo 5 – ACOMPANHAMENTO, INDICADORES E TRANSPARÊNCIA](./processos/processo-5-nome-do-processo.md "Detalhamento do Processo 5.")
