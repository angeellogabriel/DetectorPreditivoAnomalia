Este projeto simula sensores industriais (temperatura e vibração) e aplica **Redes Neurais Autoencoder** para identificar **anomalias operacionais**, com foco em **manutenção preditiva**.

---

## 🎯 Objetivo

Criar um sistema completo que:

- Gere dados de sensores com anomalias realistas
- Treine um modelo Autoencoder para detectar falhas
- Visualize resultados em um **Dashboard interativo (Dash)**
- Salve e monitore dados para análise posterior

---

## ⚙️ Tecnologias utilizadas

- `Python`
- `TensorFlow / Keras`
- `Dash (Plotly)`
- `scikit-learn`, `pandas`, `matplotlib`
- Autoencoder para detecção de anomalias

---

## 📁 Estrutura do Projeto

anomaly-detector-predictive/
├── data/ ← Dados brutos e anotados

├── models/ ← Modelos salvos (.h5, scaler)

├── scripts/ ← Scripts de geração, treino e inferência

├── dashboard/ ← Dashboard interativo com Dash

├── notebooks/ ← Notebook de análise exploratória (opcional)

└── requirements.txt


---

## 🔄 Etapas do Projeto

1. `scripts/generate_dataset.py`  
   Gera `sensor_data.csv` com anomalias em temperatura e vibração.

2. `scripts/train_model.py`  
   Treina um modelo **Autoencoder** usando apenas dados normais, calcula o erro de reconstrução e salva os arquivos.

3. `scripts/detect_anomalies.py`  
   Detecta anomalias no dataset completo e marca os pontos com erro alto.

4. `dashboard/app.py`  
   Interface interativa com gráfico de temperatura, vibração e contador de anomalias.

---

## 📊 Exemplo do Dashboard

![Dashboard de Manutenção Preditiva-1](https://github.com/user-attachments/assets/8186d055-28df-4b7e-a5e7-e50209789908)


