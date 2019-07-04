# TesisUNETLaTeX
Formato LaTeX para realizar la propuesta de tesis y el informe final de tesis en la UNET

Este formato fue creado con el propósito de facilitar la realización de la propuesta de tesis y el informe final de tesis utilizando LaTeX,
el formato utilizado se estableció tomando en consideración el instructivo TAP de la UNET del año 2012.

## Requisitos

- Los packages necesarios deberían ser descargados automáticamente por la distribución Tex que se este utilizando, de no ser el caso, proceder
a la descarga manual tomando en cuenta los packages que se utilizan en el archivo dependencias.tex

- Uno de los packages utilizados es minted, por tanto, es obligatorio tener Python instalado con la librería pygments, esto se puede
realizar con pip:

```
pip install Pygments
```
- El ejecutable de Pygments, Pygmentize, deberá estar en el PATH de variables del sistema operativo correspondiente.
- Se debe agregar el comando de lanzamiento a pdflatex:

```
--shell-scape
```

- En este formato se utiliza el package biblatex, por tanto, se debe establecer en el editor de Tex el uso de Biber como backend de bibliografía,
la secuencia recomendada de compilación para que todo salga bien es:

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

Por otro lado, se agrego en la carpeta un archivo llamado Plantillas.tex, este archivo contiene snippes de códigos latex para agregar:
- Ecuaciones
- Figuras
- Tablas
- PDF's
- Citas
- otros

Para agregar fuentes de citas, se deben agregar en el archivo referencias.bib, adicionalmente, se agrego el archivo bibliografía.bib en caso de querer generar una, para el caso del formato UNET, no se requiere de bibliografía, solo referencias.

Autor: Kleiver Carrasco

Correo: kleiver615@gmail.com
