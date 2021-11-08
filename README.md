# Filtragem no domínio espacial II

<strong>Exercicio 1</strong>

![focalizada](https://user-images.githubusercontent.com/42754908/140666481-d2c8b7b9-c4c8-4c05-91a2-e1e71bf9e678.png)<br>
Para solução do exercicio foi utilizado  como referência  o programa addweighted.cpp, repositorios do github, pdfs e videos. A imagem acima começa desfocada, e quando se mexe na seta ela será "focada" na medida que se altera a seta. Para realizar o desfoque na imagem, chamamos a função medianBlur que passa como primeiro parametro a imagem de entrada - na qual, uma linha acima foi convertida para CV_32FC3-, no segundo parametro uma imagem de saida e no ultimo parametro um valor- quanto maior esse valor, maior será o desfoque. Logo em seguida, chamamos a função createTrackbar, na qual essa função ira ser chamada para atualizar o valor da variavel base na posição do controle deslizante. O primeiro parametro é um char de 50 caracteres, o segundo é o proprio nome da janela, o terceiro é um ponteiro, o quarto é o valor maximo da altura, e por ultimo uma função CallBack on_trackbar_blend(onde passa um função por parametro)
![wei](https://user-images.githubusercontent.com/42754908/140666740-0ce5d8c9-8ef7-48ee-bcdd-f0e64865e2c7.png)
