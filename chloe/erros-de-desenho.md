---
description: Todos os Erros que a Chloe pode encontrar!
---

# 🚨 Erros de Desenho

## Error ED01

O nome arquivo não está separado corretamente.

Os códigos de desenho são separados  por traços (-) e sublinhados (\_), conforme demonstrado na Imagem 01.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img01" alt=""><figcaption><p>Imagem 01</p></figcaption></figure>

### Solução

Renomeie o arquivo seguindo a segmentação correta.

***

## Error ED02

Bloco de Legenda está com código errado.

Na Imagem 02, o Bloco de Legenda apresenta um código diferente do que está no Nome do Arquivo. Os códigos mostrados são 1FN2\_FN-08-01, mas o correto é 1FN3\_FN-A7-01.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img04" alt=""><figcaption><p>Imagem 02</p></figcaption></figure>

### Solução

Utilize o Lisp [AtualizarCodigoLegenda](../autocad/lisp/atualizacodigolegenda.md) para atualizar os códigos do Bloco de Legenda.

***

## Error ED03

Bloco de Legenda está com escala errado.

O Bloco de Legenda apresenta uma discrepância entre a escala exibida e a escala do atributo do bloco, conforme demonstrado na Imagem 03.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img03" alt=""><figcaption><p>Imagem 03</p></figcaption></figure>

### Solução

Ajuste a escala para a escala indicada nos atributos de escala do Bloco.

***

## Error ED04

Bloco de Legenda está com DRAW, CHECKED ou APPROVED errado.

O Bloco de Legenda geralmente fica com :&#x20;

* DRAW: EMB&#x20;
* CHECKED: VOL&#x20;
* APPROVED: Sem nada ou em Branco

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img02" alt=""><figcaption><p>Imagem 04</p></figcaption></figure>

### Solução

Coloque os atributos indicados acima.

***

## Error ED06

LTScale está diferente da metade da Escala do Desenho.

Ocorre quando a configuração de LTScale (escala de tipo de linha) não está de acordo com a escala do desenho.

[O que é LTScale é como ele funciona?](../autocad/ltscale.md)

### Solução

Ajustar o valor do LTScale para ser a metade da escala do desenho, conforme demonstrado na Imagem 05.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img05" alt=""><figcaption><p>Imagem 05</p></figcaption></figure>

***

## Error ED07

Camada **"CONTOUR EXI"** está presente no Desenho.

Na versão R16, existia uma camada chamada **"CONTOUR EXI"** utilizada para indicar peças existentes. A partir da versão R19, essa camada foi substituída pela camada **"ESISTENTE"** (Existente em Italiano).

### Solução 01

Digite o comando **"Eliminar / Purge"**, existe uma aba chamada **"Itens que não podem ser eliminados"**. Dentro dessa aba, há uma árvore de nós onde podemos expandir o nó  de **"Camadas"** para mostrar todas as camadas presentes no desenho. Ao selecionar a camada **"CONTOUR EXI"**, serão exibidos todos os objetos associados a ela. Selecione esses objetos e mude para a camada **"ESISTENTE"**. Conforme demonstrado na Imagem 06.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img06" alt=""><figcaption><p>Imagem 06</p></figcaption></figure>

### Solução 02

Seguindo a [solução anterior](erros-de-desenho.md#solucao-01), caso você tenha algum objeto em **"CONTOUR EXI"** dentro de um bloco, você pode copiar o nome do bloco e ao digitar o comando **"INSERIR"** abrirá uma janela mostrando todos os blocos. Selecione a aba **"Desenho Atual"** e cole o nome do bloco no campo de pesquisa que foi copiado anteriormente. Ao selecionar o bloco, é possível adicioná-lo ao desenho e ajustar o bloco para remover a layer **"CONTOUR EXI"**, conforme mostrado na Imagem 07.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img07" alt=""><figcaption><p>Imagem 07</p></figcaption></figure>

***

## Error ED08

Linha de Chamada não está na camada QUOTE.

A Linha de Chamada diferente das Cotas porque, ao contrário destas, não é automaticamente direcionada para a camada **"QUOTE"**. Em vez disso, ela é alocada na camada selecionada da Paleta de Camadas, que por padrão é a **"Camada 0"**, mas pode também ser a camada **"ASSI"** ou outras. Portanto, é necessário realizar a troca para garantir que a Linha de Chamada esteja na cama **"QUOTE"**.&#x20;

### Solução

Digite o comando **"Eliminar / Purge"**, existe uma aba chamada **"Itens que não podem ser eliminados"**. Dentro dessa aba, há uma árvore de nós onde podemos expandir o nó  de **"Estilos de cota"** para mostrar todas os estilo de cota presentes no desenho. Ao selecionar a camada qualquer estilo, serão exibidos todos os objetos associados a ela. Selecione as Linhas de Chamadas que estão fora da camada **"QUOTE"**.  Conforme demonstrado na Imagem 08.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img08" alt=""><figcaption><p>Imagem 08</p></figcaption></figure>

***

## Error ED09

Deve ter apenas um Bloco de Legenda no mesmo desenho.

Não enviar desenhos como indicado na Imagem 09, a Chloe utiliza os Blocos de Legenda para determinar certas informações para realizar outras verificações.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img09" alt=""><figcaption><p>Imagem 09</p></figcaption></figure>

### Solução

Dividir o desenho em dois arquivos dwg.

***

## Error ED10

Bloco de Revisão 0 está com a Data diferente da Data de Emissão no Bloco de Legenda.

O Bloco de Revisão 0 ou Bloco de Revisão escrito **"FIRST ISSUE / PRIMEIRA EMISSÃO"** deve ter a mesma Data de Emissão que o Bloco de Legenda como indicado na Imagem 10.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img10" alt=""><figcaption><p>Imagem 10</p></figcaption></figure>

### Solução

Colocar a mesma data no Bloco de Revisão 0 e no Bloco de Legenda.

***

## Error ED11

Bloco de Revisão atual está diferente da Data de Revisão no Bloco de Legenda.

O Bloco de Revisão atual deve corresponder à Data de Revisão do Bloco de Legenda. Por exemplo, se o desenho está na revisão 1, o Bloco de Revisão deve exibir a data correspondente a essa revisão, e o Bloco de Legenda deve refletir a mesma Data de Revisão, conforme indicado na Imagem 11.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img11" alt=""><figcaption><p>Imagem 11</p></figcaption></figure>

### Solução

Colocar a mesma data no Bloco de Revisão e no Bloco de Legenda.

***

## Error ED12

Bloco de Revisão atual não preenchido.

O Bloco de Revisão deve estar preenchido com informações de data, descrição, desenhista e verificador. Por exemplo, conforme mostrado na Imagem 12, o Bloco de Revisão 2 está vazio, apesar de o desenho estar na Revisão 02.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img12" alt=""><figcaption><p>Imagem 12</p></figcaption></figure>

### Solução

Preencher o Bloco de Revisão.

***

## Error ED13

Bloco de Legenda não está com data correta.

Ao digitar o comando **"/verificar"**, é possível especificar uma data para verificar o desenho, conforme demonstrado na Imagem 13. Caso nenhuma data seja fornecida, a Chloe utilizará a data de hoje para realizar a verificação.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img13" alt=""><figcaption><p>Imagem 13</p></figcaption></figure>

### Solução

Preencher o Bloco de Legenda com Data correta.

***

## Error ED14

As camadas do desenho não estão configuradas corretamente.

Ao copiar peças extraídas do Inventor para o AutoCAD, se o desenho não possuir certas camadas, o AutoCAD utilizará as configurações provenientes do arquivo extraído do Inventor. É importante notar que as configurações do Inventor diferem, pois ele usa o esquema de cores RGB em vez do esquema de cores indexadas do AutoCAD. Isso faz com que, ao imprimir o desenho em monocromático, o AutoCAD não consiga converter essas cores RGB para tons de preto. Como demonstrado na Imagem 14, um equipamento com camadas não alteradas fica colorido, enquanto as cotas, devidamente ajustadas, aparecem em um tom de preto.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img14.png" alt=""><figcaption><p>Imagem 14</p></figcaption></figure>

### Solução

Seguir o tutorial para [Configurar Layers corretamente](../autocad/configurando-layers.md).

***

## Error ED15

Peso no Bloco de Peça com vírgula.

O Padrão utilizado para separar número decimais é ponto. O AutoCAD usa as vírgulas como separadores de atributos, indicando o início e o fim de um atributo. Podendo ser visto na Imagem 15.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img15.png" alt=""><figcaption><p>Imagem 15</p></figcaption></figure>

### Solução

Digite o comando **"LOCALIZAR / FIND"**. No campo de texto **"Localizar o quê"**, digite **","** (Somente vírgula sem Aspas). No campo de texto **"Substituir por"**, digite **"."** (Somente ponto sem Aspas). Em seguida, clique no botão **"Substituir Tudo"**, conforme demonstrado na Imagem 16. Com isso, todas as vírgulas serão substituídas por pontos.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img16.png" alt=""><figcaption><p>Imagem 16</p></figcaption></figure>

***

## Error ED16

Bloco de Peça com pesos não batendo a multiplicação.

A quantidade multiplicada pelo peso unitário deve resultar no peso total. Por exemplo, na Imagem 17, a quantidade é 71 e o peso unitário é de 10,0 kg. Portanto, o peso total deveria ser 710,0 kg, mas consta apenas 71,0 kg.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img17.png" alt=""><figcaption><p>Imagem 17</p></figcaption></figure>

### Solução

[Como extrair atributos de blocos para verificação?](../autocad/como-extrair-atributos-de-blocos.md)

***

## Error  ED17

Bloco de Peca com vírgula na descrição.

O Padrão utilizado para separar número decimais é ponto. A Redecam usa as vírgulas como separadores de atributos, indicando o início e o fim de um atributo. Podendo ser visto na Imagem 18.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img18.jpg" alt=""><figcaption><p>Imagem 18</p></figcaption></figure>

### Solução

Digite o comando **"LOCALIZAR / FIND"**. No campo de texto **"Localizar o quê"**, digite **","** (Somente vírgula sem Aspas). No campo de texto **"Substituir por"**, digite **"."** (Somente vírgula sem Aspas). Em seguida, clique no botão **"Substituir Tudo"**, conforme demonstrado na Imagem 19. Com isso, todas as vírgulas serão substituídas por pontos.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img19.jpg" alt=""><figcaption><p>Imagem 19</p></figcaption></figure>

***

## Error ED18

Nota com Código de Identificação das peças diferente do Código do Desenho.

Nota com Código de Identificação das peças deve ter o mesmo Código do Desenho seguindo a divisão do AA-SS-DD, como mostrado na Imagem 20.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img20.jpg" alt=""><figcaption><p>Imagem 20.</p></figcaption></figure>

### Solução

Utilizar o código Lisp [AtualizaCodigoLegenda](../autocad/lisp/atualizacodigolegenda.md) para arrumar Codigo de Identificação

***

## Error ED19

Fator de Largura do atributo Marca no Bloco de Peça diferente de 0,7.

Utilizar um fator de largura de 0.7 no atributo de Marca no Bloco de Peça, de modo que ao copiar o bloco para um desenho de conjunto, o atributo receba o código de desenho ajustem adequadamente ao espaço.

### Solução

Utilizar o comando **"GERATRIB / BATTMAN"**  para poder atualizar o atributo do Bloco, como mostrado na Imagem 21.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img21.jpg" alt=""><figcaption><p>Imagem 21.</p></figcaption></figure>

***

## Error ED20

Nota com Peso Aproximado está diferente da Soma dos Blocos de Peça.

A soma dos blocos de peças deve coincidir com o peso total aproximado na nota. Se houver **"APENAS AÇO / ONLY STEELWORK"**, esse valor deve excluir o peso da "**LÃ DE ROCHA / ROCK WOOL"** e considerar esse peso na nota **"INCLUINDO LÃ DE ROCHA | INCLUDING ROCK WOOL"**, como demostrado na Imagem 22.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img22.jpg" alt=""><figcaption><p>Imagem 22.</p></figcaption></figure>

### Solução

[Como extrair atributos dos blocos para verificar a soma?](../autocad/como-extrair-atributos-de-blocos.md)

***

## Error ED21

Cota com linha fora do Por Camada.

Ao criar cotas escalonadas, é uma prática comum modificar as cores das linhas para diferentes como Azul, Ciano, Roxo invés de PorCamada, proporcionando uma diferenciação visual entre os estilos de cota utilizados. No entanto, é importante que ao entregar o desenho, as cores das linhas devem ser revertidas ao padrão de PorCamada.

### Solução

Abrir o "**Modificador de Cota"** e na aba "**Linhas"** colocar em "**Cor"** para "**PorCamada",** como demostrado na Imagem 23.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img23.png" alt=""><figcaption><p>Imagem 23</p></figcaption></figure>

***

## Error ED22

Cota com escala global incorreta.

Todas as cota do desenho devem ficar na mesma Escala do Formato.

### Solução

Abrir o "**Modificador de Cota"** e na aba "**Ajustar"** colocar em "**Usar escala global de:"**  para a Escala do Formato, como desmotrado na Imagem 24

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img24.png" alt=""><figcaption><p>Imagem 24</p></figcaption></figure>

***

## ErrorED 23

Fator de Escala ou Nome da cota incorreta.

Fator de Escala é determinado pela Equação: Escala da Cota / Escala do Formato.

Exemplo: \
Escala do Formato - 1:20.\
Escala da Cota - 1:5.

Escala da Cota / Escala do Formato.\
5 / 20 = 0,4.

### Solução 01

Abrir o "**Modificador de Cota"** e na aba "**Unidades Primárias"** colocar em "**Fator de Escala:"** para Escala da Cota / Escala do Formato, como demostrado na Imagem 25.

### Solução 02

Caso o Fator de Escala estiver correto, verificar se o nome da cota está correto.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img25.png" alt=""><figcaption><p>Imagem 25</p></figcaption></figure>

***

## Error ED0B

Lista com Blocos que estão no desenho só que numa versão antiga.

Este erro apresenta uma lista de blocos que estão presentes no desenho, porém, em uma versão antiga podendo ser R16 ou R18. O erro será exibido com o nome do bloco e uma descrição referente ao Bloco, como mostrado na Imagem 26.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img26" alt=""><figcaption><p>Imagem 26</p></figcaption></figure>

### Solução

Na comando **"Eliminar / Purge"**, existe uma aba chamada **"Itens que não podem ser eliminados"**.  Dentro dessa aba, há uma árvore de nós onde podemos expandir nó de **"Blocos"** para mostrar todas as blocos presentes no desenho, facilitando a substituição dos mesmos. Conforme demonstrado na Imagem 27.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img27" alt=""><figcaption><p>Imagem 27</p></figcaption></figure>

***

## Error EDSB

Lista de Blocos na escala errada\
(**EM DESENVOLVIMENTO**)
