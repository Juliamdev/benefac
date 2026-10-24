### 3.3.1 Processo 2 – RECEBIMENTO E ENTRADA EM ESTOQUE

_Este processo ocorre presencialmente no galpão ou sede da instituição e na Plataforma Web do BENEFAC. 
O processo tem início quando o doador comparece fisicamente com os donativos e é encerrado quando o registro da nova doação é salvo com sucesso e o estoque é atualizado, ficando disponível para que a equipe logística realize as separações e entregas no próximo processo (Processo 3 – Distribuição de Benefícios).
Participa deste processo o Estoquista, responsável por realizar a triagem física e informar os dados no sistema onde são processadas as informações e gravado o registro. As principais tarefas do processo são: conferir os itens físicos (categoria, quantidade, estado de conservação e validade), acessar o sistema para iniciar um novo registro, preencher os dados do doador e dos itens, e confirmar a entrada. O produto gerado por este processo é o Registro de Recebimento e o Saldo de Estoque Atualizado, contendo os itens conferidos e contabilizados, disponíveis para as próximas etapas do fluxo._




##### 3.3.1.1 Modelagem BPMN

<img width="3504" height="970" alt="processo2-benefac-corrigido" src="https://github.com/user-attachments/assets/0138738e-da3f-4e58-adb9-14ac242814f8" />


##### 3.3.1.2 Detalhamento das atividades do usuário (user tasks)

#### Detalhamento das atividades

**Acesso ao sistema**

| **Campo**            | **Tipo**         | **Restrições**                                  | **Valor default** |
| ---                  | ---              | ---                                             | ---               |
| login                | Caixa de Texto   | obrigatório; formato de e-mail                  | vazio             |
| senha                | Caixa de Texto   | obrigatório; mínimo de 8 caracteres             | vazio             |

| **Comandos**         |  **Destino**                                   | **Tipo** |
| ---                  | ---                                            | ---      |
| entrar               | Atividade: Registro dos itens da doação        | default  |
| recuperar senha      | Atividade: Recuperação de senha                | default  |


**Registro do doador**

| **Campo**            | **Tipo**         | **Restrições**                                  | **Valor default** |
| ---                  | ---              | ---                                             | ---               |
| cpf_cnpj_doador      | Caixa de Texto   | formato numérico; opcional                      | vazio             |
| nome_doador          | Caixa de Texto   | obrigatório                                     | vazio             |
| campanha_relacionada | Seleção única    | lista das campanhas vigentes; opcional          | vazio             |
| email_doador         | Caixa de Texto   | obrigatório                                     | vazio             |

| **Comandos**         |  **Destino**                                   | **Tipo** |
| ---                  | ---                                            | ---      |
| avançar              | Atividade: Realizar login                      | default  |
| avançar              | Atividade: Preencher dados do doador           | default  |
| cancelar             | Fim do Processo 2                              | cancel   |


**Registro dos itens da doação**

| **Campo**            | **Tipo**         | **Restrições**                                            | **Valor default** |
| ---                  | ---              | ---                                                       | ---               |
| nome_item            | Caixa de Texto   | obrigatório                                               | vazio             |
| categoria            | Seleção única    |                                                           | vazio             |
| quantidade           | Número           | obrigatório; mínimo 1                                     | 1                 |
| estado_conservacao   | Seleção única    | obrigatório; opções: Novo, Usado - bom, Usado - regular   | vazio             |
| validade             | Data             | obrigatório somente quando categoria = Alimento           | vazio             |

| **Comandos**         |  **Destino**                                         | **Tipo** |
| ---                  | ---                                                  | ---      |
| confirmar entrada    | Fim do Processo 2                                    | default  |
| adicionar outro item | Atividade: Preencher dados dos itens recebidos       | default  |
| voltar               | Atividade: Acessar o sistema e iniciar novo registro | default  |
| cancelar             | Fim do Processo 2                                    | cancel   |

##### 3.3.1.3 Wireframes (user tasks) 

<img width="1280" height="900" alt="acessar-sistema" src="https://github.com/user-attachments/assets/1c427bec-f3e6-423c-966a-167f1ec526c1" />

<img width="1869" height="1309" alt="wireframe-processo2-1" src="https://github.com/user-attachments/assets/f0dcb998-4859-4b90-9050-f6b97e09cef2" />

<img width="1863" height="1311" alt="wireframe-processo2-2" src="https://github.com/user-attachments/assets/0f1c475b-7798-40d6-bc3b-4d4d9785577f" />


