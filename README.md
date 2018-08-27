# como-criar-um-host-rust-server

<div class="row">
<div class="col-md-12">
<h1 class="hero-text"> Como Criar Rust Server dedicado? </h1>
<p class="sub-text"> O único objetivo em Rust é sobreviver. Para fazer isso, você precisará superar lutas como fome, sede e frio. Construa um fogo. Construir um abrigo. Mate animais por carne. Proteja-se dos outros jogadores e mate-os por carne. Crie alianças com outros jogadores e forme uma cidade. Faça o que for preciso para sobreviver. </p>
</div>
</div>
<hr class="narrow">
</div>
</div>
</section>

</div>
<section class="faq">
<div class="container">
<h3 class="h2 text-center">Perguntas frequentes</h3>
<div class="questions">
<div class="longform-text">
<div class="question">
<h4>O que HOST RUST SERVER?</h4>
<p class="h4">O único objetivo em Rust é sobreviver. Para fazer isso, você precisará superar lutas como fome, sede e frio. Construa um fogo. Construir um abrigo. Mate animais por carne. Proteja-se dos outros jogadores e mate-os por carne. Crie alianças com outros jogadores e forme uma cidade.</p>
</div>
<div class="question">
<h4>Como Criar Rust Server dedicado?</h4>
<div id="block-yui_3_17_2_1_1412472125855_165387" class="sqs-block html-block sqs-block-html" data-block-type="2">
<div class="sqs-block-content">
<p><span><span>Decidiu executar um Rust Dedicated Server?</span><span>A instalação e configuração do Rust Dedicated Server é muito fácil e direta.</span><span>Este guia é para a instalação de um servidor em um PC Windows.</span><span>Para Linux, confira nosso</span></span><a href="/como-criar-um-host-rust-server-em-linux"><span>Guia Como criar um servidor Rust no Linux</span></a><span>.</span></p>
</div>
</div>
<div id="block-yui_3_17_2_3_1427555213965_10044" class="sqs-block horizontalrule-block sqs-block-horizontalrule" data-block-type="47">
<div class="sqs-block-content"><hr /></div>
</div>
<div id="block-yui_3_17_2_3_1427555213965_11319" class="sqs-block html-block sqs-block-html" data-block-type="2">
<div class="sqs-block-content">
<h2><span>Requisitos de sistema</span></h2>
<p><span><span>Como uma linha de base, um mapa de 3 km quadrados (tamanho padrão do gen) gerado recentemente será executado em cerca de 2 gigabytes de RAM.</span><span>Depois de alguns testes de estresse e 150k entidades mais tarde, pode usar 6+ gigabytes de memória.</span><span>Então eu sugiro ter pelo menos 7 GB alocados por servidor.</span></span></p>
</div>
</div>
<div id="block-yui_3_17_2_3_1486311876916_19399" class="sqs-block horizontalrule-block sqs-block-horizontalrule" data-block-type="47">
<div class="sqs-block-content"><hr /></div>
</div>
<div id="block-yui_3_17_2_3_1486311876916_19461" class="sqs-block html-block sqs-block-html" data-block-type="2">
<div class="sqs-block-content">
<h2><span>Instalando e atualizando o SteamCMD</span></h2>
<p dir="ltr"><span>O SteamCMD é o console de linha de comando usado para instalar os arquivos relacionados ao Steam e o mecanismo pelo qual o servidor do Rust é instalado e atualizado.</span></p>
<ul>
<li><span>Crie uma pasta para o SteamCMD, como c:\steamcmd</span></li>
<li><span>Crie uma pasta para o servidor, como c:\rustserver</span></li>
<li><a href="https://steamcdn-a.akamaihd.net/client/installer/steamcmd.zip"><span>Baixe o</span></a><span>SteamCMD para Windows.</span></li>
<li><span>Extraia o conteúdo do arquivo zip para a pasta que você criou para o steamcmd.</span></li>
<li><span><span>Execute o programa steamcmd.exe.</span><span>(Seu computador pode pedir para você confirmar se deseja executá-lo.)</span></span></li>
</ul>
<p><span>Este arquivo, quando executado, irá baixar, instalar e atualizar para a versão mais recente do SteamCMD.</span></p>
</div>
</div>
<div id="block-yui_3_17_2_3_1459227018521_610569" class="sqs-block image-block sqs-block-image sqs-text-ready" data-block-type="5">
<div id="yui_3_17_2_1_1535287006403_152" class="sqs-block-content">
<div id="yui_3_17_2_1_1535287006403_151" class="image-block-outer-wrapper layout-caption-below    design-layout-inline">
<div id="yui_3_17_2_1_1535287006403_150" class="intrinsic">
<div id="yui_3_17_2_1_1535287006403_149" class="image-block-wrapper   has-aspect-ratio" data-description=""><img class="thumb-image loaded" src="assets/img/download.png" alt="steamcmd" data-image-dimensions="677x342" data-image-focal-point="0.5,0.5" data-load="false" data-image-id="56fa14891330bacc0f96bfd5" data-type="image" data-position-mode="standard" data-image-resolution="750w" /></div>
</div>
</div>
</div>
</div>
<div id="block-yui_3_17_2_3_1459227018521_280293" class="sqs-block html-block sqs-block-html" data-block-type="2">
<div class="sqs-block-content">
<p><span>Depois disso, você receberá o prompt Steam&gt;.</span></p>
</div>
</div>
<div id="block-yui_3_17_2_4_1485807572147_37291" class="sqs-block horizontalrule-block sqs-block-horizontalrule" data-block-type="47">
<div class="sqs-block-content"><hr /></div>
</div>
<div id="block-yui_3_17_2_4_1485807572147_37353" class="sqs-block html-block sqs-block-html" data-block-type="2">
<div class="sqs-block-content">
<h2><span>Instalando o Rust Dedicated Server</span></h2>
<p><span>Execute os seguintes comandos, um de cada vez, no prompt Steam&gt;, para iniciar o download do servidor para o seu computador.</span></p>
<pre><strong>login anonymous </strong>
<strong><span><span>force_install_dir "c:\rustserver\"</span></span><span><span>
app_update 258550</span></span><span><span>
exit</span></span>
</strong></pre>
<p><span><span>Estes são todos os arquivos necessários para um servidor “Vanilla”.</span><span>Servidores modificados exigem um pouco mais de trabalho.</span></span></p>
</div>
</div>
<div id="block-yui_3_17_2_4_1485807572147_60263" class="sqs-block horizontalrule-block sqs-block-horizontalrule" data-block-type="47">
<div class="sqs-block-content"><hr /></div>
</div>
<div id="block-yui_3_17_2_4_1485807572147_60324" class="sqs-block html-block sqs-block-html" data-block-type="2">
<div class="sqs-block-content">
<h2><span>Mudando para um ramo diferente</span></h2>
<p dir="ltr"><span>Se você deseja baixar o ramo de preparação do Rust que recebe as atualizações mais recentes, modifique o comando app_update da seguinte forma:</span></p>
<pre dir="ltr"><strong>app_update 258550 -beta staging</strong></pre>
<p dir="ltr"><span>Se você deseja baixar o ramo de pré-lançamento do Rust que recebe as atualizações futuras / de andamento do trabalho, modifique o comando app_update da seguinte forma:</span></p>
<pre dir="ltr"><strong>app_update 258550 -beta prerelease</strong></pre>
</div>
</div>
<div id="block-yui_3_17_2_2_1427561574812_11345" class="sqs-block horizontalrule-block sqs-block-horizontalrule" data-block-type="47">
<div class="sqs-block-content"><hr /></div>
</div>
<div id="block-yui_3_17_2_3_1459227018521_291004" class="sqs-block html-block sqs-block-html" data-block-type="2">
<div class="sqs-block-content">
<h2><span>Configurando e executando o servidor</span></h2>
<p><span><span>Para obter uma instância do servidor em execução, você precisa fazer pelo menos um arquivo de script em lote.</span><span>Para começar, crie um arquivo chamado RustServer.bat no diretório de instalação do servidor (c:\rustserver), clique com o botão direito e edite o arquivo.</span></span></p>
</div>
</div>
<div id="block-yui_3_17_2_3_1459227018521_289452" class="sqs-block horizontalrule-block sqs-block-horizontalrule" data-block-type="47">
<div class="sqs-block-content"><hr /></div>
</div>
<div id="block-yui_3_17_2_3_1459227018521_319368" class="sqs-block html-block sqs-block-html" data-block-type="2">
<div class="sqs-block-content">
<h2><span>O arquivo de script em lote</span></h2>
<p><span><span>Um script em lote é um documento de texto que armazena uma lista de comandos a serem executados em seqüência.</span><span>O principal uso de um script em lotes para hospedar um servidor é permitir que o proprietário do servidor verifique se o servidor está atualizado e, se o servidor travar, ele será retomado.</span><span>A maneira mais fácil de fazer isso é usando a instrução GOTO.</span><span>GOTO permitirá que você pule o script em lote para qualquer outra parte do arquivo em lote.</span></span></p>
<p><span><span>É importante notar que a Rust às vezes trava ao invés de fechar completamente.</span><span>Nesse caso, o servidor não será reiniciado se o processo parar porque o processo não foi realmente interrompido.</span><span>O script em lote aguarda a conclusão de um comando (nesse caso, o RustDedicated.exe), mas se esse processo nunca concluir o script em lote, ele apenas ficará lá.</span></span></p>
<p><span><span>Para a maior parte, você terá que configurar todas as configurações do servidor neste script em lote.</span><span>Os arquivos de configuração para o servidor ainda não funcionam, portanto definir explicitamente todas as suas configurações no script em lote é o melhor caminho a seguir.</span><span>Abaixo está um exemplo .:</span></span></p>
<pre><strong>echo off
</strong><strong>:start 
</strong><strong>C:\steamcmd\steamcmd.exe +login anonymous +force_install_dir c:\rustserver\ +app_update 258550 +quit
</strong><strong><span><span>RustDedicated.exe -batchmode +server.port 28015 +server.level "Procedural Map" +server.seed 1234 +server.worldsize 4000 +server.maxplayers 10  +server.hostname "Name of Server as Shown on the Client Server List" +server.description "Description shown on server connection window." +server.url "http://yourwebsite.com" +server.headerimage "http://yourwebsite.com/serverimage.jpg" +server.identity "server1" +rcon.port 28016 +rcon.password letmein +rcon.web 1
</span></span></strong><strong>goto start
</strong></pre>
<p><strong>Nota:</strong><span><span>Não use este exemplo sem fazer alterações.</span><span>Números de linha são mostrados apenas para referência e</span></span><strong> devem </strong><span>ser removidos.</span></p>
<p><span>Aqui está uma explicação de cada linha no arquivo em lotes.</span></p>
<p><br /><strong>echo off</strong><br /><span>Isso suprime o desejo da janela do console de exibir cada comando no arquivo em lote à medida que eles são executados.</span><br /><br /><strong>:start</strong><br /><span>O é um rótulo para um ponto inicial do loop.</span><br /><br /><strong>C:\steamcmd\steamcmd.exe +login anonymous +force_install_dir c:\rustserver\ +app_update 258550 +quit</strong><br /><span>Executa o SteamCMD para verificar as atualizações do servidor e aplicá-las, se necessário.</span><br /><br /><strong><span><span>RustDedicated.exe -batchmode +server.port 28015 +server.level "Procedural Map" +server.seed 1234 +server.worldsize 4000 +server.maxplayers 10 +server.hostname "Name of Server as Shown on the Client Server List" +server.description "Description shown on server connection window." +server.url "http://yourwebsite.com" +server.headerimage "http://yourwebsite.com/serverimage.jpg" +server.identity "server1" +rcon.port 28016 +rcon.password letmein +rcon.web 1</span></span></strong><br /></p>
<p><strong>-batchmode</strong><br /><span>Abre o Unity no modo não-GUI e elimina a necessidade de qualquer intervenção humana.</span><br /><br /><strong>+server.port 28015</strong><br /><span>Porta de conexão do cliente Rust.</span><br /><br /><strong>+server.level "Procedural Map"</strong><br /><span><span>O tipo de mapa a ser usado.</span><span>As opções são "Procedural Map","Barren",”HapisIsland”,”SavasIsland” and “SavasIsland_koth”
</span></span><br /><br /><strong>+server.seed 1234</strong><br /><span><span>Determina a forma de mapas processuais e estéreis (usados com server.worldsize).</span><span>Os valores variam de 0 a 2147483647.</span></span><br /><br /><strong>+server.worldsize 4000</strong><br /><span><span>Determina a forma de mapas processuais e estéreis (usados com server.seed).</span><span>Os valores variam de 1000 a 6000.</span></span><br /><br /><strong>+server.maxplayers 10</strong><br /><span>Número de jogadores que podem ser conectados</span><br /><br /><strong>+server.hostname "Nome do servidor conforme mostrado na lista de servidores do cliente"</strong><br /><span>Nome do servidor conforme mostrado na lista de servidores do cliente</span></p>
<p><strong>+server.description "Descrição mostrada na janela de conexão do servidor."</strong><br /><span>Descrição mostrada na janela de conexão do servidor do cliente</span><br /><br /><strong>+server.url "http://yourwebsite.com"</strong><br /><span><span>Um site válido.</span><span>Faz com que o botão "Exibir página da Web" apareça na janela de conexão</span></span><br /><br /><strong>+server.headerimage "http://yourwebsite.com/serverimage.jpg"</strong><br /><span><span>Um link válido para a imagem de fundo da janela de conexão.</span><span>Use uma imagem JPG de 512 x 256.</span></span><br /><br /><strong>+server.identity "server1"</strong><br /><span><span>O nome do diretório usado como pai para todos os arquivos do servidor.</span><span>Não use espaços ou caracteres especiais.</span></span><br /><br /><strong>+rcon.port 28016</strong><br /><span>Porta de conexão do cliente Rcon.</span><br /><br /><strong>+rcon.password letmein</strong><br /><span><span>A senha necessária para o acesso Rcon.</span><span>Não use espaços ou caracteres especiais.</span></span><br /><br /><strong>+rcon.</strong><br /><span>Usa o modo de conexão websocket para rcon (recomendado)</span><br /><br /><strong>goto start</strong><br /><span><span>Instrui o arquivo em lote a pular para o rótulo 'start'.</span><span>Remova esta linha se não quiser que o seu servidor reinicie automaticamente depois de ser desligado.</span></span></p>
</div>
</div>
<div id="block-yui_3_17_2_3_1459398029691_17902" class="sqs-block horizontalrule-block sqs-block-horizontalrule" data-block-type="47">
<div class="sqs-block-content"><hr /></div>
</div>
<div id="block-yui_3_17_2_3_1459398029691_19098" class="sqs-block html-block sqs-block-html" data-block-type="2">
<div class="sqs-block-content">
<h2><span>Conectando ao seu servidor</span></h2>
<p><span><span>Execute o Rust Client e não selecione um servidor.</span><span>Observe que seu servidor não será exibido na guia "Local Network".</span><span>Em vez disso, pressione F1 e vá para o console do cliente.</span><span>Supondo que você usou a porta padrão de</span></span><strong>28015</strong><span>, digite o seguinte comando para se conectar ao seu servidor:</span></p>
<pre><strong>client.connect localhost:28015</strong></pre>
OU
<pre><strong>client.connect ip_do_servidor:28015</strong></pre>
<p><br /><span>Se você usou uma porta diferente, altere-a de acordo.</span></p>
</div>
</div>
<div id="block-yui_3_17_2_2_1427558286432_10448" class="sqs-block horizontalrule-block sqs-block-horizontalrule" data-block-type="47">
<div class="sqs-block-content"><hr /></div>
</div>
<div id="block-yui_3_17_2_3_1427555213965_21267" class="sqs-block html-block sqs-block-html" data-block-type="2">
<div class="sqs-block-content">
<h2><span>Proprietários e Moderadores</span></h2>
<p><span><span>Quando o servidor estiver em funcionamento, você poderá optar por atribuir a propriedade a você mesmo.</span><span>Isso é feito com o</span><span>comando </span></span><strong> ownerid </strong><span><span></span><span>Você precisará do seu número SteamID de 17 dígitos.</span><span>A maneira mais fácil de obtê-lo é efetuar login e, em seguida, executar o</span><span> comando </span></span><strong> users </strong><span><span>no console.</span><span>Em seguida, insira o comando da seguinte forma:</span></span></p>
<pre><strong>ownerid 12345678901234567 AdminName</strong></pre>
<p><span>Por exemplo:</span></p>
<pre><strong>ownerid 12345678901234567 "Ricardo"</strong></pre>
<p><span><span>Você pode fazer o mesmo com moderadores usando o</span><span>comando</span></span><strong>moderatorid</strong></p>
<pre><strong>moderatorid 12345678901234567 "Admin Name"</strong></pre>
<p><span>Nota: Como com a maioria dos comandos que permitem o uso de nomes de jogadores, se o nome tiver espaços ou caracteres especiais, você deve usar aspas para conter o nome.</span></p>
<p><span><span>Certifique-se de usar o</span><span>comando</span></span><strong> writecfg </strong><span><span>depois de fazer isso e, em seguida, a pessoa deve efetuar logout e efetuar login novamente para receber as permissões.</span><span>As duas permissões são quase idênticas.</span><span>Os proprietários podem criar, expulsar e banir moderadores, se necessário, mas os moderadores não podem afetar os proprietários.</span></span></p>
</div>
</div>
<div id="block-yui_3_17_2_2_1427561574812_11537" class="sqs-block horizontalrule-block sqs-block-horizontalrule" data-block-type="47">
<div class="sqs-block-content"><hr /></div>
</div>
<div id="block-yui_3_17_2_2_1427558286432_19844" class="sqs-block html-block sqs-block-html" data-block-type="2">
<div class="sqs-block-content">
<h2><span>Compartilhando seu servidor com o mundo</span></h2>
<p><span><span>Se você deseja que outras pessoas possam se conectar ao seu servidor do mundo externo, você precisará configurar uma porta para a frente usando a porta usada acima.</span><span>Eu recomendo usar este</span></span><a href="https://cliente.widhost.com.br/knowledgebase/96/Abrir-porta-no-Firewall-Windows-Server-2008.html"><span> ABRIR PORTA NO FIREWALL WINDOWS SERVER </span></a><span><span>se você não estiver familiarizado com a configuração do encaminhamento de porta.</span><span>Você precisará encaminhar o seu "</span></span><strong>server.port</strong><span>", bem como "</span><strong>rcon.port</strong><span><span>", se usado.</span><span>Por padrão, são </span></span><strong>28015</strong><span> e </span><strong>28016.</strong></p>
<p><span><span>Mesmo que o seu servidor não apareça na lista de servidores, os jogadores podem se conectar a você por meio do</span><span> comando </span></span><strong>client.connect,</strong><span><span> se souberem do seu IP público.</span><span> Os programas de firewall locais também podem afetar a capacidade de se conectar a partir do mundo externo. </span><span>Se você suspeitar disso, desligue o firewall por alguns instantes.</span></span></p>
</div>
</div>
<div id="block-yui_3_17_2_2_1427565499613_42791" class="sqs-block horizontalrule-block sqs-block-horizontalrule" data-block-type="47">
<div class="sqs-block-content"><hr /></div>
</div>
<div id="block-yui_3_17_2_3_1427555213965_10124" class="sqs-block html-block sqs-block-html" data-block-type="2">
<div class="sqs-block-content">
<p><span><span>Mais informações podem ser encontradas no “Guia de Configuração Avançada”, em breve.</span><span>Para aqueles que desejam executar um servidor “Modded”, consulte o “Modding a Server Guide”, que será publicado em breve.</span></span></p>
<p><span>Qualquer coisa que não tenha sido abordada, consulte</span><a href="https://docs.google.com/document/d/110UCeMNogcBZrtq1NXVgFMcISbHyX51SIdoM-zPrGFA/edit?pli=1" target="_blank"><span> este documento. </span></a></p>
</div>
</div>
<div id="block-yui_3_17_2_2_1427565499613_26164" class="sqs-block horizontalrule-block sqs-block-horizontalrule" data-block-type="47">
<div class="sqs-block-content"><hr /></div>
</div>
<div id="block-yui_3_17_2_3_1459268699809_27300" class="sqs-block html-block sqs-block-html" data-block-type="2"></div>
</div>
<hr class="narrow">
<div class="question">
<p class="h4 text-center">Se você ainda tem dúvidas, ficaremos <a href="atendimento">felizes em respondê-las</a>.</p>
</div>
</div>
</div>
