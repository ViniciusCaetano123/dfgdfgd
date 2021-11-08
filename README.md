# Filtragem no domínio espacial II

<strong>Exercicio 1</strong>

![focalizada](https://user-images.githubusercontent.com/42754908/140666481-d2c8b7b9-c4c8-4c05-91a2-e1e71bf9e678.png)<br>
Para solução do exercicio foi utilizado  como referência  o programa addweighted.cpp. A imagem acima começa desfocada, e quando se mexe na seta ela será "focada" na medida que se altera ela. Para realizar o desfoque na imagem, chamamos a função medianBlur que passa a imagem de entrada- na qual, uma linha acima foi convertida para CV_32FC3-, uma imagem de saida e no ultimo parametro um valor- quanto maior esse valor, maior será o desfoque.
![wei](https://user-images.githubusercontent.com/42754908/140666740-0ce5d8c9-8ef7-48ee-bcdd-f0e64865e2c7.png)
