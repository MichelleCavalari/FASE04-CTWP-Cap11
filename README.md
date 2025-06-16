# 🌾 Classificação de Grãos de Trigo com Machine Learning

Projeto desenvolvido na graduação em Inteligência Artificial da FIAP, com o objetivo de automatizar a classificação de grãos de trigo utilizando técnicas de aprendizado de máquina, aplicando a metodologia CRISP-DM.

---

## 🚜 Contexto

Em cooperativas agrícolas de pequeno porte, a classificação dos grãos é realizada manualmente, o que demanda tempo e pode levar a erros humanos. Com o avanço da IA, é possível automatizar esse processo com alta precisão.

---

## 📊 Dataset

Utilizado o [Seeds Dataset (UCI ML Repo)](https://archive.ics.uci.edu/dataset/236/seeds), com 210 amostras de três tipos de grãos:

- Kama
- Rosa
- Canadian

### Atributos:

- Área
- Perímetro
- Compacidade
- Comprimento do Núcleo
- Largura do Núcleo
- Coeficiente de Assimetria
- Comprimento do Sulco do Núcleo

---

## 🧠 Metodologia CRISP-DM

| Etapa                 | Ação                                                                 |
|----------------------|----------------------------------------------------------------------|
| Entendimento do Negócio | Automatizar a classificação de grãos.                            |
| Entendimento dos Dados | Análise estatística e visual dos atributos.                       |
| Preparação dos Dados    | Escalonamento com `StandardScaler`.                              |
| Modelagem               | Aplicação de 5 modelos de classificação.                          |
| Avaliação               | Acurácia, F1-Score, Matriz de Confusão.                          |
| (Opcional) Deploy       | Sugestão: Interface com Streamlit.                               |

---

## 🤖 Modelos Aplicados

- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- Random Forest
- Naive Bayes
- Regressão Logística

Comparamos também as versões **otimizadas** com `GridSearchCV`:

| Modelo               | Acurácia (Antes) | Acurácia (Depois) |
|---------------------|------------------|-------------------|
| KNN                 | 0.85             | 0.90              |
| SVM                 | 0.88             | 0.92              |
| Random Forest       | 0.89             | 0.93              |

---

## 📈 Resultados

O modelo com melhor desempenho foi:

- 🏆 **Random Forest Otimizado** – Acurácia: 0.93

---

## 📦 Requisitos

```bash
pip install pandas matplotlib seaborn scikit-learn
