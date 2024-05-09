# aula4-imersao-python-ia

# Recursos instalados

!pip install -q -U google-generativeai

# Importando o Python SDK

import google.generativeai as genai
from datetime import datetime, date
from google.colab import userdata

# Configurando o generation

generation_config = {
    "candidate_count": 1,
    "temperature": 0.5,
}

# Setando dados de segurança

safety_settings = {
    "HARASSMENT": "BLOCK_NONE",
    "HATE": "BLOCK_NONE",
    "SEXUAL": "BLOCK_NONE",
    "DANGEROUS": "BLOCK_NONE"
}

# Estilização

import textwrap
from IPython.display import display
from IPython.display import Markdown

# Objetivo de APP é realizar a análise via Google AI a partir dos resultados de exame laboratorial de bioquímica, o sistema coleta os dados
# Análisa os dados fornecidos e devolve os valores de referência e dá o laudo para cada resultado obtido
# No final ele faz um resumo total com base nos dados informados
