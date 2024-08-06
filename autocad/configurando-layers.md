# Configurando Layers

## Informações:

* Este tutorial é aplicável tanto ao AutoCAD quanto ao AutoCAD LT;
* Cada etapa incluirá uma imagem explicativa.

## Passo 01

Vá na aba `Padrão / Home` no canto superior esquerdo. E na parte superior centro irá encontrar a opção `Propriedades da Camada / Layer Properties`.

<figure><img src="../.gitbook/assets/img_autocad-configurandolayer_img01.png" alt=""><figcaption><p>Imagem 01</p></figcaption></figure>

## Passo 02

Ao abrir a aba `Propriedades de Camada / Layer Properties`, localize o `Gerenciador de Estados da Camada / Layer States Manager` no canto superior direito da aba. Poderá acessá-lo clicando ou apertando `ALT + S`.

<figure><img src="../.gitbook/assets/img_autocad-configurandolayer_img02.png" alt=""><figcaption><p>Imagem 02</p></figcaption></figure>

## Passo 03

Uma nova aba intitulada `Gerenciador de Estados da Camada / Layer States Manager` será aberta, exibindo todos os estados das camadas do desenho. Caso exista um estado previamente criado, você pode selecioná-lo e excluí-lo clicando no botão `Excluir / Delete` localizado no canto direito da aba.

<figure><img src="../.gitbook/assets/img_autocad-configurandolayer_img03.png" alt=""><figcaption><p>Imagem 03</p></figcaption></figure>

## Passo 04

Clique no botão `Importar / Import`, que está localizado na direita. Isso abrirá uma nova aba chamada `Importar estado de modelo / Import layer state`, onde você deverá inserir o link fornecido abaixo no campo `Nome do arquivo / File Name`, e ir no botão `Abrir / Open`.

{% code overflow="wrap" %}
```
L:\Drives compartilhados\EMB_ENGENHARIA_BIBLIOTECA\PADRÕES PROGRAMAS\AUTOCAD\PADRÕES LAYERS
```
{% endcode %}

<figure><img src="../.gitbook/assets/img_autocad-configurandolayer_img04.png" alt=""><figcaption><p>Imagem 04</p></figcaption></figure>

## Passo 05

Ainda na aba `Importar estado de modelo / Import layer state`, no campo `Arquivos do tipo / Files of type`, selecione a opção de `(*.las)`.

<figure><img src="../.gitbook/assets/img_autocad-configurandolayer_img05.png" alt=""><figcaption><p>Imagem 05</p></figcaption></figure>

## Passo 06

Selecione o arquivo `PADRÃO-REDECAM`, e clique no botão `Abrir / Open`

<figure><img src="../.gitbook/assets/img_autocad-configurandolayer_img06.png" alt=""><figcaption><p>Imagem 06</p></figcaption></figure>

## Passo 07

Nesse passo, duas situações podem ocorrer. Se aparecer a mensagem `Não foi possível restaurar todos os tipos de linha / Restore could not restore all line types`, como mostrado na Imagem 07, será necessário ir para a seção de [Erro 01](configurando-layers.md#erro-01). Caso seja exibido o aviso `Estado da camada - Importação com êxito / Layer State - Successful import`, clique no botão `Fechar a caixa de diálogo / Close dialog`, como demonstrado na Imagem 08.

<figure><img src="../.gitbook/assets/img_autocad-configurandolayer_img07.png" alt=""><figcaption><p>Imagem 07</p></figcaption></figure>

<figure><img src="../.gitbook/assets/img_autocad-configurandolayer_img08.png" alt=""><figcaption><p>Imagem 08</p></figcaption></figure>

## Passo 08

Voltando a aba intitulada `Gerenciador de Estados da Camada / Layer States Manager`, selecione o estado de camada `PADRÃO-REDECAM`, e na parte de baixo em `Opções de restauração / Resore option` deixe desmarcado a opção `Desativar camadas não encontradas no estado da camada / Turn off layers not found in layer state`, e clique no botão `Restaurar / Restore` na parte inferior direita.

<figure><img src="../.gitbook/assets/img_autocad-configurandolayer_img09.png" alt=""><figcaption><p>Imagem 09</p></figcaption></figure>

## Passo 09

Ao fechar a aba do `Gerenciador de Estados da Camada / Layer States Manager`, podera ver as `Propriedades de Camada / Layer Properties`, com suas devidas configurações, como a Imagem 10.

<figure><img src="../.gitbook/assets/img_autocad-configurandolayer_img10.png" alt=""><figcaption><p>Imagem 10</p></figcaption></figure>

## Erro 01

Abra o **`REDECAM AutoCAD Template`**, disponível no link abaixo, e copie o `Bloco de Camada` (Na Imagem 11, você pode ver a localização do bloco). Mova-o para dentro do desenho e, em seguida, reinicie o processo desde o início.

```
L:\Drives compartilhados\EMB_ENGENHARIA_BIBLIOTECA\PADRÕES CLIENTES\REDECAM\REDECAM AutoCAD Template R19.dwg
```

<figure><img src="../.gitbook/assets/img_autocad-configurandolayer_img11.png" alt=""><figcaption><p>Imagem 11</p></figcaption></figure>
