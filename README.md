# Desenvolvimento de Agente Inteligente para Solução de Problemas

Este repositório contém o projeto final para a disciplina de **Inteligência Artificial**, no qual foi desenvolvido um agente inteligente baseado em **Algoritmos Genéticos** para resolver o problema da **Mochila 0/1**.

---

## 👥 Contribuidores
- [Matheus Morandi Cabral Domingos](https://github.com/MatheusMorandi)
- [Victor Yuchi Kashima ](https://github.com/VictorKashima)

---

## 📌 **Objetivo do Projeto**
Desenvolver um agente inteligente que utilize um método de otimização inspirado na seleção natural para resolver o problema da mochila, um clássico problema de otimização combinatória. O agente é capaz de:
- Analisar o ambiente (lista de itens com pesos e valores e a capacidade máxima da mochila).
- Tomar decisões autônomas sobre quais itens selecionar.
- Melhorar seu desempenho ao longo de várias gerações por meio de mecanismos de seleção, crossover e mutação.

---

## 🛠️ **Descrição do Problema**
O problema da **Mochila 0/1** consiste em determinar a combinação ideal de itens a serem incluídos em uma mochila, de forma a maximizar o valor total sem exceder a capacidade máxima permitida. Cada item possui:
- Um **peso**, que ocupa espaço na mochila.
- Um **valor**, que representa sua importância.

O desafio do agente é encontrar a melhor combinação que atenda às restrições do problema.

---

## 🤖 **Implementação do Agente Inteligente**
O agente foi projetado para simular um processo evolutivo. Ele inclui os seguintes componentes:

### **1. Sensores**
- Coletam informações sobre o ambiente, como:
  - Lista de itens com pesos e valores.
  - Capacidade máxima da mochila.

### **2. Atuadores**
- Realizam ações no ambiente ao selecionar combinações de itens e avaliar sua adequação.

### **3. Base de Conhecimento**
- Estruturada com dados dos itens disponíveis e regras de operação:
  - Peso máximo permitido.
  - Relação entre o valor e o peso de cada item.

### **4. Método de Aprendizagem**
- **Algoritmo Genético**:
  - **População Inicial**: Conjunto aleatório de soluções candidatas.
  - **Fitness**: Mede a qualidade de cada solução com base no valor total dos itens selecionados e na penalidade por excesso de peso.
  - **Seleção por Roleta Viciada**: Prioriza indivíduos com maior fitness para reprodução.
  - **Crossover**: Combina características de dois indivíduos para criar descendentes.
  - **Mutação**: Introduz variações aleatórias para evitar estagnação.

---

## 🎯 **Função do Agente**
O agente foi projetado para:
- Encontrar a melhor combinação de itens que maximize o valor total dentro da capacidade da mochila.
- Aprender e melhorar a qualidade das soluções ao longo de várias gerações.

---

## 📊 **Avaliação de Performance**
Foram realizados testes com diferentes listas de itens e capacidades, com o intuito de avaliar o desempenho do agente em diferentes cenários.

---

## 🎥 **Vídeo Demonstrativo**
O vídeo explicativo do projeto pode ser encontrado [aqui](https://www.youtube.com/watch?v=DcVpWLeXb2s&t). Ele inclui:
1. Descrição do problema e do ambiente.
2. Demonstração do funcionamento do agente.
3. Comparação dos resultados obtidos em diferentes cenários.

---

## 📂 **Notebook**
O código completo do agente está implementado em um **Jupyter Notebook** para facilitar a execução e análise. 

### **Como Executar**
1. Clone este repositório:
   ```bash
   git clone https://github.com/MatheusMorandi/Agente-Inteligente-Algoritmo-Genetico

2. Acesse o diretório:
   ```bash
    cd Agente-Inteligente-Algoritmo-Genetico

3. Abra o notebook:
   ```bash
   jupyter notebook algoritmo_genetico.ipynb
