# Filtragem no domínio espacial I

![filtro](https://user-images.githubusercontent.com/42754908/138572502-b91cd37b-3ef0-4bf8-aad3-3f8e8ac3f73f.png)
O codigo foi retirado do exemplos/filtroespacial.cpp do material disponibilizado , e acrescendo  uma varialvel laplgauss do tipo flot, para  quando perccorer a matriz(imagem) consegui aplicar o filtro utlizando a função matematica. Percorrendo pixel a pixel e utlizando essa variavel para fazer o calculo e o deslocamento.
![lap](https://user-images.githubusercontent.com/42754908/138573368-028da325-d743-4b9a-9276-8b64c6a004fd.png)<br>
Se for teclado a letra P, será chamada a função Mat, passando tamanho 5x5 em ponto flutuante(CV_32F), e tambem como o ultimo parametro a varivel laplgauss, logo após chamamos a função printmask, passando  a instancia que foi criada, na qual essa função vai percorrer toda a matriz e aplicar em cada pixels o feito.
![p](https://user-images.githubusercontent.com/42754908/138611445-34ef35b1-a68a-4180-b935-d4c2e47c65e9.png)
