# Semana 2 (Opcional) – Ferramentas Técnicas Usadas por Times de IA

## Principais frameworks e ferramentas open-source

- **Frameworks de Machine Learning mais comuns:**
  - `PyTorch`
  - `TensorFlow`
  - `Hugging Face`
  - `PaddlePaddle`
  - `Scikit-Learn`
  - `R`

- **Plataformas de código aberto:**
  - [arXiv.org](https://arxiv.org): publicações científicas em IA.
  - [GitHub](https://github.com): principal repositório de software open-source, incluindo muitos projetos de IA.
    - Verifique sempre a **licença** antes de usar código em produtos.

> 💡 *Como dev:* vale acompanhar repositórios populares (e.g. `ultralytics/yolov5`, `facebookresearch/segment-anything`, `openai/whisper`) para entender tendências de mercado e basear provas de conceito.

---

## Hardware para IA

### CPUs e GPUs

- **CPU** (Central Processing Unit):
  - Processador principal de um computador.
  - Fabricantes: Intel, AMD.

- **GPU** (Graphics Processing Unit):
  - Originalmente usada para processar gráficos (ex: jogos).
  - Hoje, muito usada para **treinar redes neurais profundas** com grandes volumes de dados.
  - Principais fabricantes: `NVIDIA` (líder), `AMD`, `Google TPU`, `Qualcomm`.

> 🧠 *Insight técnico:* GPUs são massivamente paralelas — ideais para os cálculos de matriz/tensor intensivos em redes neurais.

---

## Tipos de deploy em IA

### 1. **Cloud**
- Computação alugada em provedores como:
  - `AWS`, `Azure`, `GCP`.
- Popular pela escalabilidade e custo inicial menor.

### 2. **On-premises (on-prem)**
- Infraestrutura comprada e operada dentro da própria empresa.
- Útil em casos de exigências rígidas de compliance, privacidade ou latência controlada.

### 3. **Edge deployment**
- Computação acontece no próprio dispositivo onde os dados são gerados:
  - Exemplos: carros autônomos, smart speakers.
- **Vantagens:**
  - Baixa latência.
  - Menor uso de rede.
  - Privacidade (dados não saem do dispositivo).

> ⚙️ *Como dev:* edge computing exige considerar footprint de memória e CPU, e usar bibliotecas otimizadas como `TensorFlow Lite`, `ONNX Runtime`, `CoreML`.

---

## Conclusão

- A IA moderna é viabilizada por um ecossistema vasto e aberto de ferramentas, publicações e repositórios.
- Entender o **vocabulário técnico** dos times de IA ajuda a colaborar melhor e a tomar decisões mais conscientes sobre arquitetura e infraestrutura.
- Saber escolher entre **cloud, edge ou on-prem** depende do caso de uso, requisitos de performance e orçamento.