### 3.3.1 Processo 4 – GESTÃO DE USUÁRIOS E PERMISSÕES

_Este processo de apoio visa gerenciar os acessos , o fluxo é realizado exclusivamente na área administrativa pelo Gestor. Ao aceder ao módulo de gestão, o Gestor depara-se com duas opções: cadastrar um novo usuário ou alterar os dados e permissões de um usuário já existente.
Se for um novo cadastro, o Gestor insere os dados pessoais (CPF, Nome, E-mail, Senha) e define o perfil de acesso inicial.
Se a intenção for editar um acesso existente, o Gestor localiza o usuário, edita os dados necessários (ou altera o perfil de acesso/desativa o usuário).
Em ambos os fluxos, o sistema valida as informações (impedindo duplicidade de CPF/E-mail ou validando alterações) e salva as novas diretrizes, atualizando as permissões daquele perfil imediatamente. O produto final é o acesso criado, modificado ou revogado._

##### 3.3.1.1 Modelagem BPMN

<img width="3700" height="802" alt="processo4-benefac-corrigido" src="https://github.com/user-attachments/assets/3aaed9b4-0ad0-4e73-a376-d8d5ea3abc2e" />

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

**Localização do usuário**

| **Campo**            | **Tipo**         | **Restrições**                   | **Valor default** |
| ---                  | ---              | ---                              | ---               |
| termo_busca          | Caixa de Texto   | opcional; busca por nome ou CPF  | vazio             |

| **Comandos**         |  **Destino**                                      | **Tipo** |
| ---                  | ---                                               | ---      |
| novo usuário         | Atividade: Preencher dados de novo usuário        | default  |
| editar usuário       | Atividade: Editar dados, permissões ou desativar  | default  |
| cancelar             | Fim do Processo 4                                 | cancel   |


**Preencher dados de novo usuário e perfil**

| **Campo**            | **Tipo**         | **Restrições**                                    | **Valor default** |
| ---                  | ---              | ---                                               | ---               |
| cpf                  | Caixa de Texto   | obrigatório; formato numérico; único no sistema   | vazio             |
| nome_completo        | Caixa de Texto   | obrigatório                                       | vazio             |
| email                | Caixa de Texto   | obrigatório; formato de e-mail; único no sistema  | vazio             |
| senha                | Caixa de Texto   | obrigatório; mínimo de 8 caracteres               | vazio             |
| perfil_acesso        | Seleção única    | obrigatório; opções: Gestor, Estoquista, Doador   | vazio             |

| **Comandos**         |  **Destino**                               | **Tipo** |
| ---                  | ---                                        | ---      |
| confirmar gravação   | Atividade: Confirmar a gravação dos dados  | default  |
| voltar               | Atividade: Acesso ao sistema de gestão     | default  |
| cancelar             | Fim do Processo 4                          | cancel   |


**Editar dados, permissões ou desativar usuário**

| **Campo**            | **Tipo**         | **Restrições**                                   | **Valor default** |
| ---                  | ---              | ---                                              | ---               |
| cpf                  | Caixa de Texto   | bloqueado para edição (somente leitura)          | [CPF atual]       |
| nome_completo        | Caixa de Texto   | obrigatório                                      | [Nome atual]      |
| email                | Caixa de Texto   | obrigatório; formato de e-mail; único no sistema | [E-mail atual]    |
| redefinir_senha      | Caixa de Texto   | opcional; mínimo de 8 caracteres                 | vazio             |
| perfil_acesso        | Seleção única    | obrigatório; opções: Gestor, Estoquista, Doador  | [Perfil atual]    |
| status_usuario       | Caixa de Seleção | opções: Ativo, Inativo                           | Ativo             |

| **Comandos**         |  **Destino**                               | **Tipo** |
| ---                  | ---                                        | ---      |
| confirmar gravação   | Atividade: Confirmar a gravação dos dados  | default  |
| voltar               | Atividade: Acesso ao sistema de gestão     | default  |
| cancelar             | Fim do Processo 4                          | cancel   |

##### 3.3.1.3 Wireframes (user tasks) 

<img width="2200" height="1227" alt="wireframe-processo4-2" src="https://github.com/user-attachments/assets/5f3e53dc-0844-4a3c-b052-4c65105549b9" />

<img width="2208" height="1225" alt="wireframe-processo4" src="https://github.com/user-attachments/assets/24db5795-dc4a-49d9-86f6-7b74101cb7e2" />

<img width="2199" height="1222" alt="wireframe-processo4-3" src="https://github.com/user-attachments/assets/631dd5df-5ac2-4e10-ba1d-376ce2bef2f3" />

