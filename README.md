Jquery-Price-Format
===================

jQuery Price Format Plugin is a plugin to format input text fields as prices. For example, if you type 123456, the plugin updates it to US$ 1,234.56. It is costumizable, so you can use other prefixes and separators (for example, use it to get R$ 1.234,55).


Formatação de campo moeda (money) com jQuery Price Format
Um snippet javascript bem simples para formatar campos do tipo moeda / dinheiro.
Usarei o plugin jQuery Price Format. Ele possui varias configurações interessantes como quantidade de casas decimais, caractere usado para separar dezenas e milhares, prefixo, e outras que estão documentadas no site do autor: http://meiaduzia.com.br/cuducos2/priceformat/
Veja como é simples:
Inserindo os scripts necessários (jQuery + o plugin):

<script type="text/javascript" src="jquery-1.5.min.js"> </script>
 <script type="text/javascript" src="jquery.price_format.1.3.js"></script>

Configurando a formatação do campo:
<script type="text/javascript">
  $(document).ready(function(){
      $('#valor').priceFormat({
        prefix: 'R$ ',
        centsSeparator: ',',
        thousandsSeparator: '.'
      });
    });
  </script>

Neste exemplo, ativei a formatação no campo com id “valor”:

Dinheiro: <input type='text' id='valor' name='valor'/>

Poderia ser utilizada outro selector id em vez do ID do elemento, para aplicarmos a formatação em diversos campos da página.
