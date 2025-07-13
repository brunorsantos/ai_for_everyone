# Semana 2 – Workflow de um projeto de Data Science

## Diferença em relação a projetos de Machine Learning

- **ML:** objetivo é produzir um *modelo* que automatize algo (A → B)
- **Data Science:** objetivo é produzir **insights acionáveis** que informam decisões humanas

---

## Etapas de um projeto de Data Science

1. **Coleta de dados**
2. **Análise exploratória**
3. **Geração de hipóteses e recomendações**
4. **Acompanhamento e reanálise com novos dados**

---

## Exemplo 1: Otimização de funil de vendas (e-commerce de canecas)

### Etapa 1 – Coleta de dados
- Captura do caminho dos usuários no site (visita, página do produto, carrinho, checkout)
- Informações adicionais: IP, país, horário de acesso, etc.

### Etapa 2 – Análise de dados
- Equipe de Data Science testa hipóteses como:
  - Abandono no checkout por custo de frete
  - Variações sazonais (feriados, horários de trabalho)
  - Influência de hábitos culturais (ex: siesta em alguns países)

### Etapa 3 – Geração de recomendações
- Incorporar parte do frete no preço do produto
- Reduzir campanhas publicitárias durante a siesta
- Promover mais em horários estratégicos

### Etapa 4 – Coleta de novos dados após mudanças
- Avaliar impacto das mudanças
- Iterar com novos testes e hipóteses

> 🧠 *Como dev:* Isso se aproxima de uma cultura de **experimentos orientados por dados**, como A/B testing, mas com foco em análise exploratória antes de ação.

---

## Exemplo 2: Otimização de linha de produção (fábrica de canecas)

### Etapa 1 – Coleta de dados
- Informações de cada etapa do processo:
  - Fornecedor do barro, tempo de mistura, umidade, temperatura, tempo de queima

### Etapa 2 – Análise de dados
- Descobertas possíveis:
  - Baixa umidade + alta temperatura = rachaduras
  - Ajustes ideais variam com a hora do dia (temperatura ambiente)

### Etapa 3 – Ações sugeridas
- Ajustar parâmetros dinamicamente
- Criar protocolos para manter variáveis dentro de faixas ideais

### Etapa 4 – Recoleta e reavaliação
- Medir impacto sobre taxa de produtos descartados
- Novas análises, novas melhorias

> ⚙️ *Observação dev:* Pode se integrar com sistemas de controle em tempo real e pipelines de ingestão de dados (IoT, sensores, dashboards).

---

## Conclusão

- **Data Science é um processo cíclico** de investigação e recomendação.
- Não exige um modelo de predição, mas exige:
  - **Curiosidade analítica**
  - **Domínio dos dados**
  - **Capacidade de comunicar descobertas com clareza**

> 💡 *Como desenvolvedor*: Você pode apoiar projetos de Data Science ao:
> - Garantir qualidade e acesso aos dados
> - Automatizar ingestão e transformação (ETL/ELT)
> - Ajudar a implementar as ações sugeridas com rapidez e segurança

---

### ▶️ Próximo vídeo: Como IA e Data Science estão transformando várias funções dentro das empresas – incluindo a sua.