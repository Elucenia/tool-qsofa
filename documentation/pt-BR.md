<!-- ELUCENIA technical documentation · qsofa · pt-BR · no clinical/professional/rights approval -->

# qSOFA (quick SOFA)

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/qsofa)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Frequência respiratória ≥ 22 irpm

`fr`

### Alteração do estado mental (Glasgow \< 15)

`mental`

### Pressão sistólica ≤ 100 mmHg

`pas`

## Edição do método

q SOFA/Sepsis 3/Seymour 2016:FR≥22/PAS≤100/alteração mental,0–3; sem recomendação rastreioisolado SSC 2021

## Fórmula documentada

Um ponto para cada: frequência respiratória ≥ 22/min, alteração do estado mental e pressão sistólica ≤ 100 mmHg. Positivo com 2 ou mais pontos.

## Limites e população

qSOFA2016 é um instrumento de risco em adultos com suspeita de infecção, não um diagnóstico nem um teste isolado para excluir sepse. Pontuação baixa não elimina suspeita clínica. A SSC2021 recomenda contra qSOFA como único instrumento de rastreamento; a orientação oficial SSC2026 mantém preferência por outros instrumentos de rastreamento hospitalar. A avaliação e o tratamento de emergência não devem aguardar o escore. Este limiar adulto não estabelece aplicação pediátrica.

## Referências

- [Seymour CW et al. Assessment of clinical criteria for sepsis: for the Third International Consensus Definitions for Sepsis and Septic Shock (Sepsis-3). JAMA, 2016.](https://doi.org/10.1001/jama.2016.0288)

- [Singer M et al. The Third International Consensus Definitions for Sepsis and Septic Shock (Sepsis-3). JAMA, 2016.](https://doi.org/10.1001/jama.2016.0287)

- [Evans L et al. Surviving sepsis campaign: international guidelines for management of sepsis and septic shock 2021. Intensive Care Med, 2021.](https://doi.org/10.1007/s00134-021-06506-y)

- [SSC adult guidelines2021](https://www.sccm.org/clinical-resources/guidelines/guidelines/surviving-sepsis-guidelines-2021)

- [SSC adult guidelines2026, current official page as observed2026-10-03](https://www.sccm.org/survivingsepsiscampaign/guidelines-and-resources/surviving-sepsis-campaign-adult-guidelines)

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
