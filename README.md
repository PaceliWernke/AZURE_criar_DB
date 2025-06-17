# AZURE Criar Database via Portal
### Objetivo
#### Laboratório - Criação de um Banco de Dados SQL no Microsoft Azure

___

### Passo a Passo - Criação do Banco de Dados SQL no Azure

1. Acesse o [Portal Azure](https://portal.azure.com/).

2. No menu, vá em **"Criar um recurso" > "SQL" > "Banco de Dados SQL"** e clique em **"Criar"**.

3. Na guia **Básico**, preencha:

   * **Assinatura:** selecione sua conta.
   * **Grupo de recursos:** clique em **"Criar"**, digite `myResourceGroup` e confirme.
   * **Nome do banco:** `mySampleDatabase`.
   * **Servidor:** clique em **"Criar"** . Vai abrir uma nova página.
     * Preencha:
        * **Nome do servidor:** algo como `my-sql-server-1` (nome deverá ser único).
        * **Localização:** escolha a mais próxima (ex.: "(South America) Brazil South").
        * **Autenticação:** selecione **"Usar autenticação somentre do Microsoft Entra"**.
        * **Definir administrador do MS Entra:** Clique em "Definir administrador" e escolha o seu usuário do Azure e clique em "Selecionar".
   * Irá voltar para a página do Banco de Dados.

4. **Pool elástico:** mantenha como **Não**.

5. **Ambiente de carga de trabalho:** selecione **Desenvolvimento**, o que vai definir automaticamente:
   * **Computação: uso geral sem servidor**, 1 vCore, 32 GB.
   * **Redundância do armazenamento de Backup** com **redundância local** (menor custo).

6. Em **Computação + armazenamento**, clique em **"Configurar banco de dados"**, mantenha:

   * **Uso Geral (Mais amigável ao orçamento)** → **"Aplicar"**.

7. Na opção **Redundância de armazenamento de backup**, mantenha "com redundânica local".

8. Clique em **Avançar: Rede >** e configure:

   * **Método de conectividade:** **Ponto de extremidade público**.
   * **Permitir que serviços do Azure acessem este servidor:** **Não**.
   * **Adicionar IP do cliente atual:** **Sim**.
   * **Política de conexão:** mantenha **Padrão**.
   * **Versão mínima do TLS:** mantenha em **TLS 1.2**.

9. Clique em **Avançar: Segurança >**:

   * (Opcional) Ative o **Microsoft Defender para SQL** e configure identidades ou criptografia, se desejar.

10. Clique em **Avançar: Configurações adicionais >**:

    * Em **Fonte de dados**, selecione **Amostra** (carrega o banco de exemplo **AdventureWorksLT** com dados e tabelas).

11. Clique em **Revisar + criar** para revisar as configurações.

12. Se estiver tudo correto, clique em **Criar** e aguarde o provisionamento.

---
