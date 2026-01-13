# Automação de Cadastro de Produtos

Este projeto é um script em Python que automatiza o cadastro de produtos em um sistema web, utilizando um arquivo CSV como base de dados. Ele abre o navegador, acessa o sistema, faz login automaticamente e preenche o formulário de produtos linha a linha.

## Tecnologias utilizadas

- Python 3
- [PyAutoGUI](https://pyautogui.readthedocs.io/en/latest/)
- [Pandas](https://pandas.pydata.org/)
- Arquivo CSV para base de dados

## Funcionalidades

- Abre o navegador automaticamente.
- Acessa a URL do sistema de cadastro.
- Realiza login com e-mail e senha configurados no código.
- Lê os dados de produtos a partir de um arquivo `produtos.csv`.
- Preenche automaticamente os campos do formulário (código, marca, tipo, categoria, preço unitário, custo e observações).
- Cadastra todos os produtos da base de dados de forma sequencial.

## Pré-requisitos

- Python 3 instalado.
- Bibliotecas instaladas:
  ```bash
  pip install pyautogui pandas
****

## Script de apoio: posicao_mouse.py

Este projeto também inclui o script `posicao_mouse.py`, usado para descobrir as coordenadas exatas do mouse na tela antes de configurar os cliques do PyAutoGUI.

O funcionamento é simples:
- Ao executar `posicao_mouse.py`, o script espera 5 segundos.
- Nesse tempo, você posiciona o cursor do mouse no lugar desejado na tela.
- Após os 5 segundos, ele imprime no terminal a posição atual do mouse (`x` e `y`), que você pode copiar e usar nos comandos `pyautogui.click(x=..., y=...)` do arquivo `automacao.py`.
