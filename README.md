# Previsão da Umidade Relativa do Ar com Modelos Univariados: Uma Comparação entre BiLSTM e Híbrido Rolling VMD-BiLSTM

Este repositório contém os códigos-fonte utilizados para a modelagem preditiva e resultados apresentados no artigo científico **"Previsão da Umidade Relativa do Ar com Modelos Univariados: Uma Comparação entre BiLSTM e Híbrido Rolling VMD-BiLSTM"**, publicado na Revista Ibero-Americana de Humanidades, Ciências e Educação (REASE).

## 📄 Sobre a Pesquisa
O estudo avalia o desempenho da previsão univariada da umidade relativa do ar utilizando um modelo Deep Learning BiLSTM tradicional em contraposição a um modelo híbrido Rolling VMD-BiLSTM. A metodologia destaca a aplicação da Decomposição em Modos Variacionais com janela deslizante (Rolling VMD) processando a série temporal de forma iterativa para mitigar o vazamento de dados (*data leakage*), garantindo um cenário preditivo realista.

🔗 **Artigo Completo:** https://periodicorease.pro.br/rease/article/view/25722/16365
🔗 **DOI:** https://doi.org/10.51891/rease.v12i4.25722

## 💻 Códigos e Notebooks
Os modelos foram desenvolvidos em ambiente Google Colab. Você pode visualizar e executar os notebooks diretamente no seu navegador usando os botões abaixo:

1. **Modelo BiLSTM Padrão:** `BiLSTM_Forecasting_UR.ipynb`
   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1qEwIymA3deIYbVouwv6ilJE-hW1jO53U?usp=sharing)
   
2. **Modelo Híbrido Rolling VMD-BiLSTM:** `VMD_BiLSTM_UR.ipynb`
   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1uFosIDMPTvWpBLdxy__nuyFmUf9sBbhc?usp=sharing)

## 📊 Conjunto de Dados
A série temporal meteorológica (2007 a 2023) utilizada para o treinamento e validação dos modelos é importada diretamente nos notebooks por meio de um arquivo hospedado e aberto no [Google Sheets](https://docs.google.com/spreadsheets/d/1MRqHSHxVjynI_0OFkbT18MiPGZ6p0t7b/export?format=xlsx).

## 🛠️ Tecnologias Utilizadas
* Python 3
* TensorFlow / Keras (Suporte a *Mixed Precision* habilitado)
* scikit-learn
* vmdpy (Algoritmo de Decomposição em Modos Variacionais)
* joblib e tqdm (Otimização e paralelização do Rolling VMD)

## ✒️ Como Citar
Se você utilizar as metodologias ou os códigos disponibilizados neste repositório em sua pesquisa, por favor, cite nosso trabalho original:

```bibtex
@article{Souza_Nakajima_Oliveira_Thomaz_2026, 
  title={PREVISÃO DA UMIDADE RELATIVA DO AR COM MODELOS UNIVARIADOS: UMA COMPARAÇÃO ENTRE BILSTM E HÍBRIDO ROLLING VMD-BILSTM}, 
  author={Souza, Winicius dos Passos Soares de and Nakajima, Evandro Alves and Oliveira, Fabrício Correia de and Thomaz, Diego Venâncio},
  journal={Revista Ibero-Americana de Humanidades, Ciências e Educação},
  volume={12}, 
  number={4}, 
  pages={1--22},
  year={2026}, 
  month={abr.}, 
  url={https://periodicorease.pro.br/rease/article/view/25722}, 
  doi={10.51891/rease.v12i4.25722}
}
```
