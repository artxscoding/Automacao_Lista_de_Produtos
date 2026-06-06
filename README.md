# Automação de Cadastro de Produtos 🤖📦

Este projeto é uma automação desenvolvida em Python para cadastrar produtos em um sistema web de forma rápida e sem intervenção manual. O script foi construído passo a passo para abrir o navegador, fazer login no sistema corporativo, ler uma base de dados e registrar item por item.

Este projeto foi inspirado nas aulas do Intensivão de Python da Hashtag Treinamentos.

## ⚙️ Como funciona?

O script executa as seguintes etapas automaticamente:
1. Abre o navegador **Opera** usando atalhos do Windows.
2. Acessa a página de login do sistema.
3. Preenche os dados de e-mail e senha e faz o login.
4. Importa a base de dados de produtos a partir de um arquivo `produtos.csv`.
5. Entra em um loop (laço de repetição) preenchendo todos os campos necessários (código, marca, tipo, categoria, preço, custo e observações) para cada produto da tabela.
6. Envia o formulário e repete o processo até o fim da lista.

## 🚀 Tecnologias e Bibliotecas Utilizadas

* **Python**
* **PyAutoGUI**: Para automação de teclado e mouse (cliques, digitação e atalhos).
* **Pandas**: Para leitura e manipulação da base de dados (arquivo CSV).
* **Time**: Para adicionar pausas estratégicas e garantir que a página carregue antes do próximo comando.

## ⚠️ Aviso Importante: Resolução de Tela

O `PyAutoGUI` utiliza coordenadas fixas da tela para realizar os cliques (ex: `pyautogui.click(x=714, y=362)`). Isso significa que **o código precisará ser ajustado** caso o seu monitor tenha uma resolução diferente da que foi usada para criar o script.

> **Dica:** O projeto já inclui um pequeno trecho de código no final do arquivo principal para ajudar a descobrir as coordenadas exatas do seu mouse (`pyautogui.position()`). Use-o para mapear a sua própria tela se for necessário!

## 🛠️ Como executar na sua máquina

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/artxscoding/Automacao_Lista_de_Produtos.git](https://github.com/artxscoding/Automacao_Lista_de_Produtos.git)
   ```

2. **Instale as dependências:**
   Abra o terminal e instale as bibliotecas necessárias:
   ```bash
   pip install pyautogui pandas
   ```

3. **Prepare o ambiente:**
   * Certifique-se de ter o navegador **Opera** instalado (o código o procura pelo atalho do Windows).
   * Verifique se o arquivo `produtos.csv` está na mesma pasta do seu script Python.

4. **Inicie a automação:**
   Execute o script no seu terminal ou editor de código favorito:
   ```bash
   python automacao.py
   ```
   *Não mexa no mouse ou teclado enquanto a automação estiver rodando!*

## 👤 Desenvolvedor

Arthur - [artxscoding](https://github.com/artxscoding)
