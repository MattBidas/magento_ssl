# Magento2 2.1.5 SSL

> Este Modelo de Módulo foi criado por [Billie Thompson aka. PurpleBooth](https://gist.github.com/PurpleBooth).
> Para obtê-lo vá em: https://github.com/AOEpeople/Magento-2-Module-Skeleton

Magento2 2.1.5 - Módulo para Injeção de Dependência para ajuste do erro ao inserir produto quando 
usado o protocolo HTTPS/SSl.

## Como usar

Baixe ou clone o projeto para obter os arquivos.

## O que preciso

- Magento2 2.1.5
- PHP7 >=
- Apache2.2 >=
- Acesso ao Painel de Administração de sua Loja Virtual.
- SSL configurado ou acesso do item acima para configurar 

## Instalação

Após obter os arquivos, você necessita configurar o nome para qual você utiliza no seu projeto.
Para isso substitua onde está Module_Skeleton ou Module\Skeleton para o de seu uso e copie para a pasta do seu Magento2.

## Quais arquivos devo alterar ?

Os arquivos citados na instalação são:
- module.xml
- registration.xml
- di.xml (onde está  type="Module\Skeleton\SSL\Identifier" altere para o caminho de seu uso.)

### Requisitos para utilização do Módulo

Após configurar o nome/caminho do Módulo é preciso executar os comandos:
Certifique-se que está na raiz do seu projeto Magento2, exemplo: /var/www/html/

> Limpar o diretório dos arquivos usado pelos módulos e injeções de dependência
```
sudo rm -rf var/generation/* var/di/*
```

> Instalar o módulo
```
php bin/magento setup:upgrade
```
> Gerar os arquivos e injetar as dependências so módulo
```
php bin/magento setup:di:compile
```

> Se o seu Magento2 Cache está habilitado , limpe através do comando :
```
php bin/magento cache:clean
```

## Duvidas, problemas, sugestões

* Abra uma Issue com seu questionamento/dúvida

