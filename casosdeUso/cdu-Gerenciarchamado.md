# (CDU 01) Gerenciar Chamado

## 1. Descrição
O sistema permitirá que usuários autorizados gerenciem chamados, incluindo cadastro, alteração, exclusão e visualização.

## 2. Atores
- **Suporte nível 1**: Funcionário da equipe de suporte.
- **Supervisor de Suporte**: Responsável pela gestão do setor de suporte.

## 3. Pré-condições
- O usuário deve estar autenticado e autorizado.
- O sistema deve estar disponível e funcionando corretamente.

## 4. Pós-condições
1. O chamado é criado, alterado ou excluído com sucesso.
2. O sistema atualiza a lista de chamados.
3. O usuário recebe confirmação da ação realizada.

## 5. Fluxo Principal
1. O usuário acessa a interface de gerenciamento de chamados.
2. O sistema exibe a lista de chamados disponíveis.
3. O usuário seleciona a opção de **Cadastrar Novo Chamado**.
4. O sistema exibe os campos a serem preenchidos para criação do chamado (descrição do problema, urgência, setor, responsável, etc.).
5. O usuário preenche as informações necessárias e clica em **Adicionar**.
6. O sistema valida os dados e, se corretos, cria o novo chamado e o exibe na lista.
7. O sistema envia uma confirmação para o usuário de que o chamado foi criado com sucesso.
8. O usuário pode, então, visualizar, editar ou excluir o chamado conforme necessário.

## 6. Fluxo Alternativo
### 6.1 Fluxo Alternativo - Acesso sem permissão
1. O usuário tenta acessar uma funcionalidade sem permissão.
2. O sistema exibe mensagem de erro e bloqueia o acesso.
3. O usuário é redirecionado para a página inicial.

### 6.2 Fluxo Alternativo - Dados incompletos ou incorretos
1. O usuário tenta criar um chamado com dados incompletos ou incorretos.
2. O sistema exibe uma mensagem de erro informando o problema (ex: "Campo obrigatório não preenchido" ou "Descrição inválida").
3. O usuário corrige os dados e tenta novamente criar o chamado.

### 6.3 Fluxo Alternativo - Chamado já existente
1. O usuário tenta cadastrar um chamado com um código ou descrição que já existe no sistema.
2. O sistema exibe uma mensagem de erro informando que o chamado já foi registrado.
3. O usuário revisa e modifica os dados antes de tentar novamente.

## 7. Situações de erro
- **Dados do chamado incompletos ou incorretos**: O sistema não permite que o chamado seja criado ou atualizado sem todos os dados obrigatórios preenchidos corretamente.
- **Chamado já existente**: Se um chamado com o mesmo código ou descrição já estiver registrado, o sistema impedirá a duplicação.

## 8. Regras de negócio
- **RN01**: O código do chamado deve ser único no sistema.
- **RN02**: Somente usuários com permissões específicas podem editar ou excluir chamados de outros usuários.
- **RN03**: Chamados com urgência alta devem ser visualizados e tratados de forma prioritária.
- **RN04**: O sistema deve enviar uma notificação por e-mail para os responsáveis pelo chamado quando ele for criado ou atualizado.

## 9. Observações
- O fluxo de gerenciamento de chamados é central para o processo de suporte, sendo crucial para garantir a resolução eficiente dos problemas.
- A interface do sistema deve ser intuitiva para que os usuários possam facilmente navegar entre as opções de cadastro, visualização, edição e exclusão de chamados.

