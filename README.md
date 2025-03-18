# Azure AI Search: Guia de Configuração e Exploração

Este guia orienta sobre como configurar e explorar um índice de pesquisa utilizando o **Azure AI Search**, a evolução do Azure Cognitive Search, oferecendo recursos avançados de busca e inteligência artificial.

## 1. Criando os Recursos no Azure

Antes de iniciar, assegure-se de ter uma conta ativa no Azure e acesso ao [Portal do Azure](https://portal.azure.com/).

### 1.1 Criar um Serviço de Pesquisa

1. **Acessar o Portal do Azure**:
   - Faça login no [Portal do Azure](https://portal.azure.com/).

2. **Criar um Novo Recurso**:
   - No painel esquerdo, clique em "Criar um recurso".
   - Na barra de pesquisa, digite "Azure AI Search" e selecione-o.
   - Clique em "Criar".

3. **Configurar o Serviço**:
   - Preencha os campos solicitados:
     - **Nome**: Escolha um nome único para o serviço.
     - **Plano de Preços**: Selecione o plano que atenda às suas necessidades.
     - **Região**: Escolha a região mais próxima dos seus usuários.
     - **Grupo de Recursos**: Selecione um grupo existente ou crie um novo.
   - Após preencher, clique em "Revisar + Criar" e, em seguida, em "Criar" para provisionar o serviço.

## 2. Criando um Índice

1. **Acessar o Serviço de Pesquisa**:
   - No Portal do Azure, navegue até o serviço de pesquisa recém-criado.

2. **Adicionar um Índice**:
   - No menu à esquerda, selecione "Índices" e clique em "Adicionar índice".
   - Defina o esquema do índice, incluindo:
     - **Nome do Índice**: Especifique um nome para o índice.
     - **Campos**: Adicione campos como `id`, `title`, `description`, entre outros, conforme necessário.
     - **Chave Primária**: Determine o campo que servirá como identificador único.
     - **Configurações de Pesquisa**: Habilite recursos como pesquisa completa e filtros, conforme desejado.
   - Após configurar, clique em "Salvar".

## 3. Carregando Dados

### 3.1 Utilizando o Portal do Azure

1. **Acessar Indexadores**:
   - No serviço de pesquisa, vá para "Indexadores".

2. **Criar um Novo Indexador**:
   - Clique em "Adicionar indexador".
   - Escolha a fonte de dados (por exemplo, Blob Storage, SQL Database).
   - Configure os mapeamentos de campos entre a fonte de dados e o índice.
   - Defina a programação de indexação conforme necessário.
   - Salve as configurações e inicie o indexador para carregar os dados.

### 3.2 Utilizando a API REST

Para enviar dados diretamente para o índice, utilize a API REST do Azure AI Search.

## 4. Consultando Dados no Índice

### 4.1 Usando o Portal do Azure

1. **Explorar Dados**:
   - No serviço de pesquisa, selecione "Explorar dados".

2. **Executar Consultas**:
   - Escolha o índice desejado e insira os termos de pesquisa.
   - Visualize e refine os resultados conforme necessário.

### 4.2 Usando a API REST

Para realizar consultas programáticas, utilize a API REST do Azure AI Search. Para detalhes sobre como realizar essa operação, consulte a [documentação oficial do Azure AI Search](https://learn.microsoft.com/pt-pt/azure/search/search-get-started-portal).



