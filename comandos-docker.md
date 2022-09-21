# Principais comandos

## Como iniciar um container (que ainda não existe)
'''
    docker run NOME-DA-IMAGEM

    docker run docker/getting-started

'''

## listar container que estão em execução
'''
    docker ps
'''

## para stop a execução de um container
'''
    docker stop NOMEDOCONTAINER

    docker stop vigilant_bose
'''

## iniciar um container que já existe 
'''
    docker start NOMEDOCONTAINER

    docker start vigilant_bose
'''

## para remover um container (container deve estar parado)
'''
    docker rm NOMEDOCONTAINER

    docker rm vigilant_bose
'''

# estipular o nome de um container

Obs: exemplo na criação do container

'''
    docker run  --nane NOMEDOCONTAINERDESEJO NOMEDAIMAGEM
  
    docker run --name nekodocker docker/getting-started
'''

# redirecionar a requisição da máquina hospedeira para um container docker

Obs: exemplo na criação do container


```
    docker run  --name NOMEDOCONTAINERDESEJO -p PORTA-HOSPEDEIRO:PORTA-CONTAINER  NOMEDAIMAGEM

    docker run --name nekodocker -p 80:80  docker/getting-started