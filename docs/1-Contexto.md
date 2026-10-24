# Introdução

O Terceiro Setor exerce papel fundamental na mitigação das desigualdades socioeconômicas e no apoio direto a populações em extrema vulnerabilidade social. Organizações Não Governamentais (ONGs), projetos comunitários e entidades beneficentes mobilizam diariamente recursos essenciais, como alimentos, vestuário e itens de higiene, para famílias em situação de risco. Empresas de outros setores também realizam esse tipo de ação social, doando produtos e recursos para instituições e comunidades em vulnerabilidade como parte de suas iniciativas de responsabilidade social. No entanto, tanto essas instituições quanto as empresas costumam operar com recursos humanos limitados e infraestrutura administrativa rudimentar, controlando doações e cadastros sociais por meio de anotações físicas, aplicativos de mensagens e planilhas desconectadas entre si. Esse cenário reduz o alcance e a eficiência logística das iniciativas solidárias.
 
Diante desse contexto, o **BENEFAC** é proposto como uma plataforma web para a centralização, automação e governança da gestão de doações e distribuição de benefícios assistenciais, podendo ser utilizada tanto por instituições do Terceiro Setor quanto por empresas de outros setores, cobrindo o ciclo completo do processo: doação, triagem socioeconômica, controle de estoque e comprovação de entrega aos beneficiados.
 
O projeto se conecta diretamente a duas metas da Agenda 2030 da Organização das Nações Unidas (ONU, 2015). A **ODS 1 — Erradicação da Pobreza** tem como meta acabar com a pobreza em todas as suas formas e em todos os lugares, garantindo que pessoas em situação de vulnerabilidade tenham acesso a recursos básicos e proteção social (ONU, 2015); o BENEFAC contribui para esse objetivo ao tornar mais ágil e confiável a distribuição de benefícios às famílias assistidas. Já a **ODS 2 — Fome Zero e Agricultura Sustentável** busca acabar com a fome, alcançar a segurança alimentar, melhorar a nutrição e promover a agricultura sustentável (ONU, 2015); ao reduzir o desperdício de doações e otimizar o controle de estoque de itens perecíveis, o sistema apoia diretamente essa meta.
 
**Fontes:**
* ORGANIZAÇÃO DAS NAÇÕES UNIDAS (ONU). *Transformando Nosso Mundo: A Agenda 2030 para o Desenvolvimento Sustentável*. Brasília: ONU Brasil, 2015. Disponível em: <https://brasil.un.org/pt-br/91863-agenda-2030-para-o-desenvolvimento-sustentável>. Acesso em: 11 set. 2026.
* ORGANIZAÇÃO DAS NAÇÕES UNIDAS (ONU). *Objetivos de Desenvolvimento Sustentável no Brasil*. Disponível em: <https://brasil.un.org/pt-br/sdgs>. Acesso em: 11 set. 2026.

## Problema
A condução manual e fragmentada dos processos de doação gera gargalos operacionais recorrentes nas instituições do Terceiro Setor e nas empresas que realizam ações sociais:
 
* Falta de controle em tempo real dos estoques de donativos;
* Desperdício ou vencimento de itens perecíveis por ausência de rastreabilidade;
* Morosidade na triagem das solicitações de auxílio;
* Duplicidade na concessão de benefícios a um mesmo beneficiado, em detrimento de outros ainda não atendidos;
* Ausência de mecanismos transparentes de prestação de contas, o que desestimula a fidelização de doadores recorrentes;
* Falta de indicadores consolidados para o planejamento de novas campanhas assistenciais.
Esses problemas ocorrem no contexto de instituições e empresas que, majoritariamente, não possuem sistemas informatizados dedicados, dependendo de ferramentas genéricas (planilhas, aplicativos de mensagens) que não foram desenhadas para esse tipo de operação.



## Objetivos

### Objetivo Geral
 
Desenvolver uma plataforma web para automatizar e integrar os processos de registro de doações, controle de estoque de donativos, triagem de solicitações de benefícios e agendamento/comprovação de entregas aos beneficiados, na área de Sistemas de Informação.
 
### Objetivos Específicos
 
* Digitalizar o ciclo de doação, permitindo a correspondência direta entre as necessidades urgentes da instituição e os donativos oferecidos por pessoas físicas e jurídicas;
* Implementar o módulo de triagem e validação dos produtos recebidos quanto a nível de qualidade e quantidade;
* Automatizar a baixa de estoque e o registro comprobatório da distribuição/entrega final das doações aos beneficiados.
 

## Justificativa

A implementação do BENEFAC reduz significativamente o tempo médio entre o recebimento da doação e a entrega efetiva do benefício ao beneficiado. Do ponto de vista administrativo, o sistema mitiga erros manuais de contagem, evita o desperdício de insumos essenciais e concede total rastreabilidade aos itens doados — do recebimento até a entrega final.
 
Em termos sociais e estratégicos, a ferramenta fortalece a transparência institucional, tende a atrair maior volume de doadores recorrentes e municia os gestores com dados analíticos fundamentais para mensurar o impacto social das campanhas realizadas, apoiando diretamente a prestação de contas exigida por doadores e órgãos de fiscalização do Terceiro Setor e das empresas parceiras.


## Público-Alvo

O BENEFAC é destinado a instituições do Terceiro Setor (ONGs, projetos comunitários, entidades beneficentes) e a empresas de outros setores que realizam ações sociais e precisam gerenciar suas doações e a distribuição de benefícios de forma centralizada.
 
Dentro dessas organizações, o sistema atende três perfis principais de usuários, identificados a partir da análise dos processos de negócio:
 
* **Doadores (pessoas físicas ou jurídicas)**: público entre 18 e 70 anos, com uso predominante de smartphone, que busca praticidade no ato de doar e transparência sobre o destino final da doação;
* **Estoquistas/Voluntários**: público entre 18 e 55 anos, com perfil operacional e dinâmico, que utiliza dispositivos móveis ou tablets no local de recepção das doações para conferência e controle físico dos itens;
* **Gestores/Coordenadores Gerais**: público entre 30 e 65 anos, com foco estratégico e analítico, responsável pela criação e monitoramento de campanhas, gestão de permissões de acesso e emissão de relatórios de transparência.
Esses perfis apresentam níveis distintos de familiaridade com tecnologia, o que reforça a necessidade de uma interface simples para o doador, ágil e operacional para o estoquista, e analítica/gerencial para o gestor.

