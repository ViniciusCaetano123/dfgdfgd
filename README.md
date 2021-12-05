# Quantização vetorial com k-means
                                                

 ![narutoGif](https://user-images.githubusercontent.com/42754908/144731340-4c97bb65-f38c-4d7f-8a09-688a381f8dd3.gif)  ![tangen](https://user-images.githubusercontent.com/42754908/144731428-32e974e4-616a-4df0-9e3b-8e87df967da2.gif) ![shigeno](https://user-images.githubusercontent.com/42754908/144731497-9f36039d-5b52-4fc8-a86c-7adbd38a21ff.gif)
<b>Explicação do algoritmo de cluster</b>: Os algoritmos de clustering trabalham com pontos de dados, e o k-means não é diferente, precisamos inicializar os centróidespontos de dados que ficam no centro do cluster. Cada centróide representa um grupo. Para cada ponto do conjunto de dados, o algoritmo irá calcular a distância entre esse ponto de dado aos centróides definidos e atribuir esse ponto ao grupo mais próximo a ele.
![kma](https://user-images.githubusercontent.com/42754908/144767972-ce92ef7d-fe71-4d21-aaac-7c6c64e51f67.png)
Conforme o exercicio, foi pedido que  foste realizo 10 rodadas, para isso criamos um for que vai até 10, onde cada rodada aplicaremos o algoritmos k-means  na imagem.
onde será passado, a imagem, o numeros de clusters, os "critérios", para que quando esses criterios foram satisfeito, o algoritmo é interrompido, numero de vezes que o algoritmo é executado e a especificação dos centroides como parametro. No final do programa, salvamos essa imagem com a função imwrite. E para exibir o resultado,mostraremos um gif das 10 imagens clusterizadas.



