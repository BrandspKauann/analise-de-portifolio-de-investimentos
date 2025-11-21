# 📊 Otimização de Portfólio de Investimentos (Teoria de Markowitz)

## 💡 Visão Geral do Projeto

Este projeto aplica a **Teoria Moderna do Portfólio (MPT)**, desenvolvida por Harry Markowitz, para encontrar a alocação de ativos que oferece o melhor equilíbrio entre **Retorno e Risco (Máximo Sharpe Ratio)**.

O objetivo é simular milhares de combinações de pesos para um portfólio de três ativos e identificar a **Fronteira Eficiente**, que é a melhor curva de risco/retorno possível.

---

## 🚀 Tecnologias e Metodologia

| Fase | Descrição | Foco | Ferramentas Chave |
| :--- | :--- | :--- | :--- |
| **Data Prep** | Estruturação de dados de retornos mensais simulados para 3 ativos (Alto, Médio e Baixo Risco). | Séries Temporais | `Pandas` |
| **Cálculo Básico** | Determinação do **Retorno Médio Anualizado** e da **Matriz de Covariância** (o risco de cada ativo em relação aos outros). | Risco e Correlação | `NumPy` |
| **Algoritmo** | **Simulação de Monte Carlo** (5.000 iterações de alocação de pesos). | Otimização | `NumPy` |
| **Avaliação** | **Sharpe Ratio** (Métrica de Retorno Ajustado ao Risco). | Otimização | `NumPy` |

---

## 🎯 Resultados da Otimização

A simulação de Monte Carlo identificou o portfólio que gera o maior Sharpe Ratio, indicando a alocação mais eficiente.

### 1. Métricas Chave do Portfólio Otimizado

| Métrica | Resultado |
| :--- | :--- |
| **Sharpe Ratio Máximo** | **34.09** |
| Retorno Anualizado Esperado | **6.19%** |
| Volatilidade (Risco) Anualizada | **0.18%** |

### 2. Alocação Otimizada (Pesos)

| Ativo | Tipo de Risco | Peso Otimizado |
| :--- | :--- | :--- |
| **Retorno A** (Crescimento/Alto Risco) | Alto | 0.1% |
| **Retorno B** (Valor/Médio Risco) | Médio | **39.9%** |
| **Retorno C** (Renda Fixa/Baixo Risco) | Baixo | **60.0%** |

> **Conclusão de Risco:** O modelo otimizado sugere evitar o ativo de alto risco (A), concentrando o investimento nos ativos de **Risco Médio (B)** e **Baixo Risco (C)** para alcançar o melhor retorno com a menor volatilidade.
