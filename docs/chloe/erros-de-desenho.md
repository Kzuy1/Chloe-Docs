---
sidebar_position: 3
---

# 🚨 Erros de Desenho
<h3>Todos os Erros que a Chloe pode encontrar.</h3>

## Error ED01
O nome arquivo não está separado corretamente.

Os códigos de desenho são separados  por traços (-) e sublinhados (_), conforme demonstrado na Imagem 01.

<figure>
    <img src="/img/chloe/erros-de-desenho/img01.webp" alt="Imagem 01" />
    <figcaption>Imagem 01</figcaption>
</figure>

### Solução
Renomeie o arquivo seguindo a segmentação correta.

---

## Error ED02
Bloco de Legenda está com código errado.

Na Imagem 02, o Bloco de Legenda apresenta um código diferente do que está no Nome do Arquivo. Os códigos mostrados são 1FN2_FN-08-01, mas o correto é 1FN3_FN-A7-01.

<figure>
    <img src="/img/chloe/erros-de-desenho/img02.webp" alt="Imagem 02" />
    <figcaption>Imagem 02</figcaption>
</figure>

### Solução
Utilize o Lisp <a href="/docs/autocad/lisp/atualiza-codigo-legenda">AtualizarCodigoLegenda</a> para atualizar os códigos do Bloco de Legenda.

---

## Error ED03
Bloco de Legenda está com escala errado.

O Bloco de Legenda apresenta uma discrepância entre a escala exibida e a escala do atributo do bloco, conforme demonstrado na Imagem 03.

<figure>
    <img src="/img/chloe/erros-de-desenho/img03.webp" alt="Imagem 03" />
    <figcaption>Imagem 03</figcaption>
</figure>

### Solução
Ajuste a escala para a escala indicada nos atributos de escala do Bloco.

---

## Error ED04
Bloco de Legenda está com DRAW, CHECKED ou APPROVED errado.

O Bloco de Legenda geralmente fica com : 

> **DRAW:** EMB  
> **CHECKED:** VOL  
> **APPROVED:** Sem nada ou em Branco

<figure>
    <img src="/img/chloe/erros-de-desenho/img04.webp" alt="Imagem 04" />
    <figcaption>Imagem 04</figcaption>
</figure>

### Solução
Coloque os atributos indicados acima.

---

## Error ED06
LTScale está diferente da metade da Escala do Desenho.

Ocorre quando a configuração de LTScale (escala de tipo de linha) não está de acordo com a escala do desenho.

<a href="/docs/autocad/lt-scale">O que é LTScale é como ele funciona?</a>

### Solução
Ajustar o valor do LTScale para ser a metade da escala do desenho, conforme demonstrado na Imagem 05.

<figure>
    <img src="/img/chloe/erros-de-desenho/img05.webp" alt="Imagem 05" />
    <figcaption>Imagem 05</figcaption>
</figure>

---

## Error ED07
Camada **"CONTOUR EXI"** está presente no Desenho.

Na versão R16, existia uma camada chamada **"CONTOUR EXI"** utilizada para indicar peças existentes. A partir da versão R19, essa camada foi substituída pela camada **"ESISTENTE"** (Existente em Italiano).

### Solução 01
Digite o comando **"Eliminar / Purge"**, existe uma aba chamada **"Itens que não podem ser eliminados"**. Dentro dessa aba, há uma árvore de nós onde podemos expandir o nó  de **"Camadas"** para mostrar todas as camadas presentes no desenho. Ao selecionar a camada **"CONTOUR EXI"**, serão exibidos todos os objetos associados a ela. Selecione esses objetos e mude para a camada **"ESISTENTE"**. Conforme demonstrado na Imagem 06.

<figure>
    <img src="/img/chloe/erros-de-desenho/img06.webp" alt="Imagem 06" />
    <figcaption>Imagem 06</figcaption>
</figure>

### Solução 02
Seguindo a <a href="#solução-01">solução anterior</a>, caso você tenha algum objeto em **"CONTOUR EXI"** dentro de um bloco, você pode copiar o nome do bloco e ao digitar o comando **"INSERIR"** abrirá uma janela mostrando todos os blocos. Selecione a aba **"Desenho Atual"** e cole o nome do bloco no campo de pesquisa que foi copiado anteriormente. Ao selecionar o bloco, é possível adicioná-lo ao desenho e ajustar o bloco para remover a layer **"CONTOUR EXI"**, conforme mostrado na Imagem 07.

<figure>
    <img src="/img/chloe/erros-de-desenho/img07.webp" alt="Imagem 07" />
    <figcaption>Imagem 07</figcaption>
</figure>

---

## Error ED08
Linha de Chamada não está na camada QUOTE.

A Linha de Chamada diferente das Cotas porque, ao contrário destas, não é automaticamente direcionada para a camada **"QUOTE"**. Em vez disso, ela é alocada na camada selecionada da Paleta de Camadas, que por padrão é a **"Camada 0"**, mas pode também ser a camada **"ASSI"** ou outras. Portanto, é necessário realizar a troca para garantir que a Linha de Chamada esteja na cama **"QUOTE"**. 

### Solução
Digite o comando **"Eliminar / Purge"**, existe uma aba chamada **"Itens que não podem ser eliminados"**. Dentro dessa aba, há uma árvore de nós onde podemos expandir o nó  de **"Estilos de cota"** para mostrar todas os estilo de cota presentes no desenho. Ao selecionar a camada qualquer estilo, serão exibidos todos os objetos associados a ela. Selecione as Linhas de Chamadas que estão fora da camada **"QUOTE"**.  Conforme demonstrado na Imagem 08.

<figure>
    <img src="/img/chloe/erros-de-desenho/img08.webp" alt="Imagem 08" />
    <figcaption>Imagem 08</figcaption>
</figure>

---

## Error ED09
Deve ter apenas um Bloco de Legenda no mesmo desenho.

Não enviar desenhos como indicado na Imagem 09, a Chloe utiliza os Blocos de Legenda para determinar certas informações para realizar outras verificações.

<figure>
    <img src="/img/chloe/erros-de-desenho/img09.webp" alt="Imagem 09" />
    <figcaption>Imagem 09</figcaption>
</figure>

### Solução
Dividir o desenho em dois arquivos dwg.

---

## Error ED10
Bloco de Revisão 0 está com a Data diferente da Data de Emissão no Bloco de Legenda.

O Bloco de Revisão 0 ou Bloco de Revisão escrito **"FIRST ISSUE / PRIMEIRA EMISSÃO"** deve ter a mesma Data de Emissão que o Bloco de Legenda como indicado na Imagem 10.

<figure>
    <img src="/img/chloe/erros-de-desenho/img10.webp" alt="Imagem 10" />
    <figcaption>Imagem 10</figcaption>
</figure>

### Solução
Colocar a mesma data no Bloco de Revisão 0 e no Bloco de Legenda.

---

## Error ED11
Bloco de Revisão atual está diferente da Data de Revisão no Bloco de Legenda.

O Bloco de Revisão atual deve corresponder à Data de Revisão do Bloco de Legenda. Por exemplo, se o desenho está na revisão 1, o Bloco de Revisão deve exibir a data correspondente a essa revisão, e o Bloco de Legenda deve refletir a mesma Data de Revisão, conforme indicado na Imagem 11.

<figure>
    <img src="/img/chloe/erros-de-desenho/img11.webp" alt="Imagem 11" />
    <figcaption>Imagem 11</figcaption>
</figure>

### Solução
Colocar a mesma data no Bloco de Revisão e no Bloco de Legenda.

---

## Error ED12
Bloco de Revisão atual não preenchido.

O Bloco de Revisão deve estar preenchido com informações de data, descrição, desenhista e verificador. Por exemplo, conforme mostrado na Imagem 12, o Bloco de Revisão 2 está vazio, apesar de o desenho estar na Revisão 02.

<figure>
    <img src="/img/chloe/erros-de-desenho/img12.webp" alt="Imagem 12" />
    <figcaption>Imagem 12</figcaption>
</figure>

### Solução
Preencher o Bloco de Revisão.

---

## Error ED13
Bloco de Legenda não está com data correta.

Ao digitar o comando **"/verificar"**, é possível especificar uma data para verificar o desenho, conforme demonstrado na Imagem 13. Caso nenhuma data seja fornecida, a Chloe utilizará a data de hoje para realizar a verificação.

<figure>
    <img src="/img/chloe/erros-de-desenho/img13.webp" alt="Imagem 13" />
    <figcaption>Imagem 13</figcaption>
</figure>

### Solução
Preencher o Bloco de Legenda com Data correta.

---

## Error ED14
As camadas do desenho não estão configuradas corretamente.

Ao copiar peças extraídas do Inventor para o AutoCAD, se o desenho não possuir certas camadas, o AutoCAD utilizará as configurações provenientes do arquivo extraído do Inventor. É importante notar que as configurações do Inventor diferem, pois ele usa o esquema de cores RGB em vez do esquema de cores indexadas do AutoCAD. Isso faz com que, ao imprimir o desenho em monocromático, o AutoCAD não consiga converter essas cores RGB para tons de preto. Como demonstrado na Imagem 14, um equipamento com camadas não alteradas fica colorido, enquanto as cotas, devidamente ajustadas, aparecem em um tom de preto.

<figure>
    <img src="/img/chloe/erros-de-desenho/img14.webp" alt="Imagem 14" />
    <figcaption>Imagem 14</figcaption>
</figure>

### Solução
<a href="/docs/autocad/tutoriais/como-configurar-camada">Seguir o tutorial para Como Configurar Camada.</a>

---

## Error ED15
Peso no Bloco de Peça com vírgula.

O Padrão utilizado para separar número decimais é ponto. O AutoCAD usa as vírgulas como separadores de atributos, indicando o início e o fim de um atributo. Podendo ser visto na Imagem 15.

<figure>
    <img src="/img/chloe/erros-de-desenho/img15.webp" alt="Imagem 15" />
    <figcaption>Imagem 15</figcaption>
</figure>

### Solução
Digite o comando **"LOCALIZAR / FIND"**. No campo de texto **"Localizar o quê"**, digite **","** (Somente vírgula sem Aspas). No campo de texto **"Substituir por"**, digite **"."** (Somente ponto sem Aspas). Em seguida, clique no botão **"Substituir Tudo"**, conforme demonstrado na Imagem 16. Com isso, todas as vírgulas serão substituídas por pontos.

<figure>
    <img src="/img/chloe/erros-de-desenho/img16.webp" alt="Imagem 16" />
    <figcaption>Imagem 16</figcaption>
</figure>

---

## Error ED16
Bloco de Peça com pesos não batendo a multiplicação.

A quantidade multiplicada pelo peso unitário deve resultar no peso total. Por exemplo, na Imagem 17, a quantidade é 71 e o peso unitário é de 10,0 kg. Portanto, o peso total deveria ser 710,0 kg, mas consta apenas 71,0 kg.

<figure>
    <img src="/img/chloe/erros-de-desenho/img17.webp" alt="Imagem 17" />
    <figcaption>Imagem 17</figcaption>
</figure>

### Solução
<a href="/docs/autocad/tutoriais/como-extrair-atributos-de-blocos">Como extrair atributos de blocos para verificação?</a>

---

## Error ED17
Bloco de Peca com vírgula na descrição.

O Padrão utilizado para separar número decimais é ponto. A Redecam usa as vírgulas como separadores de atributos, indicando o início e o fim de um atributo. Podendo ser visto na Imagem 18.

<figure>
    <img src="/img/chloe/erros-de-desenho/img18.jpg" alt="Imagem 18" />
    <figcaption>Imagem 18</figcaption>
</figure>

### Solução
Digite o comando **"LOCALIZAR / FIND"**. No campo de texto **"Localizar o quê"**, digite **","** (Somente vírgula sem Aspas). No campo de texto **"Substituir por"**, digite **"."** (Somente vírgula sem Aspas). Em seguida, clique no botão **"Substituir Tudo"**, conforme demonstrado na Imagem 19. Com isso, todas as vírgulas serão substituídas por pontos.

<figure>
    <img src="/img/chloe/erros-de-desenho/img19.jpg" alt="Imagem 19" />
    <figcaption>Imagem 19</figcaption>
</figure>

---

## Error ED18
Nota com Código de Identificação das peças diferente do Código do Desenho.

Nota com Código de Identificação das peças deve ter o mesmo Código do Desenho seguindo a divisão do AA-SS-DD, como mostrado na Imagem 20.

<figure>
    <img src="/img/chloe/erros-de-desenho/img20.jpg" alt="Imagem 20" />
    <figcaption>Imagem 20</figcaption>
</figure>

### Solução
Utilizar o código Lisp <a href="/docs/autocad/lisp/atualiza-codigo-legenda">AtualizaCodigoLegenda para arrumar Codigo de Identificação</a>

## Error ED19
Fator de Largura do atributo Marca no Bloco de Peça diferente de 0,7.

Utilizar um fator de largura de 0.7 no atributo de Marca no Bloco de Peça, de modo que ao copiar o bloco para um desenho de conjunto, o atributo receba o código de desenho ajustem adequadamente ao espaço.

### Solução
Utilizar o comando **"GERATRIB / BATTMAN"**  para poder atualizar o atributo do Bloco, como mostrado na Imagem 21.

<figure>
    <img src="/img/chloe/erros-de-desenho/img21.jpg" alt="Imagem 21" />
    <figcaption>Imagem 21</figcaption>
</figure>

---

## Error ED20
Nota com Peso Aproximado está diferente da Soma dos Blocos de Peça.

A soma dos blocos de peças deve coincidir com o peso total aproximado na nota. Se houver **"APENAS AÇO / ONLY STEELWORK"**, esse valor deve excluir o peso da **"LÃ DE ROCHA / ROCK WOOL"** e considerar esse peso na nota **"INCLUINDO LÃ DE ROCHA | INCLUDING ROCK WOOL"**, como demostrado na Imagem 22.

<figure>
    <img src="/img/chloe/erros-de-desenho/img22.jpg" alt="Imagem 22" />
    <figcaption>Imagem 22</figcaption>
</figure>

## Solução
<a href="/docs/autocad/tutoriais/como-extrair-atributos-de-blocos">Como extrair atributos dos blocos para verificar a soma?</a>

---

## Error ED21
Cota com linha fora do Por Camada.

Ao criar cotas escalonadas, é uma prática comum modificar as cores das linhas para diferentes como Azul, Ciano, Roxo invés de PorCamada, proporcionando uma diferenciação visual entre os estilos de cota utilizados. No entanto, é importante que ao entregar o desenho, as cores das linhas devem ser revertidas ao padrão de PorCamada.

### Solução
Abrir o **"Modificador de Cota"** e na aba **"Linhas"** colocar em **"Cor"** para **"PorCamada"**, como demostrado na Imagem 23.

<figure>
    <img src="/img/chloe/erros-de-desenho/img23.webp" alt="Imagem 23" />
    <figcaption>Imagem 23</figcaption>
</figure>

---

## Error ED22
Cota com escala global incorreta.

Todas as cota do desenho devem ficar na mesma Escala do Formato.

### Solução
Abrir o **"Modificador de Cota"** e na aba **"Ajustar"** colocar em **"Usar escala global de:"**  para a Escala do Formato, como desmotrado na Imagem 24

<figure>
    <img src="/img/chloe/erros-de-desenho/img24.webp" alt="Imagem 24" />
    <figcaption>Imagem 24</figcaption>
</figure>

---

## Error ED23

Fator de Escala ou Nome da cota incorreta.

Fator de Escala é determinado pela Equação: Escala da Cota / Escala do Formato.

Exemplo:  
Escala do Formato - 1:20.  
Escala da Cota - 1:5.  

Escala da Cota / Escala do Formato.  
5 / 20 = 0,4.

### Solução 01
Abrir o **"Modificador de Cota"** e na aba **"Unidades Primárias"** colocar em **"Fator de Escala:"** para Escala da Cota / Escala do Formato, como demostrado na Imagem 25.

### Solução 02
Caso o Fator de Escala estiver correto, verificar se o nome da cota está correto.

<figure>
    <img src="/img/chloe/erros-de-desenho/img25.webp" alt="Imagem 25" />
    <figcaption>Imagem 25</figcaption>
</figure>

---

## Error ED0B
Lista com Blocos que estão no desenho só que numa versão antiga.

Este erro apresenta uma lista de blocos que estão presentes no desenho, porém, em uma versão antiga podendo ser R16 ou R18. O erro será exibido com o nome do bloco e uma descrição referente ao Bloco, como mostrado na Imagem 26.

<figure>
    <img src="/img/chloe/erros-de-desenho/img26.webp" alt="Imagem 26" />
    <figcaption>Imagem 26</figcaption>
</figure>

### Solução
Na comando **"Eliminar / Purge"**, existe uma aba chamada **"Itens que não podem ser eliminados"**.  Dentro dessa aba, há uma árvore de nós onde podemos expandir nó de **"Blocos"** para mostrar todas as blocos presentes no desenho, facilitando a substituição dos mesmos. Conforme demonstrado na Imagem 27.

<figure>
    <img src="/img/chloe/erros-de-desenho/img27.webp" alt="Imagem 27" />
    <figcaption>Imagem 27</figcaption>
</figure>

---

## Error EDSB
Lista de Blocos na escala errada.  
**(EM DESENVOLVIMENTO)**