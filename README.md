# Histograma![equalizada](https://user-images.githubusercontent.com/42754908/136682234-e7a65a0f-ac9a-4458-9679-dd6ce1fcb5e9.png)

<strong>Exercício 1</strong>.<br>
Foi utilizado o imread para pode ler a imagem(foi utilizado imagem porque eu estava sem webcam) e uma conversão para grayscale.
Para a inclusão do histograma atravez da imagem, foi modicicado o programa base histogram.cpp e incluido outras funções, que foram possiveis atraves de outros exemplos
de programa feito com imagens. 
Para realizar a equalização da imagem, foi utilizada a função equalizeHist, um método para melhorar o constrate da imagem, ele estica o intervalo dos pixels agrupados. Segue uma imagem de exemplo-tirada do google:
![images](https://user-images.githubusercontent.com/42754908/136681489-6b11b2f3-6042-45c4-8c20-49b45b7566a0.jpg)<br>
Função equalizeHist:<br>
![euqlizada](https://user-images.githubusercontent.com/42754908/136700455-b7a15725-fcee-4d0c-a6f3-7f0ee87ffc7d.png)

<br>
Defini duas imagem(um original e a outra que sofrerá a equalização) com suas alturas e larguras, e tambem foi colocado o CV_8UC1 para as imagens serem criadas para representar 8 bits por pixel. <br>
Temos duas funções calcHist, uma para a imagem sem a equalização e a outra com. Essa função serve para calcular o histograma da imagem.Tambem temos a função normalize para cada umas das imagem, ela vai servir para aumentar o constrate e remover ruídos da imagens<br>
![caclHis](https://user-images.githubusercontent.com/42754908/136700970-c9fa9827-3aee-4ce4-a271-8e1f3809aacb.png)

<br>
Depois o setTo para setar todos os pixels para um canal unico-utilizando o Scanlar(0).<br>

![scaler](https://user-images.githubusercontent.com/42754908/136700949-7f8a4682-7505-481b-bc98-d7e21d925181.png)

 
 Para realizar a exibição do histograma, foi utlizado a função line-para exibir as linhas do histograma- e a função react para exibir um retangulo no lado esquerdo superior da tela. 
![salvar](https://user-images.githubusercontent.com/42754908/136700936-23097312-edfe-4019-8b80-2934ccfdd023.png)
<strong>Exercício 2</strong>.<br>
Já que estou fazendo com comparação de duas imagem. Vamos comparar as duas, em vez de um video que é frame por frame, ou, "imagem" por "imagem".
Utilizamos a função compareHist, colocando duas imagem, uma com equalizada e a outra não. Já que foi espeficicado o CV_COMP_CORREL, quanto mais longe o histograma tiver, 
séra retornado 1 e quanto mais perto será -1.

![final2](https://user-images.githubusercontent.com/42754908/136710691-48e3c90d-f55d-40f9-9bce-8b03a8744b2e.png)



