# Semana 2 – Colaboração com times de IA

## Como colaborar com um time de IA

### Começando um projeto com um time de IA

- Mesmo sem engenheiros de IA disponíveis, é possível começar:
  - Incentive engenheiros a fazer cursos online de **Machine Learning / Deep Learning**.
  - Conhecimento introdutório já é suficiente para iniciar projetos viáveis.

---

## Especificação de critérios de aceitação

- Defina uma **meta clara de desempenho** para o sistema de IA.
  - Ex: "Detectar defeitos em canecas com **95% de acurácia**".

### Como medir essa acurácia?

- É necessário um **conjunto de dados com rótulos corretos**.
- Este conjunto é chamado de **test set**:
  - Ex: imagens de canecas com rótulos indicando se são “ok” ou “defeituosas”.
  - Pode conter poucas centenas ou milhares de exemplos, dependendo do problema.
- A meta de acurácia é **estatística**, e não determinística:
  - Ex: 95% de acurácia média, e não perfeição em todos os casos.

> 🎯 *Como dev:* já pense em como os dados de produção podem ser versionados, rotulados e mantidos de forma auditável para treinamento e validação.

---

## Como times de IA pensam sobre dados

- Dois principais conjuntos:
  - **Training set**: usado para treinar o modelo (A ➝ B).
  - **Test set**: usado para avaliar o modelo de forma objetiva.

### Outras divisões comuns

- Muitos times também usam:
  - **Validation set** (também chamado de dev set): para afinar hiperparâmetros.
  - **Final test set**: usado apenas no final, sem viés de ajuste.

> 🧪 *Insight técnico:* pense no split em 70/15/15 (train/val/test) como padrão inicial, mas adaptável conforme o volume e a complexidade do dado.

---

## Expectativas realistas: evite exigir 100% de acurácia

### Por que 100% é irreal?

1. **Limitações do estado da arte**: ML ainda não resolve tudo.
2. **Poucos dados**: modelos precisam de exemplos representativos.
3. **Dados sujos ou com rótulos errados**.
4. **Ambiguidade intrínseca nos exemplos**:
   - Ex: risco de especialistas discordarem sobre se um item é defeituoso ou não.

### Estratégias para mitigar:

- Coletar mais dados.
- **Limpar rótulos** com revisão humana.
- Definir critérios claros de **classificação ambígua**.

> ⚠️ *Como desenvolvedor:* contribua no desenho do pipeline de **validação cruzada**, gerenciamento de **data drift** e **consistência de labels** com ferramentas como DVC, Weights & Biases, ou frameworks internos.

---

## Resumo final da semana

- Aprendemos a:
  - Selecionar projetos viáveis e valiosos (interseção entre IA e negócio).
  - Conduzir diligência técnica, de negócio e ética.
  - Colaborar com times de IA, entendendo como pensam sobre dados.
- Evite tentar reinventar a roda em componentes padrão.
- Use métricas realistas e tenha clareza de dados desde o início.

---

### ✅ Próximo passo: ver como projetos de IA se encaixam no contexto organizacional e sua escalabilidade