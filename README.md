# Detecção de bordas com o algoritmo de Canny

![pontilhado_canny](https://user-images.githubusercontent.com/42754908/143772396-e9fc7c78-d508-454e-994a-5e46adac524c.png)<br>
Acima temos uma 3 imagens. O resultado da primeira imagem é do algoritmo de canny e segundo é do  pontilhismo, na qual, ambos foram disponibilizado no material de referencia.
O ultimo resultado, foi a junção do canny e pontilhismo.

![principal](https://user-images.githubusercontent.com/42754908/143956836-81bee379-c99d-4c40-ae65-e73dfb7a0694.png)<br>
Para a criação do pontilhismo, utilizamos a função circle para criar um circulo na imagem, passando como parametro a imagem, onde o circulo vai ser desenhado, a posição do
circulo, o raio do circulo, a cor do circulo e a espessura dele, isso dentro do for, percorrendo sua matriz e calculando suas posições x e y.
Para a criação do pontilhismo junto com canny, utilizamos a função Canny para detecção de bordas percorrendo sua matriz, verificando se o valor da confição é 255(branco),
para aplicação a função circle descrita acima.
