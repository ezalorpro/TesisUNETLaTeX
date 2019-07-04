# TesisUNETLaTeX
Formato LaTeX para realizar la propuesta de tesis y el informe final de tesis en la UNET

Este formato fue creado con el proposito de facilitar la realizacion de la propuesta de tesis y el informe final de tesis utilizando LaTeX,
el formato utilizado se establecio tomando en consideracion el instructivo TAP de la UNET del año 2012.

## Requisitos

- Los packages necesarios deberian ser descargados automaticamente por la distribucion Tex que se este utilizando, de no ser el caso, proceder
a la descarga manual tomando en cuenta los packages que se utilizan en el archivo dependencias.tex

- Uno de los packages utilizados es minted, por tanto, es obligatorio tener Python instalado con la libreria pygments, esto se puede
realizar con pip:

```
pip install Pygments
```
- El ejecutable de Pygments, Pygmentize, debera estar en el PATH de variables del sistema operativo correspondiente.
- Se debe agregar el comando de lanzamiento a pdflatex:

```
--shell-scape
```

- En este formato se utiliza el package biblatex, por tanto, se debe establecer en el editor de Tex el uso de Biber como backend de bibliografia,
la secuencia recomendada de compilacion para que todo salga bien es:

```
pdflatex -> biber -> pdflatex
```

## Uso y recomendaciones

Para utilizar el formato basta con abrir principalPropuesta.tex o principalTesis.tex, estos archivos son el archivo principal para realizar
la propuesta de tesis o el informe final de tesis respectivamente, debido a que la estructura de archivos utiliza varios niveles (nested files)
es recomendable agregar al comando de llamado de pdflatex la orden:

```
-recorder
```

Por otro lado, se agrego en la carpeta un archivo llamado Plantillas.tex, este archivo contiene snippes de codigos latex para agregar:
- Ecuaciones
- Figuras
- Tablas
- PDF's
- Citas
- otros


Autor: Kleiver Carrasco

Correo: kleiver615@gmail.com
