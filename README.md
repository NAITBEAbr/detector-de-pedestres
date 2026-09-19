# Detector de pedestres

Detecta pessoas caminhando em um vídeo e desenha um retângulo em volta de cada uma,
quadro a quadro.

## Como funciona

1. O OpenCV abre o vídeo `walking.avi` e lê um quadro por vez
2. Cada quadro é convertido para escala de cinza, que é o formato esperado pelo
   classificador
3. O classificador em cascata Haar (`haarcascade_fullbody.xml`) procura corpos inteiros
   na imagem
4. Para cada corpo encontrado, um retângulo verde é desenhado sobre o quadro exibido

A tecla espaço encerra o programa.

## Tecnologias

- Python
- OpenCV — leitura do vídeo e classificador Haar em cascata

## Como executar

```bash
pip install opencv-python
cd Projeto118
python Walkers.py
```

O vídeo de exemplo e o arquivo do classificador já estão na pasta `Projeto118`.
