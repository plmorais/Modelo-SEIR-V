# Modelo SEIR-V para Dengue com Sazonalidade Vetorial

Este projeto implementa um modelo compartimental SEIR-V (Suscetíveis–Expostos–Infectados–Recuperados com vetor) para simulação da transmissão da dengue em áreas urbanas, incorporando sazonalidade na população de mosquitos Aedes aegypti em função de variáveis climáticas (temperatura, precipitação e umidade relativa).

O código foi desenvolvido em Python e permite avaliar a dinâmica da doença e a sensibilidade do número básico de reprodução (R₀) a diferentes estratégias de controle, como redução da densidade vetorial ou alteração do período de incubação.

# Contexto
Modelos compartimentais vêm sendo amplamente utilizados para estudar a disseminação da dengue. O modelo SIR (Suscetível–Infectado–Recuperado) é uma abordagem simplificada, mas não considera o período de incubação nem a população vetorial. O SEIR-V estende essa formulação ao incluir:

* Compartimentos Expostos (humanos e vetores).

* Dinâmica acoplada humano–mosquito–humano.

* Efeitos sazonais sobre o tamanho e a taxa de reprodução da população vetorial.

Essa abordagem proporciona uma descrição mais realista do ciclo de transmissão e melhora o potencial preditivo para apoio a políticas públicas de saúde.

# Instalação
Clone este repositório e instale as dependências:

git clone https://github.com/usuario/seirv-dengue.git

cd seirv-dengue

pip install -r requirements.txt


# Para executar a simulação:

python scripts/seirv_model.py

Os parâmetros do modelo podem ser ajustados diretamente no arquivo seirv_model.py ou carregados de um arquivo de configuração .json.

Também a uma versão .ipynb para ser executado no colab.google.com

# Saída

* Gráficos da evolução de cada compartimento.

* Variação sazonal da população de mosquitos.

* Cálculo do número básico de reprodução (R₀).
