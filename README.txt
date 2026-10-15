# Medidor de Abertura de Dossel - UFOPA

Algoritmo desenvolvido em Python para calcular a percentagem de passagem de luz e abertura do dossel através do processamento digital de imagens. 

Esta ferramenta utiliza Visão Computacional (OpenCV) para separar as áreas de céu e folhagem, quantificando a cobertura vegetal. Pesquisa vinculada à Universidade Federal do Oeste do Pará (UFOPA).

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23403386.svg)](https://doi.org/10.5281/zenodo.23403386)

# Pré-requisitos e Bibliotecas

O script foi otimizado para o Google Colab e utiliza as seguintes bibliotecas principais:
* `opencv-python` (cv2)
* `numpy`
* `matplotlib`
* `pandas`

##  Como Funciona o Algoritmo

1. **Carregamento:** Solicita o upload das fotos do dossel.
2. **Processamento:** Extrai o canal azul da imagem (RGB) para maximizar o contraste.
3. **Binarização:** Aplica o método de Limiarização de Otsu com um ajuste fino (offset) para isolar com precisão a passagem de luz.
4. **Quantificação:** Calcula a percentagem exata de pixels claros em relação ao total da imagem, gerando uma tabela de resultados e uma comparação visual.

##  Como Citar

Se utilizar este código na sua pesquisa, por favor, cite-o seguindo o padrão ABNT:

> > V.A.Michelon.Pereira *Script de Visão Computacional para Medição de Abertura de Dossel*. Versão 1.0. Santarém, PA: Zenodo, 2026. Software. Disponível em: <https://doi.org/10.5281/zenodo.23403386>.

##  Licença

Este projeto está sob a licença MIT.
