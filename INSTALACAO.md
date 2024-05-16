Não há necessidades de instalar nada para que o código funcione à depender da sua IDE. A unica dependencia necessaria é o JUnit 4.13.2 e Hamcrest-core-1.3.jar.

Nós já acoplamos estas dependencias na pasta lib para que não haja necessidade para tal caso esteja utilizando o IDE Intellij. Caso esteja utilizando o Eclipse, talvez seja necessário se direcionar ao arquivo de testes, passar o mouse sobre os erros em cima dos @Test e incluir no projeto as duas dependencias citadas acima.

É muito provável que os testes unitários possam falhar no linux pois o sistema operacional utiliza de caracteres de notação de quebras de linha de maneira diferente do windows (\n vs \n\r). Como em alguns dos testes unitários usamos comparações de arquivos, pedimos que execute os testes no windows para que funcione.

Para rodar o programa basta executar a função main e todas instruções do código serão mostradas na tela.
1- Em primeira instância será pedido uma senha de inicio de votação, que deve ser uma senha de início no arquivo credentials.csv
2- Em seguida um título de eleitor válido, que está no arquivo voters.csv, deve ser inserido para que este candidato vote.
3- Serão pedidos votos de presidente e deputado.
4- Para terminar, digite -1 no momento de inserir um novo título de eleitor
5- Ensira a senha de saída que é par à senha de entrada usada. Caso erre a senha 3 vezes, a eleição é abortada por questões de segurança.