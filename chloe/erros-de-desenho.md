---
description: Todos os Erros que a Chloe pode encontrar!
---

# 🚨 Erros de Desenho

***

## Error ED01

O nome arquivo não está separado corretamente.

Os códigos de desenho são separados  por traços (-) e sublinhados (\_), conforme demonstrado na Imagem 01.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img01" alt=""><figcaption><p>Imagem 01</p></figcaption></figure>

### Solução

Renomeie o arquivo seguindo a segmentação correta.

***

## Error ED02

Bloco de Legenda está com código errado.

Na Imagem 02, o Bloco de Legenda apresenta um código diferente do que está no Nome do Arquivo. Os códigos mostrados são 1FN2\_FN-A8-01, mas o correto é 1FN3\_FN-A8-01.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img04" alt=""><figcaption><p>Imagem 02</p></figcaption></figure>

### Solução

Utilize o Lisp `AtualizarCodigoLegenda` para atualizar os códigos do Bloco de Legenda.

***

## Error ED03

Bloco de Legenda está com escala errado.

O Bloco de Legenda apresenta uma discrepância entre a escala exibida e a escala do atributo do bloco, conforme demonstrado na Imagem 03.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img03" alt=""><figcaption><p>Imagem 03</p></figcaption></figure>

### Solução

Ajuste a escala para a escala indicada nos atributos de escala do Bloco.

***

## Error 04

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

\[O que é LTScale é como ele funciona?]\()

### Solução

Ajustar o valor do LTScale para ser a metade da escala do desenho, conforme demonstrado na Imagem 05.

<figure><img src="../.gitbook/assets/img_chloe_erros-de-desenho_img05" alt=""><figcaption><p>Imagem 05</p></figcaption></figure>

***

## Error ED07

Layer CONTOUR EXI está presente no Desenho.

Na versão R16, existia uma camada chamada `CONTOUR EXI` utilizada para indicar peças existentes. A partir da versão R19, essa camada foi substituída pela camada `ESISTENTE` (Existente em Italiano).

### Solução 01

Digite o comando `Eliminar/Purge`, existe uma aba chamada `Itens que não podem ser eliminados`. Dentro dessa aba, há uma árvore de nós onde podemos expandir `Camadas` para mostrar todas as camadas/layers presentes no desenho. Ao selecionar a camada `CONTOUR EXI`, serão exibidos todos os objetos associados a ela. Selecione esses objetos e mude para a camada `ESISTENTE`. Conforme demonstrado na Imagem 06.

***
