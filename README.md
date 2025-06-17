# AZURE_criar_DB
### Laboratório - Criação de uma instânica gerenciada de Banco de Dados SQL no Microsoft Azure

### Objetivo

Praticar a criação e configuração de uma instância de Banco de Dados no **Microsoft Azure**, além de reunir resumos, anotações e dicas úteis como material de apoio para estudos e futuras implementações.

___

### Passo a Passo - Criação do Banco de Dados SQL no Azure

#### Criar uma **Instância Gerenciada de SQL** no Azure

1. Acesse o [Portal Azure](https://portal.azure.com/)
2. No menu esquerdo, clique em **"SQL do Azure"**  
   ➝ Se não aparecer, vá em **"Todos os serviços"** e pesquise por **"SQL do Azure"**.
3. Clique em **"+ Criar"**.
4. Na página **"Selecionar opção de implantação do SQL"**, no bloco **"Instâncias gerenciadas de SQL"**, clique em **"Mostrar detalhes"** se quiser saber mais.
5. Em **"Tipo de Banco de Dados"**, selecione **"Instância única"** e clique em **"Criar"**.
6. Preencha os dados solicitados:
   - Assinatura
   - Grupo de recursos (existente ou novo)
   - Nome da instância
   - Região
   - Login e senha de administrador
7. Configure rede, segurança, backups e outros parâmetros conforme necessário.
8. Clique em **"Revisar + criar"** e depois em **"Criar"** para iniciar a implantação.

---

#### Criar um **Banco de Dados** na Instância Gerenciada

1. Acesse sua **Instância Gerenciada de SQL** no portal.
2. Na aba **"Visão Geral"**, clique em **"+ Novo banco de dados"**.
3. Na aba **"Básico"**, informe o **nome do banco de dados**.
4. Na aba **"Fonte de dados"**, escolha:
   - **"Nenhuma"** para criar um banco vazio, ou
   - Restaurar a partir de um backup existente.
5. Defina configurações adicionais nas demais abas (como desempenho, segurança e backups).
6. Clique em **"Revisar + criar"** e, em seguida, em **"Criar"** para finalizar.
