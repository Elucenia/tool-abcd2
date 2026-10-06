<!-- ELUCENIA technical documentation · abcd2 · pt-BR · no clinical/professional/rights approval -->

# Escore ABCD²

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/abcd2)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Idade ≥ 60 anos

`idade`

### Pressão arterial ≥ 140/90 mmHg na primeira avaliação

`pa`

### Manifestação clínica

`clinica`

- `0` — Outros sintomas
- `1` — Alteração da fala sem fraqueza
- `2` — Fraqueza unilateral

### Duração dos sintomas

`duracao`

- `0` — \< 10 min
- `1` — 10 a 59 min
- `2` — ≥ 60 min

### Diabetes

`dm`

## Edição do método

ABCD 2/Johnston 2007:idade/PA/clínica/duração/diabetes, total 0–7

## Fórmula documentada

Age (idade ≥ 60) 1 · Blood pressure (≥ 140/90) 1 · Clínica: fraqueza unilateral 2, fala sem fraqueza 1 · Duração: ≥ 60 min 2, 10 a 59 min 1 · Diabetes 1. Total: 0 a 7.

## Limites e população

Escore prognóstico após um diagnóstico de AIT, estudado principalmente para risco de AVC em 2 dias, com análise adicional em 7 e 90 dias. Não confirma o diagnóstico de AIT. As probabilidades observadas nas coortes originais não representam uma previsão individual universal.

## Referências

- [Johnston SC et al. Validation and refinement of scores to predict very early stroke risk after transient ischaemic attack. Lancet, 2007.](https://doi.org/10.1016/S0140-6736(07)60150-0)

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

Baixo risco: AVC em 2 dias de 1,0%

7 dias: 1,2% · 90 dias: 3,1%.


### 2

Risco moderado: AVC em 2 dias de 4,1%

7 dias: 5,9% · 90 dias: 9,8%.


### 3

Alto risco: AVC em 2 dias de 8,1%

7 dias: 11,7% · 90 dias: 17,8%.

