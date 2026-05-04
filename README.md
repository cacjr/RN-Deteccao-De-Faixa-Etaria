# Projeto Totem Inteligente de Detecção de Faixa Etária

## Visão Geral

Este projeto tem como objetivo desenvolver um sistema inteligente capaz de detectar pessoas em imagens, estimar suas idades e classificá-las em diferentes faixas etárias utilizando técnicas de Visão Computacional e Deep Learning.

A solução simula o funcionamento de um totem inteligente que pode ser utilizado em ambientes como:

* shoppings
* eventos
* totens publicitários
* aeroportos
* centros comerciais
* jogos interativos
* campanhas de marketing personalizadas

O sistema utiliza:

* **YOLOv8** para detecção de pessoas
* **DeepFace** para estimativa de idade
* lógica personalizada para classificação etária
* painel de recomendações baseado na faixa detectada

---

# Objetivos do Projeto

* Detectar pessoas em imagens
* Estimar idade automaticamente
* Classificar faixas etárias
* Exibir recomendações personalizadas
* Avaliar desempenho da pipeline
* Aplicar conceitos de Deep Learning e Visão Computacional

---

# Tecnologias Utilizadas

* Python
* Google Colab
* OpenCV
* YOLOv8 (Ultralytics)
* DeepFace
* Pandas
* Matplotlib
* NumPy

---

# Estrutura da Pipeline

O fluxo do sistema funciona da seguinte maneira:

Entrada da imagem
↓
Detecção da pessoa com YOLOv8
↓
Recorte da região detectada
↓
Estimativa de idade com DeepFace
↓
Classificação da faixa etária
↓
Exibição das recomendações

---

# Faixas Etárias Utilizadas

| Faixa       | Intervalo    |
| ----------- | ------------ |
| Criança     | 0 a 12 anos  |
| Adolescente | 13 a 17 anos |
| Adulto      | 18 a 59 anos |
| Idoso       | 60+ anos     |

---

# Funcionalidades

* Detecção automática de pessoas
* Estimativa de idade em tempo real
* Bounding boxes nas imagens
* Exibição da faixa etária prevista
* Sistema de recomendação personalizado
* Avaliação automática dos resultados
* Cálculo de acurácia
* Medição de tempo de execução

---

# Dataset Utilizado

O projeto utiliza uma amostra reduzida do dataset **UTKFace**, contendo imagens faciais de diferentes idades.

O padrão dos arquivos segue o formato:

idade_genero_raca_data.jpg

Exemplo:

54_0_3_201701.jpg

Onde:

* 54 = idade
* 0 = gênero
* 3 = raça

A idade real é utilizada para validação automática da pipeline.

---

# Como Executar o Projeto

## 1. Clone o repositório

```bash
git clone LINK_DO_REPOSITORIO
```

---

## 2. Instale as dependências

```bash
pip install ultralytics
pip install deepface
pip install opencv-python
pip install tensorflow
pip install matplotlib
pip install pandas
```

---

## 3. Execute o notebook

Abra o arquivo `.ipynb` no:

* Google Colab
  ou
* Jupyter Notebook

Execute as células em ordem.

---

# Estrutura do Projeto

```bash
 projeto-totem
│
├── notebook.ipynb
├── README.md
├── requirements.txt
├── dataset/
└── resultados/
```

---

# Resultados Obtidos

O sistema conseguiu:

* detectar pessoas corretamente
* estimar faixas etárias
* gerar recomendações automáticas
* apresentar boa organização da pipeline

Também foram identificadas limitações relacionadas:

* iluminação
* qualidade da imagem
* ângulo facial
* oclusões
* maquiagem
* baixa resolução

---

# Melhorias Futuras

* Integração com webcam em tempo real
* Dashboard visual
* Recomendações mais inteligentes
* Treinamento de modelo próprio
* Otimização de desempenho
* Processamento em tempo real
* Uso de GPU dedicada

---

# Aprendizados

Durante o desenvolvimento do projeto foram aplicados conceitos importantes de:

* Redes Neurais
* Deep Learning
* Visão Computacional
* Detecção de Objetos
* Processamento de Imagens
* Engenharia de Pipeline
* Avaliação de Modelos

Além disso, o projeto contribuiu para o entendimento prático sobre integração entre múltiplos modelos de IA em uma única solução.

---

# Integrantes

* Claudio Alves
* Rodrigo Wolkoff
* Luna Rousseau
* Mario Oliveira
* Vinicius Silva

Turma: 1TIAPR

---

# Considerações Finais

O projeto demonstrou como técnicas modernas de Inteligência Artificial podem ser utilizadas para criar soluções inteligentes e interativas voltadas para análise de público e personalização de experiência.

Mesmo sendo um protótipo acadêmico, a arquitetura desenvolvida possui potencial de adaptação para aplicações reais em diferentes contextos comerciais e tecnológicos.
