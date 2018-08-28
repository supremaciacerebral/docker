[checkmark]: https://raw.githubusercontent.com/mozgbrasil/mozgbrasil.github.io/master/assets/images/logos/logo_32_32.png "MOZG"
![valid XHTML][checkmark]

[getcomposer]: https://getcomposer.org/
[uninstall-mods]: https://getcomposer.org/doc/03-cli.md#remove

# Docker

## Sobre o Docker

xxxx

## Iniciando o Docker

    cd ~/dados/dockers/devilbox

    docker-compose up

## Monitoramento de imagens e processos

    docker --version && docker images && docker images ps && docker ps

## Acessar o DevilBox

http://localhost/

## Paralisar o DevilBox

Pressione control + C

## Para uso após a reinicialização da máquina

    cd ~/dados/dockers/devilbox

    docker-compose down --remove-orphans

    cd ~/dados/dockers/devilbox

    docker-compose up

Ao reiniciar a máquina é carregado o servidor apache mas não o banco de dados devendo executar o comando acima.

## Configurando o DevilBox

Edite o arquivo docker-compose.yml

php & http

 # Mount volumes related to ln -s htdocs
 - /home/marcio/dados/:/home/marcio/dados/
