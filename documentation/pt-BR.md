<!-- ELUCENIA technical documentation · timi-sca · pt-BR · no clinical/professional/rights approval -->

# Escore TIMI (SCA sem supra de ST)

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/timi-sca)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Idade ≥ 65 anos

`idade`

### ≥ 3 fatores de risco para DAC

`fr`

### Estenose coronária conhecida ≥ 50%

`dac`

### Uso de AAS nos últimos 7 dias

`aas`

### ≥ 2 episódios de angina em 24 horas

`angina`

### Desvio do ST ≥ 0,5 mm

`st`

### Marcador de necrose elevado

`marc`

## Edição do método

TIMIUA/NSTEMI/Antman 2000:7 fatores 0–1, total 0–7; sem TIMISTEMI

## Fórmula documentada

Um ponto por item presente (total de 0 a 7).

## Limites e população

Esta versão TIMI foi desenvolvida em angina instável e infarto sem supradesnível, para desfechos compostos em 14 dias, e não é a versão TIMI para STEMI. Os fatores têm definições temporais e clínicas específicas. Taxas dos ensaios históricos não determinam risco individual ou tratamento atual sem avaliação e diretriz correspondentes.

## Referências

- [Antman EM et al. The TIMI risk score for unstable angina/non–ST elevation MI. JAMA, 2000.](https://doi.org/10.1001/jama.284.7.835)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

As informações abaixo preservam as saídas do método para exemplos sintéticos. Não constituem validação clínica independente.

### 1

Benefício de estratégia invasiva precoce

| Detalhes do resultado | |
| --- | --- |
| Morte, IAM ou revascularização urgente em 14 dias | 13,2% |


### 2

Benefício de estratégia invasiva precoce

| Detalhes do resultado | |
| --- | --- |
| Morte, IAM ou revascularização urgente em 14 dias | 26,2% |


### 3

Risco baixo

| Detalhes do resultado | |
| --- | --- |
| Morte, IAM ou revascularização urgente em 14 dias | 4,7% |

