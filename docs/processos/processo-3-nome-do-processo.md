### 3.3.1 Processo 3 – DISTRIBUIÇÃO DE BENEFÍCIOS

Participam deste processo o Estoquista, responsável por cadastrar a requisição, checar a disponibilidade, reservar itens, realizar a entrega e coletar a assinatura, e o Sistema, responsável por validar o estoque, organizar a fila de espera cronologicamente, registrar a rastreabilidade do lote original e abater o saldo automaticamente após a entrega. As principais tarefas do processo são: cadastrar requisição de assistência, consultar disponibilidade dos itens solicitados, reservar itens no sistema, separar itens físicos, realizar a entrega coletando assinatura digital e abater o saldo do estoque. O produto gerado por este processo é o Comprovante de Entrega e Baixa de Estoque, que atende aos requisitos de rastreabilidade e prestação de contas

##### 3.3.1.1 Modelagem BPMN

<img width="2018" height="1692" alt="Processo3CERTO" src="https://github.com/user-attachments/assets/cdaeb71b-375a-4237-977d-2f92d4a617c4" />


##### 3.3.1.2 Detalhamento das atividades do usuário (user tasks)

#### Detalhamento das atividades

### 1. Acessar o Sistema

#### Campos de Entrada
| Campo | Tipo | Restrições | Valor default |
| :--- | :--- | :--- | :--- |
| email | Caixa de Texto | obrigatório; formato de e-mail válido | vazio |
| senha | Caixa de Texto / Senha | obrigatório; mínimo 6 caracteres | vazio |

#### Comandos / Ações
| Comandos | Destino | Tipo |
| :--- | :--- | :--- |
| entrar | Atividade: Gerenciar Requisições | default |
| esqueci a senha | Tela de Recuperação de Senha | - |

**Cadastrar Requisição de Assistência**

| **Campo**       | **Tipo**         | **Restrições** | **Valor default** |
| ---             | ---              | ---            | ---               |
| cpf             | Caixa de Texto   | obrigatório    |                   |
| nome_completo   | Caixa de Texto   | obrigatório    |                   |
| categoria_item  | seleção única    | obrigatório; opções: Alimento, Higiene, Vestuário |                |
| quantidade      | número           | obrigatório; apenas números inteiros |           |

| **Comandos**         |  **Destino**                                   | **Tipo**  |
| ---                  | ---                                            | ---       |
| adicionar            | Adiciona o item à lista da requisição atual    |           |
| salvar requisição    | Atividade: Consultar disponibilidade (Sistema) | default   |
| cancelar             | Atividade: Gerenciar Requisições               | cancel    |


**Gerenciar Requisições (Aba Principal / Fila)**

| **Campo**            | **Tipo**         | **Restrições** | **Valor default** |
| ---                  | ---              | ---            | ---               |
| busca                | Caixa de Texto   | opcional       |                   |
| tabela_requisicoes   | Tabela           | campo formado por uma matriz de valores; somente leitura; ordenada da mais antiga para a mais recente | |

| **Comandos**         |  **Destino**                                       | **Tipo**  |
| ---                  | ---                                                | ---       |
| nova requisição      | Atividade: Cadastrar Requisição de Assistência     | default   |
| reservar             | Atividade: Reservar itens no sistema (Altera status)|          |
| entregar             | Atividade: Realizar Entrega e Coletar Assinatura   | default   |
| excluir              | Atividade: Excluir uma requisição                  | default   |
| editar               | Atividade: Editar uma Requisição                   | default   |


**Realizar Entrega e Coletar Assinatura Digital**

| **Campo**            | **Tipo**         | **Restrições** | **Valor default** |
| ---                  | ---              | ---            | ---               |
| info_beneficiado     | Caixa de Texto   | somente leitura |                  |
| itens_entregues      | Tabela           | campo formado por uma matriz de valores; bloqueado para alteração | |
| termo_recebimento    | Área de texto    | somente leitura |                  |
| assinatura_digital   | Área de desenho  | obrigatório; validação da entrega presencial | |

| **Comandos**               |  **Destino**                                        | **Tipo**  |
| ---                        | ---                                                 | ---       |
| limpar assinatura          | Próprio formulário (limpa o campo de desenho)       |           |
| confirmar entrega e baixa  | Fim do Processo 3 (Sistema abate saldo)             | default   |
| cancelar                   | Atividade: Gerenciar Requisições                    | cancel    |

##### 3.3.1.3 Wireframes (user tasks) 


<img width="1877" height="892" alt="Captura de tela 2026-10-16 153043" src="https://github.com/user-attachments/assets/74b12136-9e8d-4af8-a6b4-0586f1689dd6" />


<img width="1886" height="877" alt="Captura de tela 2026-10-16 153059" src="https://github.com/user-attachments/assets/943c7c02-895c-4d49-90e7-fa90705a84e3" />


<img width="1872" height="892" alt="Captura de tela 2026-10-16 153112" src="https://github.com/user-attachments/assets/1afcfe6f-1697-4e02-bb77-5ea01783e8e6" />

