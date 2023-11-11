# <h1 align="center"> Pesquisa Permissões e Sensores - PAMI</h1>
### <h3 align="center"> Pedro Santos Pequini e Matheus Kevin   </h3>
 
### <h3 align="center">  2° DESENVOLVIMENTO DE SISTEMAS </h3>



<br>
<br>  


## Tópicos:

### Actions para uso em Intents Implícitas - Sensores Diponíveis -Principais Permissões 

<br>
<br>


## Actions para uso em Intents Implícitas

 Em tradução livre, Actions significa "ações" e isto se confirma na prática, já que elas são responsáveis por realizar ações tanto com interferência do usuário (dando opções de escolha), como executando tarefas diretas. Ou seja, podem estar contidas em intents explícitas e implícitas, porém, as que serão mencionadas são especialmente implícitas, onde é uma ação em um sentido mais "amplo", como por exemplo, um compartilhamento, que pode ter diferentes destinos e que será definido pela preferência do usuário. Actions são recursos recorrentes nas aplicações, e algumas comuns são:

 1.1 **ACTION_VIEW**: Essa Action pode ser atribuida a diversas ações de visualização, porém, a mais comum e que facilmente é encontrada no mercado, é a visualização de mapas, definindo a latitude, longitude e o zoom para a exatidão da coordenada que desejar. essa Action é capaz de levar o usuário a abrir um mapa (o que ele escolher) e navegar por ele.

 <br>

 1.2 **ACTION_DIAL**: Action que ao ser acionada, o "Telefone" ou discador do dispositivo é acionado e aberto fora da aplicação, sendo possível já definir o número discado previamente na programação. Caso esteja nulo, a própria pessoa pode discar, assim ficando de livre escolha. É importante destacar que não efetua diretamente a chamada, apenas deixa a ligação pronta para ser efetuada.
 
  <br>
	
 1.3 **ACTION_WEB_SEARCH**: A característica mais marcante é a possibilidade do usuário fazer uma pesquisa pré-definida na programação, no navegador que será aberto, ou seja, assim que for executada, já faz a pesquisa de forma automática. 

  <br>
	
1.4 **ACTION_INSERT**: Também relacionado ao Telefone do smartphone, o insert pode ser usado com a finalidade de inserir contatos novos, abrindo o aplicativo telefônico e criando um contato com seu nome, número, e informações adicionais. Esta "Action" depende de "Extras" para fazer com que as informações sejam direcionadas a cada campo.

 <br>
	
 1.5 **ACTION_CALL**: A primeira informação necessária para entender essa Actin, é que ela faz uso de uma permissão chamada "CALL_PHONE" no arquivo de manifesto já que é uma ação que usa o hardware. diferente da ACTION_DIAL, a 'CALL' não só disca como realmente faz a efetuação da chamada para o número que for definido. Pode ser usada em telas suporte por exemplo, ajudando o cliente a ligar diretamente.

  <br>
	
1.6 **ACTION_CHOOSER**: Adicionada desde a primeira API, exibe um seletor de atividades, que permite escolha. Pode substituir tranquilamente o seletor de atividades padrão que é exibido pelo sistema, com uma lista de lugares que podem ser acessados para finalizar a ação.

 <br>


## Sensores Diponíveis  
Um sensor pode exercer muitas funcionalidades e por isso tem grande eficácia. Existem muitos tipos que usamos rotineiramente e que correspondem a estímulos diferentes, como por exemplo: calor, pressão, luz, e outros. Após receber esses estímulos, a sua função é retornar algo a ser interpretado por dispositivos. Pensando no calor, o sensor deve aferir a temperatura e retornar um valor que dependerá da unidade que será medida, por exemplo, em C° ou F°.
	Pensando de uma forma mais ampla, os sensores estão presentes em diversos locais como indústrias, empresas, comércios, mercados, e o mais comum, nas residências. Cada área aplica-os da forma que mais lhes forem úteis e na programação de aplicativos mobile não é diferente. Já que os sensores dos smartphones podem ser acessados por meio do Android Studio para desenvolver aplicações.   

<br>

 2.1 **Sensores Disponíveis**
	Analisando todas as diversas versões dispostas pelo Android, vemos que esse ambiente de desenvolvimento possui uma vasta lista de sensores  que podem ser usados já que suporta diferentes dispositivos. Pensando nos smartphones, os principais contidos no aparelho que podem ser utilizados, são:   
	
2.2 **Aceleração Linear**: Faz a medição da força de aceleração na unidade "m/s²" acionada em um dispositivo desprezando a gravidade. Pode ser usado em aplicações que medem a aceleração exclusiva de um eixo

 <br>

 2.3 **Acelerômetro**: Presente desde as primeiras versões de API do Android, esse sensor complementa alguns outros como o Giroscópio para sistemas de coordenadas, já que ele detecta movimentos, agitações e inclinações. O que retorna, é a força de aceleração do movimento, em "m/s²" nos eixos x, y e z.

  <br>
	
2.4 **Gravidade**: Com nome sugestivo, podemos ter base do que se é medido. Com esse sensor, é possível medir a força da gravidade, também seguindo as características do Acelerômetro, retornando em unidades de medida "m/s²" dependendo da alteração da gravidade aplicada ao dispositivo, nos eixos três eixos convencionais (x, y e z).

  <br>
  
2.5 **Giroscópio**: Presente em todos os smartphones da era atual, sempre está presente como um dos recursos que aparecem nas fichas técnicas disponibilizadas pelas distribuidoras. Tem grande utilidade em sistemas de coordenadas pois detecta rotações, voltas e etc. Mostra exatamente a taxa de rotação que o dispositivo teve em "rad/s" para cada um dos três eixos, x, y e z.

  <br>
  
2.6 **Humidade Relativa**: Sensor não tão conhecido mas que tem muitas funcionalidades. Dentre elas, a capacidade de monitorar um ponto de condensaçãoe umidade relativa presente no ar. O retorno é em "%".

  <br>
  
 2.7 **Luz**: Sensor que é capaz de medir o nível de luz, claridade, em um ambiente (retornando em unidade "lx"). Conhecido pela função da realização do controle automático do brilho da tela de acordo com a claridade externa. Acessando a câmera frontal, é possível fazer este controle;

  <br>
  
2.8 **Orientação**: Sensor que mede os graus de rotação que um dispositivo e pode ser combinado com outros dois sensores (de campo geomagnético e gravidade) com o método "getRotationMatrix()" para aplicações como determinação da posição do dispositivo.

  <br>
  
2.9 **Pressão**: Sua unidade retornada é hPa ou mbar, e é um sensor essencial pelo seu uso específico para acompanhamento das mudanças ocorridas na pressão do ar.

   <br>
   
2.10 **Proximidade**: Com esse sensor, é possível fazer a medição da proximidade que um objeto tem, da tela do smartphone. Ainda que imperceptível, ele é utilizado em muitos aparelhos e seu objetivo mais comum é desligar ao aproximar-se do rosto em uma chamada por exemplo, muito útil para as pessoas que optam por receber chamadas com o celular no ouvido para amplificar sua audição.

 <br>
	
2.11 **Temperatura Ambiente**: Implementado na API 14, este sensor tem a função de fazer um monitoramento da temperatura do ar, aferindo-a em C° sempre que solicitado pela aplicação;

 <br>

2.12 **Categorias de Sensores**   

2.12.1 **Sensores de movimento**   
	Sensores de movimento estão presentes em uma gama de aplicações e softwares que funcionam através do movimento direcionado ao smartphone, como rotações, inclinações, mudanças de velocidade, entre outros. Simplificando, eles medem grandezas físicas nos três eixos (x, y e z).
	  
2.12.2 **Sensores de ambientais**   
	Está relacionado os fenômenos naturais. Para entender melhor esses sensores, é bom pensarmos, por exemplo, no termômetro, que pode tanto calcular a temperatura ambiente, como também a temperatura presente no hardware. Isso só é possível graças aos sensores que têm a função de medir parâmetros ambientais, ou seja, relacionados a natureza.	
	
2.12.3 **Sensores de posição**   
	Orientação é um sensor que compõe essa categoria, sendo utilizado em aplicativos que se baseiam na posição física do usuário. Exemplificando, podemos citar a aplicação Google Maps, que utiliza os sensores de posição para saber a sua localização atual da pessoa, para assim, lhe dar um norte para onde ela deseja ir.   

 <br>
 <br>

## Principais Permissões  

Antes de tudo, devemos explicar o que é um permissão, que se baseia em elementos que garantem a segurança da privacidade do usuário, protegendo dados restritos, como o estado do sistema e os dados de contato dos usuários, e também ações restritas, como a conexão a um dispositivo pareado e a gravação de áudio. Algumas permissões são permitidas automaticamente quando a aplicação é instalada, e outras obrigam que o app solicite ao usuário uma permissão para ser executada, que são chamadas de permissões de execução. Mas na realidade, existem uma variedade grande de permissões, contendo vários tipos de categorias, como: 

3.1.1 **Permissões da instalação**   
Esse tipo de permissão permite que o app tenha acesso limitado a dados restritos, e também podem permitir que o aplicativo execute ações restritas que afete o sistema de outros aplicativos.

<br>

3.1.2 **Permissões normais**   
São possivelmente o tipo mais comum de permissões utilizadas em aplicações, pois autorizam o acesso a dados/ações que vão além da sandbox da aplicação, mostrando pouco risco à privacidade do usuário.

<br>

3.1.3 **Permissões de assinatura**   
Essa permissão permite uma assinatura a um aplicativo quando ele é assinado pelo mesmo certificado do aplicativo ou do sistema operacional que definiu a devida permissão. São geralmente utilizados em aplicativos que implementam serviços privilegiados, como preenchimento automatico ou VPN.

<br>

3.1.4 **Permissões de execução**  
Também sendo conhecidas como "permissões perigosas", permitem que o aplicativo tenha acesso extra a dados restritos, e também podem autorizar que ele efetue ações restritas que afetam mais significamente o sistema de outro aplicativo, por essa razão, é necessário solocitar as permissões de execução antes de acessar os dados/ações restritos.

<br>

3.1.5 **Permissões especiais**
São baseadas em operações de aplicativos específicos, sendo apenas possivel de utilizar, quando for definido pela própria plataforma e os OEMs, e geralmente são elas que definem permissões especiais pelo fato de proteger o acesso à ações significativas, um exemplo clássico que podemos citar é sobrepor outros aplicativos.

<br>

3.2 **Principais Permissões**  

3.2.1 **Internet**   
A permissão "android.permission.INTERNET" permite que a aplicação tenha acesso à rede de internet.
<br>

3.2.2 **Acesss_network_state**   
A permissão "android.permission.ACCESS_NETWORK_STATE" permite que a aplicação tenha acesso a informação sobre as redes, como conectividade.
<br>

3.2.3 **Câmera**   
A permissão "android.permission.CAMERA" permite que o aplicativo tenha acesso à câmera do dispositivo, seja para tirar fotos, ou gravar vídeos.
<br>

3.2.4 **Read_external_storage e Write_external_storage**   
As permissões "android.permission.READ_EXTERNAL_STORAGE" e "android.permission.WRITE_EXTERNAL_STORAGE" basicamente permitem que o app tenha acesso a ler e escrever no armazenamento externo, como um cartão SD por exemplo.
<br>

3.2.5 **Acess_fine_location e Acess_coarse_location**   
As permissões "android.permission.ACCESS_FINE_LOCATION" e "android.permission.ACCESS_COARSE_LOCATION" se baseiam em o aplicativo acessar informações sobre a localização do dispositivo, seja exata ou aproximada.
<br>
 
3.2.6 **Record_audio**   
A permissão "android.permission.RECORD_AUDIO" basicamnte permite que o aplicativo tenha acesso ao microfone do dispositivo.
<br>

3.2.7 **Bluetooth**   
A permissão "android.permission.BLUETOOTH" permite que a aplicação tenha acesso ao bluetooth do dispositivo.
<br>

3.2.8 **Read_contacts e Write_contacts**   
As permissões "android.permission.READ_CONTACTS" e
"android.permission.WRITE_CONTACTS" permite que o app leia e digite/escreva nos contatos do dispositivo.
<br>

3.2.9 **Send_sms e Receive_sms**   
As permissões "android.permission.SEND_SMS" e
"android.permission.RECEIVE_SMS" permitem que a aplicação possa enviar e receber mensagens de SMS em seu dispositivo.
<br>

 ## Referências Bibliográficas   

https://www.eletrogate.com/sensores-e-modulos#:~:text=Um%20sensor%20%C3%A9%20um%20dispositivo,de%20medi%C3%A7%C3%A3o%20e%2Fou%20monitoramento.  

https://www.devmedia.com.br/utilizando-o-framework-de-sensores-no-android/32362  

https://developer.android.com/guide/topics/sensors/sensors_overview?hl=pt-br  

https://developer.android.com/reference/android/content/Intent#ACTION_CHOOSER  

https://developer.android.com/guide/components/intents-common?hl=pt-br  

https://developer.android.com/guide/topics/manifest/action-element?hl=pt-br  

https://developer.android.com/guide/topics/permissions/overview?hl=pt-br   

https://www.techtudo.com.br/listas/2021/12/5-permissoes-de-aplicativos-que-voce-deve-pensar-bem-antes-de-aceitar.ghtml   




