# ORGANIZE - SISTEMA DE GERENCIAMENTO DE CHAMADOS
### Documento de Visão 

## 1 Introdução 

##### 1.1 Sumário executivo 
O Organize, é uma ferramenta desktop que, durante a primeira etapa, será capaz de  
otimizar a gestão de chamados de clientes, proporcionando uma experiência eficiente e personalizada para empresas.

##### 1.2 Escopo 
###### 1.2.1 O que o Organize é… 

 O Organize é um sistema de gerenciamento de chamados destinado a:

- Gerenciar chamados de clientes;
- Otimizar fluxos de trabalho;
- Fornecer insights estratégicos.

###### 1.2.2 O que  o Organize não é… 
-  Um sistema de comunicação social. 

###### 1.2.3 O que  o Organize faz… 
- Cria, consulta e atualiza e armazena dados dos chamados da (EMPRESA FICTICIA). 


###### 1.2.4 O que o Organize não faz … 
- Não realiza troca de informações com outros sistemas;
- Não realiza troca de mensagens entre usuários externos e internos;


## 2 Problema

##### 2.1 Dispersão 
- Os dados estão armazenados de forma dispersa, em diferentes documentos, o que tem imposto uma lentidão no gerenciamento, atualização e consulta desses chamados. 

## 3 Cliente 

- Empresas de Prestação de Serviços (EMPRESA FICTICIA). 


## 4 Usuários


##### 4.2 Supervisor de Suporte (EMPRESA FICTICIA). 

- Criar, consultar, atualizar e excluir chamados;
- Editar informações de clientes;
- Gerenciar chamados prioritários;
- Atribuir chamados à equipe.
- Visualizar relatórios de desempenho por usuário;
- Analisar métricas de eficiência;
- Tomar decisões estratégicas.

##### 4.4 Suporte Nível 1 (EMPRESA FICTICIA). 

- Alterar dados específicos do chamados (objetivo, status, cliente, etc.);
- Preencher campos obrigatórios;
- Anexar documentos relevantes.


## 5 Requisitos 

##### 5.1Requisitos Funcionais 

| Cod | Nome | Descrição |  
| ------ | ------ | ------ |
| RF01 | Gerenciar Chamados | O sistema realiza o cadastro, alteração e exclusão de chamados.
| RF02 | Gerenciar Cliente | O sistema realiza o cadastro, alteração e exclusão de clientes. 
| RF03 | Pesquisa detalhada  | O sistema permite buscar através da combinação de filtro de dados o cliente desejado.
| RF04 | Gerenciar usuários | O sistema realiza o gerenciamento de permissões dos usuários. 

##### 5.2 Requisitos Não Funcionais

| Cod | Nome | Descrição |
| ------ | ------ | ------ |
| NF01 | Desempenho | O sistema deve responder em menos de 2 segundos. |
| NF02 | Usabilidade | Interface intuitiva e fácil de usar. |
| NF03 | Segurança | Autenticação e autorização para acessar chamados. |
| NF04 | Escalabilidade | Suporte a 100 usuários simultâneos. |
| NF05 | Compatibilidade | Suporte a navegadores modernos e dispositivos móveis. |
| NF06 | Facilidade de Manutenção | Documentação clara e atualizada. |
| NF07 | Recuperabilidade | Backup automático diário. |
| NF08 | Confiabilidade | Disponibilidade de 99,9%. |

##### 5.3 Requisitos de Qualidade

###### RF01 - Gerenciar Chamados

| Item | Descrição |
| ------ | ------ |
| Identificação | RF01 |
| Objetivo | Tempo de resposta rápido |
| Escala | Tempo decorrido em segundos |
| Métrica | Medir tempo entre ação e confirmação |
| Mínimo | Menos de 2s para 90% dos casos |
| Intervalo OK | Entre 1-2s para 95% dos casos |
| Ótimo | Menos de 1s para 99% dos casos |
| Prioridade | Alta |

######  RF02 - Gerenciar Clientes

| Item | Descrição |
| ------ | ------ |
| Identificação | RF02 |
| Objetivo | Eficiência na busca de clientes |
| Escala | Tempo de busca |
| Métrica | Medir tempo entre busca e resultado |
| Mínimo | Menos de 1,5s para 90% dos casos |
| Intervalo OK | Entre 1-1,5s para 95% dos casos |
| Ótimo | Menos de 1s para 99% dos casos |
| Prioridade | Alta |

###### RF03 - Pesquisa Detalhada

| Item | Descrição |
| ------ | ------ |
| Identificação | RF03 |
| Objetivo | Precisão na pesquisa |
| Escala | Taxa de resultados relevantes |
| Métrica | Medir precisão dos resultados |
| Mínimo | 90% de precisão |
| Intervalo OK | Entre 90-95% |
| Ótimo | 100% de precisão |
| Prioridade | Média |

###### RF04 - Gerenciar Usuários

| Item | Descrição |
| ------ | ------ |
| Identificação | RF04 |
| Objetivo | Segurança nas permissões |
| Escala | Taxa de acessos autorizados |
| Métrica | Medir acessos autorizados vs. não autorizados |
| Mínimo | 99% de acessos autorizados |
| Intervalo OK | Entre 99-100% |
| Ótimo | 100% de acessos autorizados |
| Prioridade | Alta |


## 6 Regras de Negócio 

| Cod | Nome | Descrição |
| ------ | ------ | ------ |
| RN01 | Permissões de alteração | Para realizar modificações no sistema o usuário precisa estar cadastrado e possuir as permissões de alteração, conforme o(s) perfil(is) de usuário a ele atribuído(s). 
| RN02 | Tipo definido de status | Os chamados só podem ser cadastrados se possuir um tipo ( manutenção, suporte, agendamento) definido.
| RN03 | Condições de Cadastro de Chamados | Os processos só podem ser cadastrados se possuírem um cliente vinculado ao cadastro do chamado.