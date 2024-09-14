# Atualização do App AutoescolaOnline

Um aplicativo que foi criado em 2020 e nao recebeu nenhuma atualizacao após isso pela empresa Legtransito LTDA. Refêrencia nacional com relação a Trânsito e ajudando uma imensa comunidade a conseguir se Aprovado na Prova Teórica do Detran.

O Aplicativo tem o objetivo de ajudar a comunidade a Decorar as placas de Trânsito e liberar alguns simulados para o cliente testar o seu conhecimento. Essa são as suas principais funcionalidades e sua finalidade, contando também com uma API que retornar os videos do Youtube no canal para o aplicativo sendo possivel assistir os mesmo no aplicativo, sem a necessidade de ir até o app do Youtube, e também tem o blog de notícias. 

# Atualizações que Foram Necessárias

Ao pegar o aplicativo com a liguagem Flutter que foi desenvolvida, foi necessário de 3 a 4 dias para a leitura completa da aplicação e entender como que funcionava a parte de dentro nos códigos. Após isso, fiz uma pesquisa para saber o que havia atualizado na linguagem Dart e Flutter para que pudesse estar primeiramente atualizado com a linguagem usada, e percebi que a principal era a mudança para o Null Safety do dart, que consiste que todas as variaveis e funcoes que retornem nulo seja declarada como Nula ou Não Nula. 

E então dentro aii de 2 dias, com os códigos atualizados ele já estava apto para rodar nas novas versoes do android.. Fazendo os primeiros testes, ja vi alguns erros que consistiam em não atualizar a lista de videos novos do Youtube, isso era devido a versao antiga do Dart, assim que atualizei, este problema ja foi resolvido. 

O segundo era que a parte do Blog de noticias, estava dando erro pois a requisição na API voltava sempre o 'author' como "Null", entao eu olhei no site e percebi que no cadastro, nunca usaram quem era o Autor, sempre deixando ele nulo( apesar que so tinha uma opção) logo eu simplesmente removi a variavel de author da requição e voltou a funcionar normalmente.

Esses era os principais erros que constavam no app para a funcionalidade nele. Após isso fizemos algumas modificações.. sendo elas 

# 1  Mudança no Visual

Começamos fazendo um pequeno protótipo do que seria feito nessa atualização visual. Com a ajuda de um designer fizemos esse protótipo:

#imagem

A mudança em como as questoes dos simulados apareciam para o usúario é a principal mudança, onde antigamente, as questões eram todas visualizadas de uma unica vez, sendo não tendo um total feedback se a questão foi ou não selecionada ( Por conta do Radio ). Mudei para colocar uma por vez, e o modo de seleção foi em todo o Container usando um GestureDetector para mudar de cor também quando clicado, selecionamos o amarelo, de acordo com o protótipo, e para questoes certas o verde, erradas o veremlho.. 

