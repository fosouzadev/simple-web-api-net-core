# Estudo de constru��o de imagem docker para Web Api

## Construir imagem
Utilizando o terminal, entre na pasta raiz do projeto e execute o seguinte comando:
```
docker build -t fosouzadev/simple-web-api:1.0.0 .
docker build -t fosouzadev/simple-web-api:latest .
```

## Construir e executar container
Utilize o seguinte comando para criar e executar o container da aplica��o:
```
docker run -d -p 8080:8080 --name simple-web-api simple-web-api:latest
```

## Requisi��o de teste
Fa�a uma requisi��o para o endpoint abaixo para testar o funcionamento da aplica��o.
```
GET http://localhost:8080/Sum/Number1/5/Number2/6
```