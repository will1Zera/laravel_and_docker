<div align="center">
    <br>
    <h1 align="center">Laravel e Docker</h1>
    <p align="center">
        <a href="#sobre-o-desafio">Sobre</a> | 
	    <a href="#ambiente-local">Ambiente</a>
    </p>
</div>
<br>

## Sobre o desafio
Foi criado um projeto de Laravel com composer e configurado um ambiente docker utilizando uma imagem php

##### Pré requisitos:
- <a href="https://getcomposer.org/download/">Composer</a>

## Ambiente local
Foi criado um projeto em Laravel com o seguinte comando:

```sh
composer create-project laravel/laravel laravel_and_docker
```

Em seguida, foi configurado os arquivos Dockerfile e nginx.conf e criado uma imagem docker com o seguinte comando:

```sh
docker build -t laravel_and_docker .
```

Por fim, foi preciso rodar a imagem docker:

```sh
docker run -d -p 9002:80 laravel_and_docker
```

<br>
by <a href="https://github.com/will1Zera">William Bierhals</a> 😄 <br>
📥 <a href="https://www.linkedin.com/in/williambierhals/">Linkedin</a>
