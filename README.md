# Prova1Camputacaonuvem

# Prova 1 de Computação em nuvem
Nome: Elywelton ferreira nunes  RA - ECBA0899FD31127082B4

## Oque eu fiz

Executei uma página web em um contêiner Docker chamado loja.
Usei a imagemnginx:alpine e a porta 8081 do ambiente.

## Verificação do contêiner:

root@ubuntu:~$ docker ps
CONTAINER ID   IMAGE          COMMAND                  CREATED              STATUS              PORTS                                     NAMES
1b3c0270493f   nginx:alpine   "/docker-entrypoint.…"   About a minute ago   Up About a minute   0.0.0.0:8081->80/tcp, [::]:8081->80/tcp   loja

## Teste da página

root@ubuntu:~$ curl http://localhost:8081
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<title>Loja</title>
</head>
</body>
<h1>Loja no ar</h1>
</body>
</html>

## Explicação 

Com minha palavras qual é a diferença aentre a nginx:alpine e o contêiner loja? para que serviu o mapeamento 8081:80?

nginx:alpine é como uma caixinha pronta com o Nginx dentro.
loja é o nome da caixinha funcionando.
A porta 8081 manda para a porta 80 do Nginx, e o Nginx entrega o seu index.html.

