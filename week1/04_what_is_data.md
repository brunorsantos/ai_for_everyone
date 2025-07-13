# Semana 1 – O que é dado (data)

## O que é um conjunto de dados?

- Um conjunto de dados (dataset) pode ser tão simples quanto uma planilha com colunas (ex: tamanho da casa e preço).
- O que é considerado entrada (A) e saída (B) depende do objetivo do negócio:
  - Exemplo 1: A = tamanho + número de quartos | B = preço da casa.
  - Exemplo 2: A = orçamento | B = tamanho da casa possível.

## Exemplos de datasets

- **Classificação de imagens**: A = imagem | B = rótulo (gato ou não).
- **Histórico de navegação de usuários**: comportamento dos usuários serve de base para datasets de recomendação e previsão.
- **Sensores de máquinas**: dados como temperatura e pressão podem ser usados para prever falhas.

## Como adquirir dados

1. **Rotulagem manual (manual labeling)**:
   - Humanos identificam e classificam elementos em um conjunto de dados.
   - Útil para casos como imagens de gatos.
2. **Observação de comportamento**:
   - Ex: registrar se o usuário comprou ou não após ver um produto.
   - Também vale para sensores em máquinas industriais.
3. **Dados públicos ou de parceiros**:
   - Muitos datasets estão disponíveis online (visão computacional, reconhecimento de fala, etc).
   - Parcerias com empresas que já coletaram dados também são uma opção.

## Erros comuns na estratégia de dados

- **Erro 1: “Vamos coletar dados por 3 anos e só depois usar IA”**:
  - Estratégia ineficaz.
  - Melhor: coletar dados e já envolver o time de IA desde o início para ajustar o que deve ser coletado.

- **Erro 2: “Temos muitos dados, logo conseguimos gerar valor”**:
  - Nem todo dado é útil.
  - Quantidade ≠ qualidade.
  - Terabytes de dados irrelevantes não garantem sucesso sem análise estratégica e alinhamento com aplicações de IA.

## Dados são bagunçados (data is messy)

- Problemas comuns:
  - **Rótulos incorretos**: Ex: casa com preço de $1.
  - **Dados ausentes**: campos vazios ou desconhecidos.
- O time de IA precisa lidar com:
  - Limpeza de dados (data cleaning).
  - Estratégias para lidar com ausência ou erro de informação.

## Tipos de dados

- **Dados não estruturados (unstructured)**:
  - Ex: imagens, áudios, textos.
  - Interpretados facilmente por humanos.
  - Utilizam técnicas específicas de IA.

- **Dados estruturados (structured)**:
  - Ex: tabelas com colunas fixas (como planilhas).
  - Técnicas de IA para dados estruturados são diferentes das usadas com dados não estruturados.

- **Observação**:
  - A IA generativa trabalha principalmente com dados não estruturados.
  - Supervised learning funciona bem com **ambos os tipos**.

## Conclusão

- Dados são fundamentais para IA, mas **qualidade > quantidade**.
- Envolver o time de IA cedo é essencial para:
  - Coletar os dados certos.
  - Evitar desperdício de esforço e investimento.
- Bons times de IA conseguem contornar dados imperfeitos, desde que tenham contexto e envolvimento com o problema real.

> Próximo vídeo: definição clara dos termos IA, Machine Learning e Data Science.