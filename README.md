# Dio-MS-ai900-DP04-CognitiveSearchAzure
Desafio de Projeto da DIO para bootcamp ai900 Azure AI Fundamentals - Cognitive Search Azure

- Dentro desse desafio estaremos seguindo as três documentações a seguir, mas note que o inicio de criação e deploy do Resource é igual. Apenas dentro do Vision Studio havera distinção nas documentações.
  - Azure AI Search => [https://aka.ms/ai900-face](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/11-ai-search.html)

## STEP 01
- No partal do Azure: https://portal.azure.com/ 
- Crie um novo recurso, dependendo em qual tela estiver pode clicar em "**+ Create a resurce**" ou "**Create**".
![Screenshot 2024-04-05 083344](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/1424e0b1-ec82-4808-803e-a67ae4c1086f)

- O recurso a ser criado será o "**Azure Ai Search**", pode pesquisar por esse nome na barra de pesquisa ou dentro da categori "**AI + Machine Learning**".
![Screenshot 2024-04-05 083552](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/a761b693-a7ad-4869-948b-516e0bab4501)
![Screenshot 2024-04-05 084001](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/db891904-5d07-4ec9-a3ac-e57d153e873b)
- Preencha o "**Resource Group**", "**Name**", "**Change Pricing tier**" Selecione o "**Basic**". Agora Clique em "**Review + create**" e na tela final "**Create**".
- "**Lembre**": Criar os resources com a "**Region**" nos EUA consome menos créditos do Azure.
![Screenshot 2024-04-05 084041](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/ebdfc82c-c3fe-4d72-ac0a-395d653c513c)
![Screenshot 2024-04-05 084120](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/682620f7-dbf9-4000-85a2-16080ca9089a)
![Screenshot 2024-04-05 084208](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/94e018c3-c8d7-453b-bb0d-1374f516ebb9)
![Screenshot 2024-04-05 084232](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/2cb0b667-2487-4d36-8c4a-f121a8423f8c)
- Aguarde o deploy do resource estar completo.
![Screenshot 2024-04-05 084305](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/a3361d13-b41a-4039-86c9-942731dbb1e2)

## STEP 02
- Crie um novo recurso, dependendo em qual tela estiver pode clicar em "**+ Create a resurce**" ou "**Create**".
![Screenshot 2024-04-05 084403](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/327f2293-8ae9-4118-88a1-d8a09455f64a)

- O recurso a ser criado será o "**Azure Ai Services**", pode pesquisar por esse nome na barra de pesquisa ou dentro da categori "**AI + Machine Learning**".
- Preencha o "**Resource Group**", "**Name**", "**Pricing tier**" com o valor "**Standard S0**" e por fim marque o checkbox. Agora Clique em "**Review + create**" e na tela final "**Create**".
- "**Lembre**": Criar os resources com a "**Region**" nos EUA consome menos créditos do Azure.
![Screenshot 2024-04-05 084550](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/29a2cf31-d705-443d-81de-6ee37c58bc2f)
![Screenshot 2024-04-05 084608](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/339db355-42ac-43e1-8045-c3dd143d6974)

- Aguarde o deploy do resource estar completo.
![Screenshot 2024-04-05 084631](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/a4127f1f-5938-4b68-a0f1-63a15a66d533)


## STEP 03
- Volte a tela inicial ou vá ao create novo resource e vamos criar uma "**Storage Account**".
![Screenshot 2024-04-05 090304](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/bc8943eb-7b58-4fcd-9228-4479e61d5349)
![Screenshot 2024-04-05 091901](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/253f9624-5daa-43b3-a71c-2b5273b8206c)
- - Preencha o "**Resource Group**", "**Storage account Name**", "**Performance**" com o valor "**Standard**" e "**Redunsdancy**" com o valor "**Locally-redundant storage(LRS)**". Agora Clique em "**Review + create**" e na tela final "**Create**".
- "**Lembre**": Criar os resources com a "**Region**" nos EUA consome menos créditos do Azure.
![Screenshot 2024-04-05 093456](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/079c26ce-bb99-43e1-8b17-ef23620532b6)
![Screenshot 2024-04-05 093525](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/1bd7cfa4-84df-49bf-9fee-89a25ec4b00a)
- Aguarde o deploy do resource estar completo e entre no resource(Storage Account).
![Screenshot 2024-04-05 093647](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/d0f49e8c-37c2-4959-a6a8-e8c9afdf7bb0)

## STEP 04
- Dentro do Storage Account vá em **Configuration** e deixar a opção "**Allow Blob anonymous access**" como **Enabled**
![Screenshot 2024-04-05 093733](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/8ed4c45e-4140-4ea5-8aa6-1ceb5b0f2eec)
![Screenshot 2024-04-05 093851](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/86f426d6-5ba6-46fa-a81e-be40f306265d)

## STEP 05
- Ainda dentro do Storage Account vá em **Containers** vamos criar um novo Container
![Screenshot 2024-04-05 093925](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/c3ccfd2a-6e1d-4e60-b530-189de4be2703)
  - Name: coffee-reviews
  - Public access level: Container (anonymous read access for containers and blobs)
  - Advanced: no changes.
![Screenshot 2024-04-05 094435](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/47a1d9ba-7fa5-40b1-aaf6-12748772c3c1)
- Selecione o Container para fazermos o upload de arquivos. **Faça DOWNLOAD dos arquivos na documentação**
![Screenshot 2024-04-05 094447](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/c49514f7-6ad7-4061-9926-4194eb45597f)
![Screenshot 2024-04-05 094712](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/92187a91-c055-4585-a809-9b351bbb4a93)
![Screenshot 2024-04-05 094815](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/e88a2a5b-a414-48e8-9b09-a9c59ef8e11c)

## STEP 06
- Vamos ao AI Search para fazermos um **Import Data**
![Screenshot 2024-04-05 094849](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/54e7f50a-1dc2-45f0-9ace-410805bf5eca)
![Screenshot 2024-04-05 094908](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/216022a0-822c-49a1-989c-a4c1923b3f0e)
![Screenshot 2024-04-05 094930](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/12660e94-0ebb-4670-8183-355549d7a9dd)
  - Data Source: Azure Blob Storage
  - Data source name: coffee-customer-data
  - Data to extract: Content and metadata
  - Parsing mode: Default
  - Connection string: *Select Choose an existing connection. Select your storage account, select the coffee-reviews container, and then click Select.
  - Managed identity authentication: None
  - Container name: this setting is auto-populated after you choose an existing connection.
  - Blob folder: Leave this blank.
  - Description: Reviews for Fourth Coffee shops.
![Screenshot 2024-04-05 095129](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/a68f4c93-1eff-4b40-9cab-3a2c8ddb13dc)
![Screenshot 2024-04-05 095141](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/85de3428-5746-4f60-9ea1-2c69838a84ab)
![Screenshot 2024-04-05 095200](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/5d0c966f-1a77-4577-b2a7-c90c933c3c94)
![Screenshot 2024-04-05 095235](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/475817cd-c34a-4e89-8536-dac4298957f2)
- Clique em **Next: Add cognitive skills (Optional).** e aguarde a validação.
![Screenshot 2024-04-05 095248](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/41451714-ea40-4591-b985-443221d766f4)
- Selecione o seu AI Service.
![Screenshot 2024-04-05 095409](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/b3789593-8aad-4625-8f9f-bedbdb3dd7e7)
- Na seção **Add enrichments**:
  - Mudar o Skillset name para coffee-skillset.
  - Selecione o checkbox **Enable OCR and merge all text into merged_content field**.
  - Source data field: merged_content.
  - Selecione Enrichment granularity level como **Pages (5000 character chunks)**.
  - Não selecione Enable incremental enrichment
- Select the following enriched fields:
  - Cognitive Skill		
  - Extract location names	=> 	locations
  - Extract key phrases	=> 	keyphrases
  - Detect sentiment	=> 	sentiment
  - Generate tags from images	 => 	imageTags
  - Generate captions from images	 => 	imageCaption
![Screenshot 2024-04-05 095435](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/1e015362-5aa1-4cae-aceb-031d30349251)
![Screenshot 2024-04-05 095634](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/dbdfeeff-dae3-4764-9721-c3ce3e16b2d0)
- Dentro de **Save enrichments to a knowledge store**, selecione:
  - Image projections
  - Documents
  - Pages
  - Key phrases
  - Entities
  - Image details
  - Image references
  - Container name: knowledge-store.
![Screenshot 2024-04-05 100231](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/85579973-0ad1-41e8-9803-e15a22ca4ca3)
- Siga esses passos para selecionar a **Storage Account Connection String**
  - Clique **Choose an existing connection**. Escolha a storage account que criamos.
  - Clique em **+ Container** para criar um novo contêiner chamado **knowledge-store** com o nível de privacidade definido como **Provate** e clique em **Create**.
  - Selecione o contêiner de **knowledge-store** e clique em **Select**  na parte inferior da tela.
![Screenshot 2024-04-05 095913](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/94929ca7-908a-418b-b92f-befb115ca51b)
![Screenshot 2024-04-05 095950](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/9c21d6c2-f4bb-4352-9fb1-c52a31bd1ee1)
![Screenshot 2024-04-05 100013](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/39441f03-ff9b-43b3-9a49-ed9164577045)
- Clique em **Next: Customize target index.**
![Screenshot 2024-04-05 100231](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/85579973-0ad1-41e8-9803-e15a22ca4ca3)

- Em **Customize target index**
  -  Index name: coffee-index.
  -  Key: metadata_storage_path
  -  Certifique que os checkboxs estão iguais ao da imagem
- Clique em **Next:Create an indexer**
![Screenshot 2024-04-05 100346](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/986b4015-afb8-4784-b1e1-a9e520f738a1)

- Nessa tela final preencha  
  -  name: coffee-indexer.
  -  Schedule: Once
  -  Selecione o checkbox **Base-64 Encode Keys**
- Clique em **Submit**
![Screenshot 2024-04-05 100431](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/02ddddd3-b9c4-4f45-901e-85d87f2d669b)

## STEP 07
- Apos o Submit do Import Data, dentro do AI Search, clique em **Search explorer**
- No index vamos usar o **coffee-index**, vamos preencher a query com os valores dados pela documentação e clicar em **Search**
![Screenshot 2024-04-05 100506](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/df7c57db-957d-4576-8ebd-6f7ed714b9f5)

- search=*&$count=true
![Screenshot 2024-04-05 100608](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/1e1e653b-98c7-4b47-a170-6a97f8219338)

- search=locations:'Chicago'
![Screenshot 2024-04-05 100742](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/114c7e91-f858-4b5e-8fd9-655f0fd92375)

- search=sentiment:'negative'
![Screenshot 2024-04-05 100806](https://github.com/c23b/Dio-MS-ai900-DP04-CognitiveSearchAzure/assets/12342627/42dd4427-bda9-4c61-b5f0-2b797fd56b3d)

## Concluções
- Essa ferramenta de IA nos da abertura para consultar dentro de qualquer área de conhecimento que esteja em documentos, livros, artigos entre outros que estejam em arquivos digitais.
- Hoje dentro do Azure podemos utilizar essa ferramenta em features que tem como objetivo dar performance em rotinas de procura de informações e pesquisa em arquivos.
