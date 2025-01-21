# Storage_ServiceStorageAccounts
Objetivo é configurar o serviiço: Storage Accounts

### Material:
* https://learn.microsoft.com/pt-br/azure/storage/common/storage-account-create?tabs=azure-portal

01 - Selecionar na tela ``` Home ``` a opção: ``` Create a resource ```
![image](https://github.com/user-attachments/assets/bae4af5f-fdfe-4d57-b507-9b674c327d75)

02 - Selecionar o recurso ``` Storage Account  ``` e no botão ``` Create  ```
![image](https://github.com/user-attachments/assets/2ab0d391-829a-4f0e-9db0-5d1c7b4c69fa)

03 - Iniciar a configuração criando o repositório onde será salvo nosso projeto, modelo, laboratório. Fique a vontade para chamar do melhor padrão para sua necessidade.
   * Subscription: é a conta que você está logado. É como se você a sua empresa. Repositótorio geral de tudo que é criado, a Pasta principal. Já vem preenchido de padrão, Esse padrão é criado automaticamente quando realiza o cadastro. Mas pode ser criado outras opções.
   * Resource group: é uma sub-repositório do "Subscription".
Imagina uma gaveteiro onde o gaveteiro inteiro é Subscriptiom e uma gaveta desse gaveteiro é o Resource group.
   * Storage account name: nome do repositório que irá subir os dados para realizar essa atividade. A sua base de dados.
   * Region: basicamente, quer dizer em qual servidor da Microsoft você quer salvar(brasil, USA etc). Acredito que também determina a moeda que será cobrado por utilizar esse serviço.
   * Primary service: permite que você escolha os tipos de serviços de armazenamento que serão habilitados no armazenamento que está sendo criado. No nosso caso escolher "Azure Blob Storage or Azure Data Lake Storage Gen 2". Cuidado que dependendo da escolha o custo do serviço pode ficar maior. Para esse exemplo, não importa muito, pois vamos excluir no final.
   * Performance: Selecionar Standard. Cuidado que dependendo da escolha o custo do serviço pode ficar maior.
   * Redundancy: Vamos selecionar a opção "Locally-redundant storage (LRS)". Cuidado que dependendo da escolha o custo do serviço pode ficar maior.
![image](https://github.com/user-attachments/assets/6285d2ac-a36f-499e-9109-489980e5daa1)

04 - Demais Abas: vamos manter o padrão, pois estamos realizando uma configuração basica e iremos excluir esse modelo no final. Então, click no botão Review + create para validar as configurações e depois click novamente no botão Create
   * Advanced: Configuração de segurança do banco criado: Como será o acesso, permite acesso anônimo etc. 
   * Networking: configuração de privacidade do seu modelo(Publico/Privado)
   * Data protetion: configuração de restauração, backup.
   * Encryption: habilitar encryptitação do banco.
   * Tags: muito usado para criar filtros. Por exemplo: Quero fazer rateio para lançamento de custo por Departamento, então, cria as tags por departamento. Conforme sua necessidade.
![image](https://github.com/user-attachments/assets/0089d25c-b726-4bef-af31-82b44874e297)

05 - Após finalizar a criação do Storage, então selecionar o mesmo  clicando no nome para entrarmos nas configurações.
![image](https://github.com/user-attachments/assets/f543df60-2ec2-40ec-8694-c5e1325989b0)

06 - Nesse nosso laboratório vamos precisar desativar algumas configurações de acesso anonimo para conseguir finalizar. Lembrando que essa ação é devido o nosso laboratório e vamos excluir logo em seguida, Na produção essas configurações tem que ser avaliada.
![image](https://github.com/user-attachments/assets/a62304b0-9d25-4c43-af56-71335ed2b326)

07 - Agora, vamos criar um "Container", onde iremos colocar nossos arquivos.
   * Name: nome unico do Container
   * Anonymous access level: selecionar a opção  ``` Container (anonumous read access for containers and blobs)  ```
![image](https://github.com/user-attachments/assets/19e2df6c-fd50-4446-9054-a9e1eeba404a)

08 - Neste momento, vamos subir nosso arquivo que iremos utilizar. Então, após criar o Container, selecionar clicando no nome, e depois no botão ``` Upload  ```, subir os arquivos. (Nadocumentaçaõ tem o link dos arquivos que vamos usar aqui e subir o mesmo numa pasta aqui no Github). Lembrar que os arquivos devem está descompactados.
![image](https://github.com/user-attachments/assets/1de94e85-0bc3-45f0-83e0-a32f9cc7a389)

