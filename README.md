# Projeto: Encontre o Marcos

## Descrição
"Encontre o Marcos" é um projeto de aprendizado de máquina que utiliza técnicas de reconhecimento facial para identificar o Marcos em um conjunto de imagens. O objetivo é treinar um modelo com várias fotos do Marcos e, posteriormente, usar esse modelo para detectar o Marcos em novas fotos de teste.

## Estrutura do Projeto

1. **Coleta de Imagens**
   - As imagens de treinamento estão armazenadas na pasta `marcos/`.
   - As imagens de teste estão na pasta `encontre/`.

2. **Pré-processamento**
   - Detecção de faces nas imagens usando um classificador Haar Cascade.
   - Recorte das faces detectadas e salvamento na pasta `cropped_faces/`.

3. **Treinamento do Modelo**
   - Uso do modelo `LBPHFaceRecognizer` do OpenCV para treinar com as imagens de faces recortadas.

4. **Teste e Avaliação**
   - Uso do modelo treinado para prever se o Marcos está presente nas imagens de teste.
   - Marcação das faces detectadas com um retângulo verde se a predição for positiva.

## Pré-requisitos

- Google Colab
- Python 3.x
- OpenCV
- Matplotlib
- NumPy

