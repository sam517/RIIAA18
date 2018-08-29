# RIIAA Escuela18

Repo para la escuela de verano de la RIIAA 2018

<p align="center">
<img src="extra/poster_web_escuela.png">
</p>

## Requisitos

1. [Python 3.6 (anaconda)](https://www.anaconda.com/download/)
2. Paquetes descritos dentro de `requirements.txt` o `environment.yml`.

[google colaboratory](https://colab.research.google.com/notebooks/welcome.ipynb#recent=true). Con google colaboratory no se necesitan los requerimientos (2,3,4).


### Con Anaconda: Crear un conda environment

Desde una terminal, estando en la carpeta donde se encuentra **environment.yml**, corres el comando:
```
conda env create -f environment.yml
```

### Con pip
Desde una terminal, estando en la carpeta donde se encuentra **requirements.txt**, corres el comando:
```
pip install -r requirements.txt
```

### Con Docker
Puedes construir una imagen docker, es decir un ambiente virtual via el siguiente comando
```
docker build -t "riiaa18" .
```
y luego para correr el ambiente docker en la carpeta favorita de tu eleccion usas el comando
```
docker run -it --rm -p 8890:8888 -v $(pwd):/home/jovyan/work  riiaa18
```
