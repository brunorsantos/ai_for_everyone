# Semana 2 – Workflow de um projeto de Machine Learning

## Etapas principais de um projeto de ML

1. **Coletar dados**
2. **Treinar o modelo**
3. **Implantar o modelo (deploy)**
4. **Iterar constantemente** para melhorar performance

---

## Exemplo 1: Reconhecimento de fala (speech recognition)

- Objetivo: detectar quando alguém diz “Alexa”
- **Entrada (A):** clipe de áudio
- **Saída (B):** palavra detectada (ex: "Alexa" ou "Hello")

### Etapas:

- **1. Coletar dados:**  
  - Gravar pessoas dizendo “Alexa” e outras palavras
- **2. Treinar o modelo:**  
  - Usar algoritmo para aprender o mapeamento A → B
  - Primeiras tentativas geralmente falham → requer **muita iteração**
- **3. Deploy:**  
  - Embutir modelo no dispositivo (ex: Amazon Echo)
  - Exemplo de problema comum: sotaques diferentes (ex: britânico vs americano)
- **4. Atualizar com feedback:**  
  - Coletar dados de falhas reais e atualizar o modelo com isso

> 🧠 *Como dev:* Pense no deploy como ir “para produção”, e no feedback como **telemetria + aprendizado contínuo**. Sem feedback, o modelo pode estagnar.

---

## Exemplo 2: Detecção de veículos para carro autônomo

- Objetivo: identificar a posição de outros carros a partir de imagens
- **Entrada (A):** imagem da câmera frontal
- **Saída (B):** posições dos veículos (retângulos delimitando os carros)

### Etapas:

- **1. Coletar dados:**
  - Capturar imagens e rotulá-las com bounding boxes dos carros
- **2. Treinar modelo:**
  - Primeiras versões falham (ex: confundem postes com carros)
  - Iteração até que a performance melhore
- **3. Deploy com segurança:**
  - Colocar em carros-teste
  - Novos casos como **golf carts** exigem atualização
- **4. Manutenção contínua:**
  - Coletar novos dados de falhas e re-treinar o modelo

> 🚗 *Observação dev:* Isso se assemelha a **testes A/B com rollback** + coleta de logs e reprocessamento. Aqui, porém, a “regra de negócio” é aprendida, não programada.

---

## Conclusão

- O fluxo de projeto em ML é iterativo por natureza.
- Mesmo após o deploy, espera-se coletar dados, revisar erros e melhorar.
- **Etapas clássicas:**
  1. Coleta
  2. Treinamento
  3. Deploy
  4. Iteração + re-treinamento

> 🔁 *Como desenvolvedor*, você pode aplicar práticas similares às de CI/CD:
> - Versão de modelo
> - Automação de testes com dados reais
> - Observabilidade e métricas de inferência

---

### ▶️ Próximo vídeo: Workflow de um projeto de Data Science