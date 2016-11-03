## Jupyter Notebook

Para rodar o container, execute
`docker docker run -p 8888:8888 -v /my/notebook/dir:/home/jovyan/work -d -P jupyter/[docker-stack]`

Onde:
- **/my/notebook/dir**: diretório local onde será salvo os *notebooks*
- **docker-stack**: container que será executado. Para saber quais containers estão disponíveis, consulte https://github.com/jupyter/docker-stacks

Existe um outro container com o kernel iTorch instalado:
- docker run -v /my/notebook/dir:/root/dev -it --rm -p 8888:8888 dhunter/itorch-notebook
