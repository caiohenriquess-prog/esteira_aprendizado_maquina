# Esteira de Aprendizado de Máquina - Base Plants (UCI)

Trabalho da disciplina de Inteligência Artificial (Fatec - Análise e Desenvolvimento de Sistemas).

## Descrição do projeto

Esteira de aprendizado de máquina em um notebook Python (`esteira_ml_plants.ipynb`) usando a base **Plants** do UCI Machine Learning Repository (https://archive.ics.uci.edu/dataset/180/plants).

A base lista espécies de plantas e os estados dos EUA/províncias do Canadá onde elas ocorrem. O problema de classificação definido foi:

> Dada a lista de estados dos EUA onde uma espécie ocorre, prever se ela **também ocorre no Canadá**.

Etapas do notebook: download da base, estatísticas descritivas, transformações em linhas e colunas, divisão em treino/validação/teste (70/15/15), treinamento de um Random Forest, avaliação com acurácia e matriz de confusão, e predição de exemplo.

## Como reproduzir a execução

1. Acesse https://colab.research.google.com e entre com sua conta Google.
2. Vá em **Arquivo > Fazer upload de notebook** e envie o arquivo `esteira_ml_plants.ipynb` (ou, em **GitHub**, cole o link deste repositório e escolha o notebook).
3. Vá em **Ambiente de execução > Executar tudo**.
4. O próprio notebook baixa a base da UCI (pasta `dados/`). Não é preciso instalar nada, pois o Colab já tem pandas, scikit-learn e matplotlib.
5. Ao final, veja a acurácia, a matriz de confusão e as predições de exemplo.

Se o download automático falhar, baixe o zip em https://archive.ics.uci.edu/static/public/180/plants.zip, extraia e envie os arquivos `plants.data` e `stateabbr.txt` para uma pasta chamada `dados` no Colab.

## Execução local (opcional)

```bash
pip install pandas scikit-learn matplotlib jupyter
jupyter notebook esteira_ml_plants.ipynb
```
