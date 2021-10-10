# Histograma![equalizada](https://user-images.githubusercontent.com/42754908/136682234-e7a65a0f-ac9a-4458-9679-dd6ce1fcb5e9.png)

<strong>Exercício 1</strong>.<br>
Foi utilizado o imread para pode ler a imagem(foi utilizado imagem porque eu estava sem webcam) e uma conversão para grayscale.
Para a inclusão do histograma atravez da imagem, foi modicicado o programa base histogram.cpp e incluido outras funções, que foram possiveis atraves de outros exemplos
feito com imagens. 
Para realizar a equalização da imagem, foi utilizada a função equalizeHist, um método para melhorar o constrate da imagem, ele estica o intervalo dos pixels agrupados. Segue uma imagem de exemplo-tirada do google:
![images](https://user-images.githubusercontent.com/42754908/136681489-6b11b2f3-6042-45c4-8c20-49b45b7566a0.jpg)<br>
Função equalizeHist:
![euqlizada](https://user-images.githubusercontent.com/42754908/136700455-b7a15725-fcee-4d0c-a6f3-7f0ee87ffc7d.png)

<br>
Defini duas imagem(um original e a outra que sofrerá a equalização) com suas alturas e larguras, e tambem foi colocado o CV_8UC1 para a imagens serem criadas com   para representar 8 bits por pixel. <br>
Temos duas funções calcHist, uma para a imagem sem a equalização e a outra com. Essa função serve para calcular o histograma da imagem.Tambem temos a função normalize para cada umas das imagem, ela vai servir para aumentar o constrate e remover ruídos da imagens<br>

![image,sa](https://user-images.githubusercontent.com/42754908/136682293-bbfb353f-725e-4d1f-b3a1-3eb612bad1a7.png)<br>
Depois o setTo para setar todos os pixels para um canal unico-utilizando o Scanlar(0).<br>
![scaler](https://user-images.githubusercontent.com/42754908/136682552-331044d8-7053-49bb-a094-7eeff951c4ca.png)
 
 Para realizar a exibição do histograma, foi utlizado a função line-para exibir as linhas do histograma- e a função react para exibir um retangulo no lado esquedo superior da tela. 
![final](https://user-images.githubusercontent.com/42754908/136682625-9669275d-b7b1-4903-b6d9-0c1167281bd2.png)



