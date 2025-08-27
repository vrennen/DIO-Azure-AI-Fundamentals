# Passo a passo de criação de workspace
1. Faça login no portal do Azure em https://portal.azure.com usando suas credenciais Microsoft
2. Selecione + Criar recurso, pesquise por "Machine Learning" e crie um novo recurso Azure Machine Learning usando as configurações padrão e selecionando um nome único para o workspace
3. Selecione Review + criar e então Criar. Aguarde o workspace ser criado e então abra-o

# Treinar um modelo
1. No recurso do workspace do Azure Machine Learning, selecione *Abrir Estúdio* e selecione seu workspace recém criado
2. Abra a página *Automated ML*
3. Crie um novo serviço *Automated ML* com as seguintes configurações:
    Experiment name: mslearn-bike-rental
    Task type: Regression
    Data Type: Table
    Data Source: From local file
    MLtable selection: Insira os arquivos que pode ser baixado em https://aka.ms/bike-rentals
4. Selecione *Create*. Após a criação do dataset, selecione para continuar o envio do serviço
5. Aguarde o serviço finalizar.

# Testar o modelo
1. No Machine Learning studio, selecione Endpoints e abra o endpoint *predict-rentals*.
2. Abra a aba Test.
3. No campo *Input data to test endpoint*, substituia o JSON exemplo com os dados do arquivo *input_endpoint.json*
4. Clique no botão Test.
5. Avalie os resultados de teste, que deve incluir um resultado previsto similar ao do arquivo *output_endpoint.json*

E assim foi possível testar o modelo de Machine Learning do Azure. Você pode modificar as configurações ou deletar caso não queira mais utilizar aquele modelo
