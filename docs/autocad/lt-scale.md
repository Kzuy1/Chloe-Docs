---
sidebar_position: 3
---

# LTScale

## O que é LTScale?
O LTSCALE é utilizado para controlar a escala dos tipos de linha (linetype scale) em um desenho. Isso afeta a aparência dos tipos de linha aplicados aos objetos, como linhas tracejadas, pontilhadas e outros estilos personalizados. A configuração do LTSCALE ajusta a repetição e o espaçamento dos padrões de linha em relação ao tamanho e escala do desenho.

## Exemplo do LTScale
Na Imagem 01, podemos observar diferentes configurações de LTSCALE:

- Esquerda: Podemos ver uma linha menos espaçada, com os valores de LTSCALE = 0.25 e LTSCALE = 0.5, onde os traços e espaços são curtos e densos;
- Meio: O valor LTSCALE = 1.0 representa a transição, onde o espaçamento e os traços são equilibrados;
- Direita: Podemos ver linhas mais espaçadas, com os valores de LTSCALE = 1.5 e LTSCALE = 5.0, onde os traços e espaços são mais longos e espaçados.

Essa transição de espaçamento ilustra como diferentes valores de LTSCALE afetam a aparência dos tipos de linha no desenho, permitindo ajustar a visibilidade e o detalhe conforme necessário.

<figure>
    <img src="/img/autocad/ltscale/img01.webp" alt="Imagem 01" />
    <figcaption>Imagem 01</figcaption>
</figure>

## Convenção de Desenho
O valor do LTScale deve ser a metade da escala do desenho, conforme demonstrado na Imagem 02. Por exemplo, se o desenho tiver escala 1:50, divide-se 50 por 2, resultando em 25 para LTScale. Da mesma forma, se a escala for 1:20, divide-se 20 por 2, obtendo-se 10 para LTScale.

<figure>
    <img src="/img/autocad/ltscale/img02.webp" alt="Imagem 02" />
    <figcaption>Imagem 02</figcaption>
</figure>