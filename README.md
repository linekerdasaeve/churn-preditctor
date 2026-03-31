# 📉 Previsão de Churn de Clientes (Customer Churn Prediction)

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://churn-preditctor.onrender.com/)

Este é um projeto pessoal de Machine Learning focado em prever a evasão de clientes (*churn*). O modelo preditivo foi desenvolvido utilizando o algoritmo **XGBoost** e a interface web foi construída com a biblioteca **Streamlit**. O deploy online da aplicação foi realizado através da plataforma **Render**.

🌐 **Acesse a aplicação rodando online:** [Predictor App no Render](https://churn-preditctor.onrender.com/)

---

## 📂 Estrutura do Projeto

Os arquivos deste repositório estão organizados da seguinte forma:

* **`telco_churn_data.csv`**: O conjunto de dados (dataset) utilizado. Contém informações da empresa Telco, com 7.043 registros (linhas) e 21 atributos (colunas) sobre o comportamento dos clientes e o status de *churn*.
* **`customer_churn.ipynb`**: Jupyter Notebook contendo todo o processo de desenvolvimento. Inclui a Análise Exploratória de Dados (EDA), pré-processamento, construção, treinamento e avaliação do modelo.
* **`churn_encoders.pkl`**: Arquivo contendo os *encoders* (transformadores de variáveis categóricas) salvos após o treinamento. Eles são essenciais para garantir que os dados de entrada do usuário na aplicação web recebam exatamente o mesmo tratamento dos dados usados no treino.
* **`customer_churn_model.pkl`**: O modelo de Machine Learning (XGBoost) treinado e exportado. É este arquivo que o aplicativo carrega para fazer as predições em tempo real.
* **`churn_app.py`**: O código-fonte da nossa aplicação web (Frontend e integração com o modelo), escrito usando o Streamlit.
* **`requirements.txt`**: Lista de todas as bibliotecas e dependências do Python necessárias para rodar o projeto. Este arquivo é crucial para que o ambiente de deploy (Render) saiba o que instalar.

---

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python
* **Machine Learning:** XGBoost, Scikit-Learn, Pandas, NumPy
* **Desenvolvimento Web:** Streamlit
* **Deploy:** Render

---

## 💻 Como rodar o projeto localmente

Se você quiser clonar este projeto e rodá-lo na sua própria máquina, siga os passos abaixo:

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/linekerdasaeve/churn-preditctor.git]
   cd churn-preditctor.git
   
2. **Crie um ambiente virtual (Opcional, mas recomendado):**
	```bash
	python -m venv venv
	source venv/bin/activate  # No Windows use: venv\Scripts\activate
	
3. **Instale as dependências:**
	```bash
	pip install -r requirements.txt

4. **Execute a aplicação Streamlit:**
	```bash
	streamlit run churn_app.py

Após rodar o comando acima, a aplicação abrirá automaticamente no seu navegador padrão (geralmente no endereço http://localhost:8501).
