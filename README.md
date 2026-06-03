# Docker e Docker Compose
## O que é Docker? Explique o conceito de container e como o Docker resolve o problema do "funciona na minha máquina"
Docker é uma plataforma utilizada para criar, executar e gerenciar contêiners. Um container é um ambiente isolado que contêm tudo que uma aplicação, sistema, software precisa pra funcionar. Como por exemplo bibliotecas, dependências, configurações e arquivos do projeto. O Docker acaba resolvendo o problema do “na minha máquina funciona”, pois permite que a aplicação, sistema, projeto sejam executado no mesmo ambiente (container), em qualquer computador ou servidor que possua o Docker instalado fazendo com que problemas como diferenças de sistemas operacionais, versões de  bibliotecas ou configuração não afetem o funcionamento da aplicação. Docker e Docker Compose são ferramentas muito utilizadas no desenvolvimento de software moderno. Elas ajudam desenvolvedores a criar ambientes padronizados para executar aplicações em diferentes computadores e servidores. Com essas ferramentas, é possível reduzir problemas de compatibilidade e facilitar a implantação de sistemas. Atualmente, Docker e Docker Compose são amplamente utilizados por empresas e profissionais da área de tecnologia, em conclusão, podemos dizer que Docker e Docker Compose são ferramentas importantes para o desenvolvimento moderno. Elas ajudam a reduzir problemas de compatibilidade, simplificam a configuração de ambientes e tornam o processo de desenvolvimento mais organizado. Por esse motivo, são amplamente utilizadas por empresas e desenvolvedores em diversos tipos de projetos.


## Imagem vs Container. Qual a diferença entre os dois conceitos?
Imagem são como um modelo contendo instruções necessárias para criar um ambiente de execução, uma espécie de receita que diz como o container vai ser criado. Já o container em si é uma instancia de uma imagem em execução, quando o Docker inicia uma imagem, é criado um container e passa a funcionar. Da pra pensar que a imagem é o mais difícil de se fazer pois é como se fosse o passo a passo de como e oque devemos fazer para a aplicação funcionar, já o container já é tudo isso feito, tudo já mastigado, como por exemplo, da pra pensar que a imagem funciona como uma receita, enquanto o container é essa receita sendo executada..

## O que é um Dockerfile? O que é e para que serve?
Dockerfile é um arquivo de texto que contêm instruções que o Docker usa para criar uma imagem. Sendo possível definir imagem base, copiar arquivos do projeto, instalar dependências e configurar comandos de inicialização da aplicação. O Docker file automatiza a criação de imagens e garante que o ambiente possa ser reproduzido de forma consistente em diferentes máquinas. 

## O que é Docker Compose? O que é, quando usar e qual problema ele resolve?
Docker Compose é uma ferramenta utilizada para gerenciar aplicações compostas por múltiplos containers. Ele é usado quando um projeto depende de vários serviços trabalhando juntos, como aplicação, banco de dados e sistema de cache. O principal problema que o Docker composse resolve é a complexidade de iniciar e configurar vários containers manualmente. Ao invés de executar vários comandos separados, toda a configuração fica centralizada em um único local. Como se ele encurtasse o trabalho iniciando tudo que que a aplicação precisa em um único lugar.

## Exemplo Prático Descreva com suas palavras o que acontece quando executamos “docker compose up”
Quando esse comando é executado o Docker compose faz a leitura do arquivo e verifica quais serviços precisam ser iniciados, logo após ele baixa as imagens necessárias, cria os containers, configura a rede e volumes e inicia os serviços automaticamente.

## Referências
- https://docs.docker.com/get-started/docker-overview/
- https://docs.docker.com/compose/
- https://www.ibm.com/br-pt/topics/docker
- https://aws.amazon.com/pt/docker/
