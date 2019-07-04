### Projeto simples com gradle e docker

Para executar o programa, é preciso ter o Docker e o Gradle instalado.

No diretório do projeto, execute:
`./gradle build`
para que o maven crie o projeto com suas dependências

depois
`./gradle build docker`
para criar a imagem do docker

utilizando
`docker images`
é possível ver a imagem criada (com.example/hello-docker)

para subir o projeto, utilize:
`docker start com.example/hello-docker`

para parar o projeto, encontre o id da imagem com 
`docker ps`
(a155e4166c99	com.example/hello-docker)

e por fim
`docker stop a155e4166c99`
