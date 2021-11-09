# Filtragem no domínio espacial II


<strong>Exercicio 1</strong><br>
![focalizada](https://user-images.githubusercontent.com/42754908/140828904-ffe59962-f20f-4ffd-a6ba-dbe469685b9f.png)
<br>
Para solução do exercicio foi utilizado  como referência  o programa addweighted.cpp, repositorios do github, pdfs e videos. A imagem acima começa desfocada, e quando se mexe na seta ela será "focada" na medida que se altera a seta. Para realizar o desfoque na imagem, chamamos a função medianBlur que passa como primeiro parametro a imagem de entrada - na qual, uma linha acima foi convertida para CV_32FC3-, no segundo parametro uma imagem de saida e no ultimo parametro um valor- quanto maior esse valor, maior será o desfoque. <br>Logo em seguida, chamamos a 4 funções createTrackbar(3 createTrackbar novas para a resolução do exercicio), onde vai ser criada o slider(controle deslizante,tipo uma "seta pra baixo" pra mexer ela na barrinha) , na qual á função on_trackbar_blend  ira ser chamada para atualizar/setar quando voce deslizar a setinha. O primeiro parametro é um char de 50 caracteres, o segundo é o proprio nome da janela, o terceiro é um ponteiro, o quarto é o valor maximo da altura(esse valor vai começar em 100, mas tambem pode ser modificado pra 200 ou até mais, apenas segui o padrão do anterior que era 100, caso mude pra 200, voce podera deslizar a setinha até o valor 200), e por ultimo uma função CallBack(onde passa um função por parametro) on_trackbar_blend. E por ultimo irá salvar o resultado da imagem utilizando a função imwrite<br>
![inclinar](https://user-images.githubusercontent.com/42754908/140828572-1c7299ee-211a-4e62-bb58-c4f98510c8e5.png)
<br>
Como avia falado anteriormente, quando voce deslizar a setinha, a função on_trackbar_blend será chamada. Essa função ira calcular a altura,declinio,posicao_um,slider,posicao_dois, para depois dentro do for, a variavel  alpha(uma variavel muito importate) vai receber um calculo matematico que vai ser responsavel por aplicar os efeitos<br>
![alpha](https://user-images.githubusercontent.com/42754908/140782865-050abf94-7277-4835-a6ff-42fccc148c53.png)<br>

Criei uma função atribuir, onde será passado o x, y e o alpha. Logo em seguida irá ser atribuido  na posição x e y da matriz de pixel o efeito<br>![atribuir](https://user-images.githubusercontent.com/42754908/140783461-ed36867d-7bec-4744-a3f1-03c67d72d0e7.png)<br>

<strong>Exercicio 2</strong><br>
![exercicio2](https://user-images.githubusercontent.com/42754908/140839923-3fc27907-d0dd-4a37-bf32-1c22f0a3da09.png)
<br>
![dois](https://user-images.githubusercontent.com/42754908/140840527-f896ef9d-1887-46b4-ba00-70ccfadf02cf.png)<br>
As duas imagens aqui acima, representa dois frame do video que vai estar no repositorio.<br>
Primeiro vamos abrir um video que foi baixo do youtube e pegamos a altura e largura dele. criamos a variavel densidade, na qual ela vai atuar como uma opacidade dos quadrados de baixo e de cima do efeito blur. Clocamos duas instancia da class Mat com suas largura e altura respecitvas e conversando ela pra CV_8UC1.<br>
![saida](https://user-images.githubusercontent.com/42754908/140847161-effb61e5-362f-4f17-a823-64708910aefc.png)
<br>
Na imagem abaixo vamos percorer a matriz de pixel, para cada interação vamo setar o valor negativo que seria represetando com o sinal de menos. No proximo for, vamos percorrer a matriz de pixel novamente e pra cada pixel da imagem, vamo aplicar a principal função alpha que retornara um valor e será aplicado na matriz. Chamamos a função cvtColor para converter para CV_GRAY2RGB. Aplicar o loop no while, chamamos a função medianBlur para aplicar o blur na imagem e tambem á multiply, como o proprio nome já diz, ela via multiplar duas "imagem", na qual vão ser passada pelo parametro um e dois, o terceiro parametro é a varivel de resultado entre a multiplicação das duas. Depois chamamos a função addWeighted para mesclar os resultados da multiplicação feita coma  função multiply. E depois exibimos ela com a função inshow.<br>
![parte2](https://user-images.githubusercontent.com/42754908/140843961-d2aef514-3a94-47a7-8f9f-6db1abbe05bc.png)
