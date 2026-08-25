# Donut 3D em ASCII (C)

Implementação do clássico Donut 3D renderizado inteiramente no terminal. Este projeto é um motor de computação gráfica de baixo nível espremido em poucas linhas de C, operando sem nenhuma interface gráfica ou biblioteca externa de vídeo.

**Como funciona sob o capô:**
* **Projeção 3D para 2D:** Utiliza matemática pura (trigonometria) para calcular as coordenadas de rotação do toroide no espaço.
* **Z-Buffer (Profundidade):** Implementa um buffer na memória para garantir que apenas a parte frontal do objeto seja desenhada, criando o efeito de solidez.
* **Iluminação (Raytracing simples):** Calcula a incidência de "luz" em cada ponto, mapeando o resultado para uma string de caracteres (`.,-~:;=!*#$@`) para simular sombras e volume.
