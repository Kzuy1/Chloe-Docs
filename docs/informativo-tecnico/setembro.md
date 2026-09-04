---
sidebar_position: 9
---

# Setembro/2026

## 1 - Solda da Câmara Central - Tampa Superior
<!-- INFO-META
Quem: Fabio Puccio
Oque: Email com assunto "C126002 - Mason City: plenum central duct top panel weldings"
Onde: Email
Data: 02/09/2026
-->
> 📅 02/09/26  • <span class="status-valid">VÁLIDO</span>

<div class="bt-card">
- Categoria: Detalhamento
- Equipamento: Câmara Central - Tampa Superior
</div>

Para projeto Redecam, a Câmara Central (Central Duct), a Tampa Superior deve receber `SOLDA FILETE` na parte externa e `SOLDA FILETE DESCONTÍNUA` na parte interna da Câmara Central.

<figure>
    <img src="/img/informativo-tecnico/setembro-2026/img01.webp" alt="Imagem 01" />
    <figcaption>Imagem 01</figcaption>
</figure>

## 2 - Explicação sobre escala de Seção e Detalhe

<!-- INFO-META
Sem Informação clara: Curso que o Lucas teve com Wendel e o Henrique
-->

> 📅 02/09/26  • <span class="status-valid">VÁLIDO</span>

<div class="bt-card">
- Categoria: Detalhamento
</div>

Para projetos **Redecam e Satus**, a definição da escala de **Seção** e **Detalhe** deve seguir uma lógica baseada na relação entre a **escada do formato** e a **escala desejada**.

### 2.1 - Entendendo a lógica da escala

A escala aplicada a uma Seção ou Detalhe deve ser determinada a partir da relação entre a escala do formato e a escala de representação desejada para a vista derivada.

No contexto do detalhamento, a escala do formato estabelece a referência de representação da vista principal. Quando uma Seção ou Detalhe necessita ser representada em uma escala diferente, deve ser aplicado um Fator de Escala que realize a conversão entre essas duas condições de escala.

Para isso, utilizamos dois conceitos:

- Escala do Formato: escala de referência utilizada no formato do desenho;
- Escala Desejada: escala na qual a Seção ou Detalhe deverá ser representada;
- Fator de Escala: Valor que deve ser informado no comando de escala para ajustar a representação da Seção ou Detalhe.

A regra é:

> **FATOR DE ESCALA = ESCALA DO FORMATO ÷ ESCALA DESEJADA**

Consequentemente:

> **ESCALA DESEJADA = ESCALA DO FORMATO ÷ FATOR DE ESCALA**

Essas duas fórmulas são a mesma relação vista de maneiras diferentes.

### 2.2 - Exemplo prático

Considere um desenho cuja **escala do formato é 1:10** e queremos representar um Detalhe na escala **1:5**.

**Escala do formato = 10**

**Escala desejada = 5**

Aplicando a fórmula:

> **FATOR DE ESCALA = 10 ÷ 5 = 2**

Portanto, o **Fator de Escala será 2**.

Esse valor representa o fator de ampliação aplicado ao Detalhe em relação à escala utilizada no formato.

É possível visualizar esse resultado no **Detalhe "A" da Imagem 02**.

---

Seguindo para o próximo exemplo, considere um desenho cuja **escala do formato é 1:10** e queremos representar um Detalhe na escala **1:2**.

**Escala do formato = 10**

**Escala desejada = 2**

Aplicando a fórmula:

> **FATOR DE ESCALA = 10 ÷ 2 = 5**

Portanto, o **Fator de Escala será 5**.

É possível visualizar esse resultado no **Detalhe "C" da Imagem 02**.

<figure>
    <img src="/img/informativo-tecnico/setembro-2026/img02.webp" alt="Imagem 02" />
    <figcaption>Imagem 02</figcaption>
</figure>

### 2.3 - Regra para utilização

Para garantir a correta representação e a compatibilidade entre o desenho e o modelo 3D, devem ser observadas as seguintes regras:

- A vista principal não deve ter sua escala alterada. A representação deve permanecer na escala definida pelo formato, garantindo que suas dimensões correspondam às dimensões do modelo.
- Não devem ser utilizadas escalas diferentes das previstas nos templates padronizados. Escalas como 1:4, 1:7.5, entre outras não contempladas pelo padrão, não devem ser utilizadas.

### 2.4 - Tabela de referência

| Escala do Formato | Escala Desejada | Fator de Escala |
|:-----------------:|:---------------:|:---------------:|
|       1:10        |       1:2       |        5        |
|       1:10        |      1:2.5      |        4        |
|       1:10        |       1:5       |        2        |
|       1:15        |      1:2.5      |        6        |
|       1:15        |       1:10      |       1,5       |
|       1:75        |       1:25      |        3        |
|       1:75        |       1:50      |       1,5       |
|      1:100        |       1:25      |        4        |
|      1:100        |       1:75      |      1,333      |

### 2.5 - Passo a Passo

1. Identificar a **escala do formato**;
2. Definir a **escala desejada** para a Seção ou Detalhe;
3. Calcular o **fator de escala**;
4. Aplicar o valor calculado à representação;
5. Confirmar se a escala indicada na identificação da vista corresponde à escala desejada.

<!-- <span class="status-valid">VÁLIDO</span> -->
<!-- <span class="status-obsolete">OBSOLETO - dd/mm/yy</span> -->