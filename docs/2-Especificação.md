# Especificações do Projeto

<span style="color:red">Pré-requisitos: <a href="01-Documentação de Contexto.md"> Documentação de Contexto</a></span>

Definição do problema e ideia de solução a partir da perspectiva do usuário. É composta pela definição do  diagrama de personas, histórias de usuários, requisitos funcionais e não funcionais além das restrições do projeto.

Esta seção reúne as personas da solução, as histórias de usuário construídas a partir delas e os requisitos funcionais, não funcionais e restrições derivados dessas histórias, cobrindo tanto instituições do Terceiro Setor quanto empresas de outros setores que utilizem o BENEFAC para gerenciar suas doações.

## Personas

**1. Mariana Oliveira | Doadora**
Mariana Oliveira tem 28 anos, é analista administrativa e trabalha em uma empresa de médio porte. Ela gosta de participar de ações sociais e costuma contribuir com instituições por meio de doações de alimentos, roupas, produtos de higiene e outros item necessários. Maria utiliza a internet frequentemente para realizar atividades do dia a dia e está acostumada a utilizar plataformas web para realizar cadastros, consultar informações e acompanhar serviços. Ao realizar uma doação, ela procura instituições e campanhas que transmitam segurança, otimização e transparência. Uma das suas principais preocupações é não saber exatamente o que acontece com os produtos depois que são doados. Por isso, ela gostaria de criar uma conta na plataforma, fazer login e utilizá-la para consultar campanhas, verificar quais produtos são necessários e acompanhar o destino dos itens doados.

**Objetivos**
Encontrar campanhas sociais confiáveis;
Identificar quais produtos as instituições estão necessitando;
Realizar doações de maneira simples;
Encontrar um ponto de coleta adequado;
Acompanhar o andamento de sua doação;
Saber para onde os produtos foram destinados;
Ter maior transparência sobre as ações realizadas pela instituição.

**Necessidades**
Consultar campanhas disponíveis;
Visualizar informações detalhadas das campanhas;
Escolher um ponto de coleta;
Consultar o status da doação;
Acompanhar o destino dos itens doados.

**Dificuldades**
Não saber quais produtos as instituições precisam;
Falta de informações sobre campanhas;
Dificuldade para acompanhar o destino das doações;
Falta de transparência sobre a utilização dos itens;

**Perfil tecnológico**
Mariana possui facilidade para utilizar a internet e serviços digitais. Acessa sites por computador, notebook ou smartphone e espera encontrar uma plataforma web responsiva, intuitiva e de fácil navegação.

**2. Carlos Henrique | Estoquista**
Carlos Henrique tem 41 anos e trabalha como responsável pelo recebimento e organização das doações em uma  instituição social. Sua rotina envolve receber os produtos doados, conferir as mercadorias, registrar a entrada e organizar o estoque, além de acompanhar a saída dos produtos destinados aos beneficiados. Carlos precisa de uma ferramenta que facilite o controle dos produtos, pois os registros manuais podem gerar erros, informações duplicadas ou dificuldades para identificar a quantidade real de itens disponíveis. Ele utiliza computadores, notebooks, ou tablets durante suas atividades e precisa que a plataforma seja objetiva, permitindo realizar os registros rapidamente durante o recebimento e a distribuição das doações.

**Objetivos**
Organizar as doações recebidas;
Manter o estoque atualizado;
Evitar erros nos registros;
Controlar a entrada e saída de produtos;
Identificar os produtos disponíveis;
Registrar a entrega das doações.

**Necessidades**
Registrar mercadorias recebidas;
Conferir os produtos;
Registrar entradas no estoque;
Registrar baixas e saídas;
Consultar a quantidade de produtos disponíveis;
Registrar a confirmação da entrega ao beneficiado.

**Dificuldades**
Controle manual dos produtos;
Possibilidade de divergência entre o estoque físico e os registros;
Dificuldade para localizar informações;
Falta de atualização imediata do estoque;
Risco de esquecer ou duplicar registros de entrada e saída.

**Perfil tecnológico**
Carlos possui conhecimento básico a intermediário em informática e utiliza sistemas web no ambiente de trabalho. Precisa de uma plataforma simples, objetiva e rápida, que possa ser acessada pelo navegador em computador, notebook ou tablet.

**3. Juliana Martins | Gestora/Coordenadora Geral**
Juliana Martins tem 35 e atua como gestora e coordenadora geral de uma instituição social. Ela é responsável pelo planejamento das campanhas, acompanhamento das doações, gerenciamento dos usuários e supervisão das atividades realizadas pela instituição. Juliana precisa ter uma visão ampla do funcionamento da organização. Para isso, necessita acompanhar informações como quantidade de doações recebidas, produtos disponíveis, campanhas ativas, beneficiados atendidos e resultados obtidos. Além disso, ela considera fundamental que a instituição consiga demonstrar aos doadores e parceiros como as doações foram utilizadas. Dessa forma, relatórios e indicadores são importantes para a transparência e prestação de contas.

**Objetivos**
Criar campanhas solidárias;
Acompanhar o desempenho das campanhas;
Monitorar as doações recebidas;
Encontrar um ponto de coleta adequado;
Acompanhar o estoque;
Gerenciar os usuários da plataforma;
Controlar permissões de acesso;
Obter indicadores sobre os atendimentos;
Emitir relatórios;
Garantir transparência na utilização das doações.

**Necessidades**
Criar e editar campanhas;
Ativar ou encerrar campanhas;
Acompanhar as doações;
Consultar informações do estoque;
Gerenciar usuários;
Definir permissões de acesso;
Visualizar métricas;
Emitir relatórios de transparência.

**Dificuldades**
Falta de centralização das informações;
Utilização de planilhas e registros manuais;
Dificuldade para acompanhar todas as doações;
Falta de indicadores atualizados;
Dificuldade para gerar relatórios;
Falta de controle sobre os diferentes níveis de acesso dos usuários.

**Perfil tecnológico**
Juliana possui conhecimento intermediário em informática e utiliza principalmente computador ou notebook para atividades administrativas. Necessita de uma plataforma web organizada, intuitiva e com dashboards, indicadores e relatórios, facilitando a tomada de decisões.

## Histórias de Usuários
As Histórias de Usuário foram elaboradas com base nas necessidades e objetivos das personas definidas para a solução. Elas descrevem, de forma simples e objetiva, as principais funcionalidades que a Plataforma Web de Gestão de Doações para Instituições Sociais e Empresas Privadas deve oferecer, considerando as necessidades dos usuários e os benefícios esperados. As histórias foram organizadas por contextos, facilitando a identificação dos requisitos e a compreensão dos principais fluxos da aplicação. Os contextos abordados incluem cadastro e acesso, campanhas de doação, registro e acompanhamento das doações, controle de estoque, beneficiários e distribuição, gestão de usuários e permissões, além de indicadores e relatórios.

Com base na análise das personas forma identificadas as seguintes histórias de usuários:

**1.Cadastro e acesso**
| EU COMO... `PERSONA`           | QUERO/PRECISO ... `FUNCIONALIDADE` | PARA ... `MOTIVO/VALOR`                        |
|--------------------------------|------------------------------------|------------------------------------------------|
| Doador                         | Criar uma conta na plataforma      | Poder realizar e acompanhar minhas doações     |
| Doador                         | Realizar login                     | Acessar minha conta e minhas informações       |
| Estoquista                     | Realizar login                     | Acessar o sistema e registrar as movimentações sob sua responsabilidade |
| Gestor/Coordenador Geral       | Realizar login                     | Permitir que possam administrar contas         |
| Gestor/Coordenador Geral       | Cadastrar usuários da instituição  | Permitir acesso à plataforma aos colaboradores |

**2.Campanhas de doação**
| EU COMO... `PERSONA`       | QUERO/PRECISO ... `FUNCIONALIDADE` | PARA ... `MOTIVO/VALOR`                                |
|----------------------------|------------------------------------|--------------------------------------------------------|
| Doador                     | Consultar campanhas vigentes       | Encontrar uma campanha que eu possa apoiar             |
| Doador                     | Ver os detalhes da campanha        | Conhecer o objetivo e as necessidades da campanha      |
| Doador                     | Consultar os produtos necessários  | Saber quais itens a instituição precisa receber        |
| Gestor/Coordenador Geral   | Criar campanhas de doação          | Divulgar as necessidades da instituição                |
| Gestor/Coordenador Geral   | Editar campanha                    | Manter as informações das campanhas atualizadas        |
| Gestor/Coordenador Geral   | Encerrar campanha                  | Informar que os objetivos da campanha foram alcançados |
| Gestor/Coordenador Geral   | Acompanhar as campanhas            | Verificar os resultados das ações realizadas           |

**3. Acompanhamento das doações**
| EU COMO... `PERSONA`         | QUERO/PRECISO ... `FUNCIONALIDADE`  | PARA ... `MOTIVO/VALOR`                              |
|-----------------------------|--------------------------------------|------------------------------------------------------|
| Doador                      |	Visualizar os pontos de coleta	     | Saber onde entregar a doação                         |
| Doador	                     | Consultar minhas doações             |	Acompanhar minhas contribuições                      |
| Doador	                     | Acompanhar o status da doação        |	Saber se foi recebida                                |
| Doador	                     | Consultar o destino da doação	       | Saber onde foi utilizada                             |
| Gestor/Coordenador Geral    |	Consultar as doações recebidas	      | Acompanhar as contribuições                          |

**4. Controle de estoque**
| EU COMO... `PERSONA`         | QUERO/PRECISO ... `FUNCIONALIDADE`   | PARA ... `MOTIVO/VALOR`                             |
|------------------------------|--------------------------------------|-----------------------------------------------------|
| Estoquista                   |	Registrar o recebimento das doações (conferência e entrada dos itens em um único registro)              |	Atualizar o estoque com os produtos recebidos                     |
| Estoquista	                  | Consultar o estoque	                 | Saber os produtos disponíveis                       |
| Estoquista                   | 	Registrar a saída dos produtos	     | Atualizar o estoque                                 |
| Estoquista                   | 	Registrar a entrega dos produtos    |	Confirmar a entrega                                 |

**5. Beneficiados e distribuição**
| EU COMO... `PERSONA`         | QUERO/PRECISO ... `FUNCIONALIDADE`     | PARA ... `MOTIVO/VALOR`                           |
|------------------------------|----------------------------------------|---------------------------------------------------|
| Estoquista	                  | Registrar produtos para as campanhas corretas |	Controlar os itens destinados                     |
| Estoquista	                  | Registrar a entrega ao beneficiado	   | Confirmar o atendimento                           |
| Gestor/Coordenador Geral	    | Consultar beneficiados atendidos       |  Acompanhar as ações sociais                      |
| Gestor/Coordenador Geral     |	Consultar o histórico de distribuições	| Acompanhar o destino das doações                  |

**6. Gestão de usuários e permissões**
| EU COMO... `PERSONA`         | QUERO/PRECISO ... `FUNCIONALIDADE`   | PARA ... `MOTIVO/VALOR`                             |
|------------------------------|--------------------------------------|-----------------------------------------------------|
|Gestor/Coordenador Geral      |	Consultar usuários cadastrados       |	Controlar os usuários                               |
|Gestor/Coordenador Geral     	| Alterar permissões de acesso         |	Definir os acessos                                  |
|Gestor/Coordenador Geral      |	Editar dados dos usuários	           | Manter os cadastros atualizados                     |
|Gestor/Coordenador Geral	     | Desativar usuários	                  | Impedir acessos indevidos                           |
|Gestor/Coordenador Geral	     | Consultar atividades dos usuários    |	Acompanhar as operações                             |

**7. Indicadores e relatórios**
| EU COMO... `PERSONA`         | QUERO/PRECISO ... `FUNCIONALIDADE`   | PARA ... `MOTIVO/VALOR`                             |
|------------------------------|--------------------------------------|-----------------------------------------------------|
|Gestor/Coordenador Geral	     | Visualizar quantidade de doações     |	Acompanhar os resultados                            |
|Gestor/Coordenador Geral      |	Visualizar produtos recebidos	       | Conhecer os itens arrecadados                       |
|Gestor/Coordenador Geral      |	Visualizar produtos distribuídos     |	Acompanhar as doações                               |
|Gestor/Coordenador Geral	     | Visualizar campanhas atendidas       |	Avaliar o impacto das ações                         |
|Gestor/Coordenador Geral      |	Emitir relatórios de doações         |	Facilitar a prestação de contas                     |
|Gestor/Coordenador Geral      |	Emitir relatórios de distribuição    |	Mostrar o destino das doações                       |
|Gestor/Coordenador Geral      |	Visualizar indicadores das campanhas |	Auxiliar nas decisões                               |






## Requisitos

As tabelas que se seguem apresentam os requisitos funcionais e não funcionais que detalham o escopo do projeto. Para determinar a prioridade de requisitos, aplicar uma técnica de priorização de requisitos e detalhar como a técnica foi aplicada.

### Requisitos Funcionais

|ID    | Descrição do Requisito  | Prioridade |
|------|-----------------------------------------|----|
|RF-001| O sistema deve permitir o cadastro de usuários e a atribuição de perfis de acesso específicos, abrangendo as funções de Doador, Estoquista e Gestor. O beneficiado não possui login nem perfil de acesso: seus dados são registrados pelo Estoquista no momento da solicitação de assistência.  | ALTA | 
|RF-002| O sistema deve fornecer permissões de acesso diferenciadas com base no perfil do usuário, cabendo ao Gestor Geral o gerenciamento dessas permissões.   | ALTA |
|RF-003| O sistema deve permitir que o Doador consulte as campanhas solidárias vigentes.   | MÉDIA |
|RF-004| O sistema deve permitir que o Estoquista registre a doação recebida, unificando a conferência e a entrada de um ou mais itens em um único registro — informando nome do item, categoria (alimentos, higiene ou vestuário), quantidade, estado de conservação e validade (em caso de produto perecível) —, atualizando automaticamente o saldo do estoque em tempo real.   | ALTA |
|RF-005| O sistema deve permitir que o Estoquista registre a saída de produtos do estoque e consulte a quantidade de itens disponíveis a qualquer momento.   | ALTA |
|RF-006| O sistema deve fornecer um Painel de Controle (Dashboard) para que o Gestor Geral visualize e controle as campanhas apoiadas.   | BAIXA |
|RF-007| O sistema deve permitir que o Estoquista reserve os itens no estoque conforme as solicitações aprovadas e registre a retirada e a entrega.   | MEDIA |
|RF-008| No ato da distribuição, o sistema deve validar a entrega e coletar um comprovante ou assinatura digital para validar a entrega, contendo data e hora da entrega, itens e quantidades entregues, identificação do beneficiado e do responsável pela entrega.   | MÉDIA |
|RF-009| O sistema deve abater definitivamente o saldo no estoque e alterar o status da entrega para "Entregue" após a confirmação do repasse ao beneficiado.   | ALTA |
|RF-010| O sistema deve manter um histórico detalhado dos lotes de itens doados com as respectivas entregas efetuadas.   | MÉDIA |
|RF-011| O sistema deve enviar automaticamente uma notificação ou recibo ao doador original, apenas na conclusão da campanha, informando que seus itens atenderam com sucesso um beneficiado, concluindo o ciclo.   | ALTA |


### Requisitos não Funcionais

|ID     | Descrição do Requisito  |Prioridade |
|-------|-------------------------|----|
|RNF-001| A interface da plataforma web deve ser totalmente responsiva, garantindo operação adequada em smartphones, tablets e desktops, para atender à mobilidade de doadores e estoquistas. | ALTA | 
|RNF-002| O sistema deve implementar controle de acesso baseado em perfis de usuário (Doador, Estoquista e Gestor), restringindo funcionalidades e dados de acordo com a permissão de cada papel. |  ALTA |
|RNF-003| O sistema deve processar a entrada e baixa de donativos de forma a atualizar o saldo de estoque em tempo real, evitando divergências físicas e garantindo o fluxo contínuo da logística. |  ALTA |
|RNF-004| A interface voltada para o doador deve possuir navegação simplificada e acessível, considerando que este público abrange idades de 18 a 70 anos com níveis distintos de familiaridade tecnológica. |  MÉDIA |
|RNF-005| O banco de dados deve proteger informações sensíveis cadastradas na tabela de usuários (como CPF, CNPJ, telefone, e-mail e senhas), utilizando criptografia adequada para garantir a privacidade dos envolvidos. |  ALTA |
|RNF-006| O sistema deve possibilitar a rastreabilidade integral dos dados, correlacionando de forma imutável os lotes de doação recebidos com os registros de entrega e comprovantes digitais gerados aos beneficiados. |  ALTA |
|RNF-007| A emissão de relatórios gerenciais consolidados de impacto e transparência não deve impactar a performance do sistema durante a operação simultânea dos estoquistas. |  BAIXA |

Com base nas Histórias de Usuário, enumere os requisitos da sua solução. Classifique esses requisitos em dois grupos:

- [Requisitos Funcionais
 (RF)](https://pt.wikipedia.org/wiki/Requisito_funcional):
 correspondem a uma funcionalidade que deve estar presente na
  plataforma (ex: cadastro de usuário).
- [Requisitos Não Funcionais
  (RNF)](https://pt.wikipedia.org/wiki/Requisito_n%C3%A3o_funcional):
  correspondem a uma característica técnica, seja de usabilidade,
  desempenho, confiabilidade, segurança ou outro (ex: suporte a
  dispositivos iOS e Android).
Lembre-se que cada requisito deve corresponder à uma e somente uma
característica alvo da sua solução. Além disso, certifique-se de que
todos os aspectos capturados nas Histórias de Usuário foram cobertos.

## Restrições

O projeto está restrito pelos itens apresentados na tabela a seguir.

|ID| Restrição                                             |
|--|-------------------------------------------------------|
|01| O projeto utilizará apenas ferramentas e servidores gratuitos. | ALTA |
|02| O sistema não utilizará login via redes sociais.  | BAIXA |
|03| O sistema não calculará a depreciação financeira dos itens estocados.  | MÉDIA |
|04| O sistema operará exclusivamente no idioma português do Brasil.  | MÉDIA |
|05| Não haverá funcionalidade para importar dados em massa através de planilhas Excel ou CSV. | MÉDIA
|06| Cada formulário de registro de doação terá um limite de produtos para evitar sobrecarga. | MÉDIA
|07| A interface web será homologada apenas para as versões recentes do Google Chrome, Edge e Firefox. | ALTA
|08| O sistema aceitará apenas imagens nos formatos JPG e PNG para os envios de fotos. | MÉDIA
|09| O registro de itens no estoque não aceitará quantidades fracionadas, apenas números inteiros. | MÉDIA
|10| Os logs de auditoria de operações de estoque serão apagados automaticamente após 6 meses. | BAIXA
