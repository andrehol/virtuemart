***********
M�dulo de integra��o PagSeguro para VirtueMart
v.1.0
***********


= Descri��o =

Este m�dulo tem por finalidade integrar o PagSeguro como meio de pagamento dentro da plataforma VirtueMart.


= Requisitos =

Joomla 2.5.9 + VirtueMart 2.0.18


= Instala��o =

1. Na �rea administrativa do seu sistema, v� at� o menu "Extens�es > Gerenciador de Extens�es";
2. Na aba Instalar aparecer� a op��o "Enviar Pacote de Arquivos", onde voc� dever� clicar em "Selecionar Arquivo", o qual abrir� uma janela para que voc� selecione em seu sistema o arquivo .zip do plugin PagSeguro. Ap�s selecionado, clique em "Upload & Instalar";
3. Nesse momento, o plugin ser� importado para o sistema e instalado, necessitando apenas de algumas configura��es para que funcione corretamente;
4. Agora, v� at� o menu "Extens�es > Gerenciador de Plugins", busque por "pagseguro", selecione o m�dulo PagSeguro e clique na op��o ativar. Agora seu plugin estar� ativo para o Sistema.


= Configura��o =

1. Acesse "Componentes > VirtueMart", no menu que for exibido ao lado, clique em "Loja" e depois "M�todos de Pagamento". Clique na op��o "Novo", preencha os campos com as informa��es que desejar e selecione para o campo "M�todo de Pagamento" o m�todo de pagamento "PagSeguro". N�o se esque�a de manter a op��o "Publicado" como "Sim". Clique em salvar;
2. Agora, na aba "Configura��o", ser�o exibidas as seguintes op��es de configura��o necess�rias para o funcionamento do plugin:
2.1. logotipos (Opcional): Logotipos a serem exibidos com o nome do m�todo de pagamento
2.2. email (Obrigat�rio): E-mail cadastrado no PagSeguro
2.3. token (Obrigat�rio): Token cadastrado no PagSeguro
2.4. codifica��o de caracteres (Obrigat�rio): codifica��o do sistema (UTF-8 ou ISO-8859-1)
2.5. url de redirecionamento: url utilizada para se fazer redirecionamento ap�s o cliente realizar a efetiva��o da compra no ambiente do PagSeguro. Pode ser uma url do pr�prio sistema ou uma outra qualquer de interesse do vendedor
2.6. gravar log (Opcional): define se ser�o gerados logs para as transa��es do seu sistema com o PagSeguro. Caso seja definido como "Sim" e preenchido o campo de nome do log, ser� gerado um log no diret�rio logs do sistema, caso o campo de nome do log n�o esteja preenchido, o log ser� gerado do diret�rio da lib do PagSeguro, dentro de /plugins/vmpayment/pagseguro/PagSeguroLibrary com o nome de PagSeguro.log
2.7. Nome do arquivo de log (Opcional): Nome dado ao arquivo de log. Ex.: log_pagseguro.log


= Changelog =

v1.0
Vers�o inicial. Integra��o com API de checkout do PagSeguro.


= NOTAS =
	
	- Certifique-se que o email e o token informados estejam relacionados a uma conta que possua o perfil de vendedor ou empresarial.
	- Certifique-se que tenha definido corretamente o charset de acordo com a codifica��o (ISO-8859-1 ou UTF-8) do seu sistema. Isso ir� prevenir que as transa��es gerem poss�veis erros ou quebras ou ainda que caracteres especiais possam ser apresentados de maneira diferente do habitual.
	- Para que ocorra normalmente a gera��o de logs pelo plugin, certifique-se que o diret�rio e o arquivo de log tenham permiss�es de leitura e escrita.
	- O PagSeguro somente aceita pagamento utilizando a moeda Real brasileiro (BRL).