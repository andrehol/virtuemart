-------------------------------------------------
M�dulo de integra��o PagSeguro para VirtueMart
v1.0
-------------------------------------------------


= Descri��o =

Com o m�dulo instalado e configurado, voc� pode pode oferecer o PagSeguro como op��o de pagamento em sua loja. O m�dulo utiliza as seguintes funcionalidades que o PagSeguro oferece na forma de APIs:

	- Integra��o com a API de Pagamentos


= Requisitos =

	- Joomla 2.5.9
	- VirtueMart 2.0.18
	- PHP 5.1.6+
	- SPL
	- cURL
	- DOM


= Instala��o =

	- Certifique-se de que n�o h� instala��o de outros m�dulos para o PagSeguro em seu sistema;
	- Baixe o reposit�rio como arquivo zip ou fa�a um clone;
	- Na �rea administrativa do seu sistema, acesse o menu Extension > Extension Manager, no campo Package File aponte para o caminho do arquivo .zip que foi baixado e em seguida selecione Upload & Install;
	- Acesse o menu Extension -> Plugin Manager, localize e selecione o m�dulo PagSeguro e em seguida defina o Status como Enabled.


= Configura��o =

Para acessar e configurar o m�dulo acesse o menu Components -> VirtueMart -> Shop -> Payment Methods -> New, preencha os dados conforme modelo a seguir:

	- Payment Name: PagSeguro
	- Published: Yes
	- Payment Description: Pague com PagSeguro e parcele em at� 18 vezes
	- Payment Method: PagSeguro
	- Shopper Group: Aqui voc� deve definir os grupos de clientes que poder�o pagar usando o PagSeguro
	- List Order: Aqui voc� deve definir a ordem em que o PagSeguro ser� exibido no checkout de sua loja


Salve as configura��es e clique na aba Configuration. As op��es dispon�veis est�o descritas abaixo.


	- e-mail: e-mail cadastrado no PagSeguro
	- token: token cadastrado no PagSeguro
	- url de redirecionamento: ao final do fluxo de pagamento no PagSeguro, seu cliente ser� redirecionado automaticamente para a p�gina de confirma��o em sua loja ou ent�o para a URL que voc� informar neste campo. Para ativar o redirecionamento ao final do pagamento � preciso ativar o servi�o de Pagamentos via API em https://pagseguro.uol.com.br/integracao/pagamentos-via-api.jhtml
	- charset: codifica��o do seu sistema (ISO-8859-1 ou UTF-8)
	- log: ativa/desativa a gera��o de logs
	- diret�rio: informe o local a partir da ra�z de instala��o do Joomla onde se deseja criar o arquivo de log. Ex.: /logs/ps.log. Caso n�o informe nada, o log ser� gravado dentro da pasta ../PagSeguroLibrary/PagSeguro.log

	Opcionalmente voc� pode mudar o relacionamento feito entre os status de pagamento no PagSeguro com os status de pagamento dentro de sua loja. Para mais informa��es acesse https://pagseguro.uol.com.br/v2/guia-de-integracao/api-de-notificacoes.html#v2-item-api-de-notificacoes-status-da-transacao


= Changelog =

	v1.0

	- Vers�o inicial. Integra��o com API de checkout do PagSeguro.


= Notas =
	
	- O PagSeguro somente aceita pagamento utilizando a moeda Real brasileiro (BRL).
	- Certifique-se que o email e o token informados estejam relacionados a uma conta que possua o perfil de vendedor ou empresarial.
	- Certifique-se que tenha definido corretamente o charset de acordo com a codifica��o (ISO-8859-1 ou UTF-8) do seu sistema. Isso ir� prevenir que as transa��es gerem poss�veis erros ou quebras ou ainda que caracteres especiais possam ser apresentados de maneira diferente do habitual.
	- Para que ocorra normalmente a gera��o de logs, certifique-se que o diret�rio e o arquivo de log tenham permiss�es de leitura e escrita.
	- D�vidas? https://pagseguro.uol.com.br/desenvolvedor/comunidade.jhtml
