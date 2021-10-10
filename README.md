# Histograma![equalizada](https://user-images.githubusercontent.com/42754908/136682234-e7a65a0f-ac9a-4458-9679-dd6ce1fcb5e9.png)

Exercício 1.
Foi utilizado o imread para pode ler a imagem(foi utilizado imagem porque eu estava sem webcam) e uma conversão para grayscale.
Para a inclusão do histograma atravez da imagem, foi modicicado o programa base histogram.cpp e incluido outras funções, que foram possiveis atraves de outros exemplos
feito com imagens. 
Para realizar a equalização da imagem, foi utilizada a função equalizeHist, um método para melhorar o constrate da imagem, ele estica o intervalo dos pixels agrupados. Segue uma imagem de exemplo-tirada do google:
![images](https://user-images.githubusercontent.com/42754908/136681489-6b11b2f3-6042-45c4-8c20-49b45b7566a0.jpg)
Defini duas imagem(um original e a outra que sofrerá a equalização) com suas alturas e larguras, e tambem foi colocado o CV_8UC1 para a imagens serem criadas com   para representar 8 bits por pixel. 
Temos duas funções calcHist, uma para a imagem sem a equalização e a outra com. Essa função serve para calcular o histograma da imagem.Tambem temos a função normalize para cada umas das imagem, ela vai servir 






