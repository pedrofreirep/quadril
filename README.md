# Projeto: Predição de Complicações Hospitalares e Óbitos com Random Forest

---

## **Descrição do Projeto**

Este repositório contém o desenvolvimento de um modelo preditivo baseado em **Random Forest** para identificar **complicações hospitalares** e **óbitos** em pacientes hospitalizados. O objetivo principal do projeto é aplicar técnicas avançadas de análise de dados e aprendizado de máquina para fornecer insights acionáveis e melhorar a qualidade e eficiência dos cuidados hospitalares.

Este projeto foi desenvolvido pela **Blue**, uma empresa dedicada a criar soluções baseadas em inteligência artificial para otimizar planos de saúde empresariais e reduzir custos hospitalares desnecessários.

---

## **Objetivos do Projeto**

1. **Predição de Complicações Hospitalares**:
   - Identificar pacientes com maior risco de complicações clínicas (ex.: infecções, atrasos no atendimento, etc.).
   - Auxiliar em intervenções preventivas para reduzir eventos adversos.

2. **Predição de Óbitos**:
   - Prever o risco de mortalidade hospitalar com base em variáveis demográficas, clínicas e temporais.
   - Priorização de casos críticos para intervenções mais rápidas e eficazes.

3. **Melhoria de Decisões Clínicas**:
   - Fornecer suporte a decisões clínicas por meio de análises preditivas.
   - Comparar o desempenho dos modelos com o Índice de Charlson.

4. **Contribuir para a Automação de Planos de Saúde Empresariais**:
   - Criar ferramentas que permitam à **Blue** oferecer soluções de otimização de custos com base em modelos robustos de predição.

---

## **Estrutura do Repositório**

- **`notebooks/`**:
  - Contém os notebooks com o desenvolvimento, tratamento dos dados e experimentos com os modelos preditivos.
- **`data/`**:
  - Conjunto de dados utilizado (não incluído no repositório por questões de privacidade).
  - Instruções para o uso de dados podem ser encontradas na seção **Como Utilizar**.
- **`scripts/`**:
  - Scripts de pré-processamento, treinamento do modelo e avaliação.
- **`outputs/`**:
  - Resultados dos modelos (curvas ROC, matrizes de confusão e métricas de performance).
- **`README.md`**:
  - Documento atual que descreve o projeto.

---

## **Tecnologias Utilizadas**

- **Linguagem**:
  - Python 3.9
- **Bibliotecas Principais**:
  - `pandas`, `numpy`: Manipulação e análise de dados.
  - `scikit-learn`: Algoritmos de aprendizado de máquina.
  - `imblearn`: Técnicas de balanceamento de classes (ex.: SMOTE).
  - `matplotlib`, `seaborn`: Visualização de dados.
  - `graphviz`: Visualização de árvores de decisão.

---

## **Principais Funcionalidades**

### 1. **Modelos de Previsão**
- Dois modelos preditivos foram desenvolvidos:
  - **Complicações Hospitalares**:
    - Previsão de eventos adversos baseados em variáveis como infecção, tempo até cirurgia e idade.
  - **Óbitos**:
    - Modelo mais avançado para prever mortalidade hospitalar.

### 2. **Técnicas de Pré-Processamento**
- Tratamento de dados categóricos (ex.: variáveis como "Eletiva", "Infecção").
- Criação de variáveis derivadas, como:
  - Faixas etárias.
  - Faixas temporais para tempos hospitalares (ex.: TEMPO ATÉ CIRURGIA).
  - Variáveis binárias para tipos de cirurgias e complicações.

### 3. **Visualização**
- Curvas ROC para avaliar a performance do modelo.
- Matrizes de confusão para análise de erros.
- Visualização de árvores de decisão para entender as regras do modelo.

### 4. **Comparação com o Índice de Charlson**
- Charlson foi usado como baseline para comparar a eficiência dos modelos.
- Random Forest se mostrou mais adaptável e eficaz em cenários específicos.
