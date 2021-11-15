# Filtragem no domínio da frequência


<strong>Exercicio 1</strong><br>

![imagemFiltrada](https://user-images.githubusercontent.com/42754908/141846796-2032d90f-9766-48b9-b968-6b2a2beab6cd.png)

![imagem_teste_2](https://user-images.githubusercontent.com/42754908/141848601-62af150b-dd43-4448-8a13-5497fd5486c3.png)

Foi utilizado o programa exemplos/dft.cpp como ponto de partida para a resolução de problemas. Foi implementado o filtro homomórfico para melhorar a qualidade da iluminação das imagens. Veja que ambas as imagens do lado esquerdo estão escuras, quando o controle deslizando das quatro opções são deslizadas pro lado direito, a um ganho de iluminação, contraste e realce da imagem.<br>
![Create](https://user-images.githubusercontent.com/42754908/141861391-00dddbdc-5d62-4b3a-a6b3-667eeaf4d1e3.png)<br>
Na imagem acima, criaremos 4 controles deslizantes para a aplicação do filtro. onde todas vão ter um limite de até 500 para o filtro. <br>
![filtra](https://user-images.githubusercontent.com/42754908/141860624-0d07ab39-48de-44ce-b477-84b9eca6a82b.png)<br>
A imagem acima aplica uma função de filtragem que será aplicada em cada pixel da imagem, percorrendo toda imagem. Para obter o resultado da imagem filtrada, utilziamos uma função matematica que está no código acima. Conforme o wikipedia, "aplicar transformada de Fourier na imagem  realizando-se em seguida a filtragem desejada e depois calculando-se a transformada inversa de Fourier para obter o resultado da imagem filtrada".

<h3> Bibliografia </h3>
https://pt.wikipedia.org/wiki/Filtragem_no_dom%C3%ADnio_da_frequ%C3%AAncia
https://pt.wikipedia.org/wiki/Transformada_de_Fourier

