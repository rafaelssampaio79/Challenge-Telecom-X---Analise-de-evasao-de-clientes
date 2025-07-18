
# 📊 Análise de Evasão de Clientes - TelecomX

Este projeto tem como objetivo realizar uma análise exploratória detalhada sobre o comportamento de clientes de uma empresa de telecomunicações fictícia, a **TelecomX**, com foco na identificação de padrões associados ao **cancelamento de serviço (churn)**.

O trabalho foi desenvolvido como parte de um desafio prático e pode ser utilizado como base para estudos, projetos acadêmicos ou avaliação de perfil analítico em processos seletivos.

---

## 🧠 Objetivos

- Entender os fatores que levam os clientes a cancelarem seus serviços.
- Identificar padrões e perfis de clientes mais propensos à evasão.
- Preparar os dados para futuras aplicações de modelos preditivos.
- Gerar recomendações com base nos insights encontrados.

---

## 🗂 Estrutura do Projeto

O projeto está organizado da seguinte forma:

```
├── TelecomX_Data.json            # Base de dados original (formato JSON)
├── TelecomX_Analise.ipynb        # Notebook com toda a análise realizada
├── README.md                     # Este arquivo
```

---

## 📦 Tecnologias e Bibliotecas Utilizadas

- Python 3.11+
- [Pandas](https://pandas.pydata.org/)
- [NumPy](https://numpy.org/)
- [Matplotlib](https://matplotlib.org/)
- [Seaborn](https://seaborn.pydata.org/)
- Google Colab (ambiente de desenvolvimento)

---

## 📝 Etapas Realizadas

### 🔹 1. Importação e Exploração Inicial
- Carregamento do arquivo JSON.
- Visualização das primeiras linhas e estrutura dos dados.
- Verificação de tipos e valores únicos por coluna.

### 🔹 2. Limpeza e Tratamento de Dados
- Conversão de valores categóricos para binários (Yes/No → 1/0).
- Remoção de valores inconsistentes (`Unknown`, nulos e duplicados).
- Criação da coluna `valor_diario`, com base no valor mensal dividido por 30.
- Renomeação e padronização de colunas para o idioma português.

### 🔹 3. Análise Exploratória
- Proporção geral de evasão (`cancelou`).
- Análise por variáveis **categóricas**: gênero, tipo de contrato, forma de pagamento, fatura digital.
- Análise por variáveis **numéricas**: tempo como cliente, mensalidade, total gasto, valor diário.
- Visualizações com **boxplots**, **gráficos de pizza** e **histogramas empilhados**.

### 🔹 4. Análise de Correlação
- Cálculo da matriz de correlação entre variáveis numéricas.
- Destaque das variáveis mais relacionadas ao cancelamento.
- Estudo da relação entre `valor_diario`, `quantidade de serviços contratados` e churn.

---

## 🔍 Principais Insights

- Clientes com **contrato mensal** apresentam muito mais evasão que os com contratos anuais ou bienais.
- O churn é mais comum entre clientes com **pouco tempo de relacionamento**.
- **Fatura digital** e **pagamento por boleto** estão associados a maior probabilidade de evasão.
- Clientes que contratam **menos serviços** ou têm **valor diário mais alto** tendem a cancelar mais.

---

## 💡 Recomendações Estratégicas

1. Oferecer **descontos ou benefícios** em contratos de longo prazo.
2. Criar campanhas de retenção focadas nos **primeiros meses do cliente**.
3. Incentivar **pagamentos automáticos** (cartão ou débito).
4. Desenvolver **pacotes de serviços mais completos e vantajosos**.
5. Monitorar **clientes com alto valor diário e baixa fidelização**.

---

## ▶️ Como Executar

1. Acesse o notebook [`TelecomX_Analise.ipynb`](TelecomX_Analise.ipynb) via Google Colab.
2. Faça upload do arquivo `TelecomX_Data.json` na raiz do ambiente.
3. Execute as células em sequência para ver a análise completa.
4. Personalize ou expanda a análise conforme necessário.

---

## ⚠️ Possíveis Problemas

- Certifique-se de que todas as bibliotecas estão instaladas se for executar localmente (`pip install pandas numpy matplotlib seaborn`).
- O arquivo JSON deve estar no mesmo diretório do notebook ou corretamente referenciado.

---

## 📌 Próximos Passos (Sugerido)

- Criação de modelos preditivos com regressão logística, árvores de decisão, ou XGBoost.
- Uso de explicações interpretáveis com SHAP.
- Implementação de dashboards interativos com Streamlit.

---

## 🙋‍♂️ Autor

**Rafael Schmidt Sampaio**  
📧 Contato: rafaelssampaio@msn.com  
🔗 [Adicione seu LinkedIn ou GitHub aqui]

---

## 🧾 Licença

Este projeto é de uso livre para fins educacionais e demonstrativos.
