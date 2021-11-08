# Filtragem no domínio espacial II


<strong>Exercicio 1</strong>

![focalizada](https://user-images.githubusercontent.com/42754908/140666481-d2c8b7b9-c4c8-4c05-91a2-e1e71bf9e678.png)<br>
Para solução do exercicio foi utilizado  como referência  o programa addweighted.cpp, repositorios do github, pdfs e videos. A imagem acima começa desfocada, e quando se mexe na seta ela será "focada" na medida que se altera a seta. Para realizar o desfoque na imagem, chamamos a função medianBlur que passa como primeiro parametro a imagem de entrada - na qual, uma linha acima foi convertida para CV_32FC3-, no segundo parametro uma imagem de saida e no ultimo parametro um valor- quanto maior esse valor, maior será o desfoque. <br>Logo em seguida, chamamos a função createTrackba, onde vai ser criada o slider(controle deslizante,tipo uma "seta pra baixo" pra mexer ela na barrinha) , na qual á função on_trackbar_blend  ira ser chamada para atualizar/setar quando voce deslizar a setinha. O primeiro parametro é um char de 50 caracteres, o segundo é o proprio nome da janela, o terceiro é um ponteiro, o quarto é o valor maximo da altura(esse valor vai começar em 100, mas tambem pode ser modificado pra 200 ou até mais, apenas segui o padrão do anterior que era 100, caso mude pra 200, voce podera deslizar a setinha até o valor 200), e por ultimo uma função CallBack(onde passa um função por parametro) on_trackbar_blend.<br>
![wei](https://user-images.githubusercontent.com/42754908/140666740-0ce5d8c9-8ef7-48ee-bcdd-f0e64865e2c7.png)
<br>
Como avia falado anteriormente, quando voce deslizar a setinha, a função on_trackbar_blend será chamada. Essa função ira calcular o <br>
![alpha](https://user-images.githubusercontent.com/42754908/140782865-050abf94-7277-4835-a6ff-42fccc148c53.png)<br>

Criei uma função atribuir, onde será passados o x, y e o resultado da função alpha.<br>![atribuir](https://user-images.githubusercontent.com/42754908/140783461-ed36867d-7bec-4744-a3f1-03c67d72d0e7.png)

