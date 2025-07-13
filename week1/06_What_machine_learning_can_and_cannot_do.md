# Semana 1 – O que a IA pode e não pode fazer

## Contexto

- Antes de investir em um projeto de IA, é essencial fazer **diligência técnica**:
  - Mapear claramente: qual é o input A? qual é o output B?
  - Verificar se esse mapeamento A → B é algo que a IA *realmente consegue aprender*.

> 🧠 *Como dev:* Pense como se fosse avaliar uma dependência externa: antes de integrar, você verifica se resolve o problema real com os dados e limitações que você tem.

---

## Viés do sucesso

- A mídia e a academia tendem a publicar **apenas os casos de sucesso**.
- Isso cria uma percepção falsa de que IA pode resolver qualquer coisa — **não pode**.

---

## Regra prática (rule of thumb)

> “Se um ser humano pode resolver a tarefa em **menos de 1 segundo de raciocínio**, provavelmente pode ser automatizada com IA supervisionada.”

### Ex: Tarefas que funcionam bem com IA

- Detectar posição de carros ao dirigir.
- Avaliar se há um arranhão em um produto.
- Transcrever um áudio simples.

### Ex: Tarefas difíceis ou inviáveis com IA atual

- Prever o preço futuro de uma ação com base apenas no histórico dela.

> 💡 *Observação técnica:* Esse é um problema **altamente estocástico**. O passado de um ativo não determina seu futuro. ML precisa de padrão — e o mercado financeiro é quase aleatório nesses termos.

---

## Casos limítrofes

- Com dados externos (ex: tráfego de usuários, vendas), traders *podem* obter algum poder preditivo.
- Porém, ainda é limitado e caro de operacionalizar.

---

## Regras para estimar viabilidade de projetos com IA

1. **Conceito simples → mais viável**
   - Se você resolve com pouco raciocínio humano, é mais fácil de modelar.
   - Ex: detectar carros, classificar objetos visuais.
2. **Ter muitos dados rotulados A → B → mais viável**
   - Ex: milhares de imagens com rótulo “com arranhão” ou “sem arranhão” aumentam a chance de sucesso do modelo.

> 📌 *Insight dev:* Mesmo com dados "bons", a curadoria e pré-processamento (validação, limpeza, balanceamento) são cruciais. Não basta “ter dados”, é preciso **ter dados úteis e utilizáveis**.

---

## Conclusão

- IA é poderosa, mas não é mágica.
- Desenvolver **intuição sobre o que é viável** evita desperdício de tempo e investimento.
- Tarefas que exigem julgamento complexo, raciocínio estratégico ou criatividade aberta **ainda estão fora do alcance da IA supervisionada atual**.

> ⚙️ *Como dev líder:* Use essas regras ao ajudar seu time ou liderança a priorizar projetos — e evite promessas irreais que viram débito técnico ou desilusão.

---

### Próximo vídeo: mais exemplos de onde IA funciona bem ou mal — para continuar fortalecendo sua intuição.



# Semana 1 – Exemplos Práticos: Onde a IA Funciona e Onde Falha

## Por que ver exemplos importa?

- Projetos de IA reais ensinam limites e possibilidades da tecnologia.
- Se você faz só 1 projeto por ano, levaria anos para ter repertório de acertos e erros.
- Esses exemplos aceleram o desenvolvimento da **intuição prática** sobre o que é ou não viável com IA.

---

## Exemplo 1: Carros Autônomos

### ✅ O que IA consegue fazer bem
- Entrada (A): imagem + sensores (radar, lidar, etc.)
- Saída (B): posição dos outros veículos
- ✅ Detectar veículos é uma tarefa com conceito simples e muito dado disponível

### ❌ O que IA ainda não faz bem
- Entrada (A): vídeo curto de uma pessoa gesticulando
- Saída (B): intenção da pessoa (ex: pare, siga, vire)
- Problemas:
  - Alta variabilidade de gestos humanos
  - Pouco dado rotulado
  - Segurança crítica exige **altíssima precisão**

> 🧠 *Como dev:* Evite depender da IA para interpretar intenção implícita de humanos em contextos abertos (ex: gestos, expressões faciais, sinais contextuais).

---

## Exemplo 2: Diagnóstico Médico por Imagem

### ✅ Funciona bem
- Entrada (A): radiografias de tórax
- Saída (B): presença ou ausência de pneumonia
- Com muitos exemplos rotulados, IA pode superar humanos em tarefas específicas.

### ❌ Não funciona bem
- Entrada: apenas 10 imagens + explicações textuais de livro
- IA não aprende como um humano: **não consegue extrair generalizações a partir de poucos exemplos** e texto descritivo.

> 🧬 *Observação:* Aprendizado baseado em poucos exemplos (“few-shot learning”) ainda é um desafio em IA prática — especialmente fora dos LLMs.

---

## Generalização: o calcanhar de Aquiles da IA

- Modelos treinados com um tipo de dado (ex: imagens limpas) tendem a falhar com dados diferentes (ex: ângulos, ruídos, interferências).
- Exemplo: IA treinada com imagens de hospital A não funciona bem em hospital B com imagens mais sujas ou inclinadas.

> 💡 *Como dev:* Isso é equivalente a um sistema acoplado demais ao "happy path". Pense em robustez e testes com dados fora do padrão desde o início.

---

## Força e Limitações da IA (resumo)

| Quando IA funciona bem                        | Quando IA falha                                  |
|---------------------------------------------|--------------------------------------------------|
| Conceitos simples                            | Conceitos complexos ou subjetivos                |
| Grande volume de dados rotulados (A → B)     | Pouco dado ou com ruído                          |
| Domínio bem definido e fechado               | Domínio aberto, ambíguo ou com muita variabilidade |
| Entrada semelhante à vista no treino         | Entrada diferente (generalização fraca)          |

> ✅ *Dica prática:* Mesmo com boa intuição, avaliar viabilidade real de um projeto requer algumas semanas de **diligência técnica**.

---

## Conclusão da Semana 1

- Você agora conhece:
  - O que é IA, ML, DL e Data Science.
  - O papel dos dados e os erros comuns em estratégia de dados.
  - O que torna uma empresa boa em IA.
  - O que a IA pode e não pode fazer (com base em casos reais).

> ⚙️ *Como dev experiente*, você agora tem uma base sólida para:
> - Escolher projetos de IA mais realistas.
> - Ajudar a filtrar ideias com alto risco de fracasso técnico.
> - Contribuir tecnicamente e estrategicamente com iniciativas de IA em sua empresa.

---

### ▶️ Próximos Passos

- Dois vídeos opcionais sobre o funcionamento de **redes neurais** e **deep learning**.
- Semana 2: vamos explorar **como construir projetos de IA na prática**, com exemplos de processos, times e decisões técnicas.