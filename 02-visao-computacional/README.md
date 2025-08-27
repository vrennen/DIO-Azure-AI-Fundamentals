# Passo a passo de criação de workspace
1. Faça login no portal do Azure em https://portal.azure.com usando suas credenciais Microsoft
2. Selecione + Criar recurso, pesquise por "Azure AI services" e crie um novo plano. Configure com a região mais próxima fisicamente de você e o nível de preço em Standard S0.
3. Selecione Review + criar e então Criar. Aguarde o workspace ser criado e então abra-o

# Conectar o serviço Azure AI ao Vision Studio
1. Em outra aba, abra o *Vision Studio* em https://portal.vision.cognitive.azure.com
2. Entre com sua conta e selecione *View all resources*.
3. Na página de seleção de recurso para trabalhar, marque a checkbox com o nome de recurso e selecione *Select as default resource*.
4. Feche a página de configurações

# Detectar rostos
1. Na página do *Vision Studio*, selecione a aba *Face* e então a opção *Detect Faces in an image*.
2. Aceite os termos de uso na seção *Try It Out*.
3. Selecione as imagens de amostra e observe os dados retornados.
4. Teste agora com novas imagens! Baixe o arquivo de exemplo em https://aka.ms/mslearn-detect-faces
5. Extraia o conteúdo do arquivo baixado e faça upload das imagens de exemplo e veja os dados de detecção facial retornados. Note que o serviço Azure AI não detecta rostos que estejam obstruídos

# Reconhecimento Ótico de Caracteres (OCR)
1. Na página do *Vision Studio*, selecione a aba *Optical character recognition* e então a opção *Extract text from images*.
2. Aceite os termos de uso na seção *Try It Out*.
4. Teste com novas imagens! Baixe o arquivo de exemplo em https://aka.ms/mslearn-ocr-images
5. Extraia o conteúdo do arquivo baixado e faça upload das imagens de exemplo e veja os dados de detecção facial retornados. Em *Detected attributes*, qualquer texto encontrado fica estruturado numa hierarquia de regiões, linhas e palavras.
6. Observe que na imagem, o texto encontrado é destacado por uma caixa.

E assim foi possível testar o modelo de detecção de imagens do Azure. Você pode modificar as configurações ou deletar caso não queira mais utilizar aquele modelo
