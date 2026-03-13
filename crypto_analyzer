# importa a biblioteca yfinance que baixa dados financeiros da internet
import yfinance as yf

# importa a biblioteca responsável por criar gráficos
import matplotlib.pyplot as plt


# perguntaa para o usuário digitar qual criptomoeda quer analisar
# exemplo: BTC, ETH, SOL
crypto = input("Digite o símbolo da criptomoeda que você deseja analisar: (ex: BTC, ETH, SOL): ")

# cria o ticker no formato usado pelo Yahoo Finance
# exemplo: BTC-USD
ticker = crypto.upper() + "-USD"


# baixa os dados da criptomoeda a partir de 2023
data = yf.download(ticker, start="2023-01-01")


# define o tamanho da janela do gráfico
plt.figure(figsize=(10,5))


# cria o grafico usando o preço de fechamento (Close)
plt.plot(data["Close"])


# título do gráfico
plt.title(f"{crypto.upper()} Price")


# nome do eixo horizontal
plt.xlabel("Date")


# nome do eixo vertical
plt.ylabel("Price (USD)")


# gira as datas para ficarem legíveis
plt.xticks(rotation=45)


# ajusta o layout para evitar sobreposição
plt.tight_layout()


# mostra o grafico na tela
plt.show()
