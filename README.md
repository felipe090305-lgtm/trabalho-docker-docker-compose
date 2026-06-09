# Docker e Docker Compose
## O que é Docker? Explique o conceito de container e como o Docker resolve o problema do "funciona na minha máquina"
Docker é uma plataforma utilizada para criar, executar e gerenciar contêineres. Um container é um ambiente isolado que contém tudo o que uma aplicação, sistema ou software precisa para funcionar, como bibliotecas, dependências, configurações e arquivos do projeto. O Docker resolve o problema do “na minha máquina funciona”, pois permite que a aplicação, sistema ou projeto sejam executados no mesmo ambiente (container) em qualquer computador ou servidor que possua o Docker instalado. Dessa forma, diferenças entre sistemas operacionais, versões de bibliotecas ou configurações não afetam o funcionamento da aplicação, tornando o ambiente mais padronizado e confiável.


## Imagem vs Container. Qual a diferença entre os dois conceitos?
Imagem é como um modelo contendo instruções necessárias para criar um ambiente de execução, uma espécie de receita que diz como o container será criado. Já o container em si é uma instância de uma imagem em execução. Quando o Docker inicia uma imagem, um container é criado e passa a funcionar. Dá para pensar que a imagem é a parte mais difícil de se fazer, pois é como se fosse o passo a passo do que devemos fazer para a aplicação funcionar. Já o container é tudo isso pronto, tudo já mastigado. Como exemplo, podemos pensar que a imagem funciona como uma receita, enquanto o container é essa receita sendo executada.

## O que é um Dockerfile? O que é e para que serve?
Dockerfile é um arquivo de texto que contém instruções que o Docker usa para criar uma imagem. Nele é possível definir uma imagem base, copiar arquivos do projeto, instalar dependências e configurar comandos de inicialização da aplicação. O Dockerfile automatiza a criação de imagens e garante que o ambiente possa ser reproduzido de forma consistente em diferentes máquinas.

## O que é Docker Compose? O que é, quando usar e qual problema ele resolve?
Docker Compose é uma ferramenta utilizada para gerenciar aplicações compostas por múltiplos containers. Ele é usado quando um projeto depende de vários serviços trabalhando juntos, como aplicação, banco de dados e sistema de cache. O principal problema que o Docker Compose resolve é a complexidade de iniciar e configurar vários containers manualmente. Ao invés de executar vários comandos separados, toda a configuração fica centralizada em um único local. É como se ele encurtasse o trabalho, iniciando tudo o que a aplicação precisa em um único lugar.

## Exemplo Prático Descreva com suas palavras o que acontece quando executamos “docker compose up”
Quando esse comando é executado, o Docker Compose faz a leitura do arquivo e verifica quais serviços precisam ser iniciados. Logo após, ele baixa as imagens necessárias, cria os containers, configura a rede e os volumes e inicia os serviços automaticamente. Quando executamos o comando docker compose up, o Docker Compose lê o arquivo docker-compose.yml para verificar quais serviços precisam ser iniciados. Após isso, ele verifica se as imagens necessárias já existem no computador. Caso não existam, ele realiza o download ou cria as imagens automaticamente. Em seguida, o Docker cria os containers definidos no arquivo, configura redes e volumes, estabelece a comunicação entre os serviços e inicia tudo automaticamente. Por exemplo, em uma aplicação que utiliza uma API e um banco de dados, apenas o comando docker compose up é suficiente para iniciar ambos os serviços e permitir que eles se comuniquem corretamente. Isso facilita o desenvolvimento, reduz a quantidade de comandos necessários e torna a configuração do ambiente mais simples e organizada.

## Referências
- https://docs.docker.com/get-started/docker-overview/
- https://docs.docker.com/compose/
- https://www.ibm.com/br-pt/topics/docker
- https://aws.amazon.com/pt/docker/
