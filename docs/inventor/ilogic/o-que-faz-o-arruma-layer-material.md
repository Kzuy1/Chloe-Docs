---
sidebar_position: 2
---

# O que o faz o ArrumaLayerMaterial?

## Informações:

Passará por cada componente, atribuindo-os a uma camada específica correspondente ao seu respectivo material.

Exemplo:

O Plenum possui dois tipos de materiais distintos: AISI 304L e S32205. Os componentes feitos de AISI 304L serão movidos para a camada **``AISI 304L``**, enquanto aqueles feitos de S32205 serão alocados na camada **``S32205``**.

As linhas ocultas permanecerão na camada **``NASCOSTE``**, e os materiais que não tiverem uma camada definida permanecerão na camada **``CONTORNI``**.

<figure>
    <img src="/img/inventor/ilogic/o-que-faz-o-arruma-layer-material/img01.webp" alt="Imagem 01" />
    <figcaption>Imagem 01</figcaption>
</figure>

## Passo 01
Ir na aba **``Administrar``**, **``Editor de Estilos``**, opção **``Camadas``** e adicionar a camada do material desejado. Observe na Imagem 02.

**IMPORTANTE DIGITAR O NOME IGUAL**

<figure>
    <img src="/img/inventor/ilogic/o-que-faz-o-arruma-layer-material/img02.webp" alt="Imagem 02" />
    <figcaption>Imagem 02</figcaption>
</figure>

## Passo 02
Execute o código e ao final ele mostrará os materiais que não foram mexidos, ou uma mensagem de erro, conforme mostra a Imagem 03.

<figure>
    <img src="/img/inventor/ilogic/o-que-faz-o-arruma-layer-material/img03.webp" alt="Imagem 03" />
    <figcaption>Imagem 03</figcaption>
</figure>