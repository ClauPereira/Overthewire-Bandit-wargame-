<div align="center">

  <!-- Linha separadora superior -->
  <hr style="border:1px solid #A0FF2E; width:40%; margin:auto 0 8px 0;">
  <!-- Badge principal -->
  <img src="https://img.shields.io/badge/Bandit-OverTheWire-A0FF2E?style=for-the-badge&logo=linux&logoColor=white"
       style="height:35px; display:block; margin:auto;" />

  <br>

  <!-- Badge nível -->
  <img src="https://img.shields.io/badge/Nível-07%20%E2%86%92%2008-A0FF2E?style=for-the-badge&logo=linux&logoColor=white"
       style="height:30px; display:block; margin:auto; margin-top:8px;" />

  <!-- Linha separadora inferior -->
  <hr style="border:1px solid #A0FF2E; width:40%; margin:auto 0 8px 0;">

</div>


<!-- Resumo -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Summary.png"
       width="70"
       style="margin-right: 12px;">
Resumo do Desafio
</h1>

Neste nível, a password encontra-se dentro do ficheiro **`data.txt`**.  
O objetivo era localizar **a linha que contém a palavra `millionth`** e obter a password que aparece ao lado dessa palavra.

Para resolver o desafio utilizei o comando **`grep`**, que permite pesquisar palavras específicas dentro de ficheiros.

---

<!-- Conceitos Aprendidos -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/concepts_learned.png"
       width="70"
       style="margin-right: 12px;">
Conceitos Aprendidos
</h1>

Durante este desafio pratiquei conceitos essenciais de **pesquisa de texto no Linux**:

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/search.png" width="18" style="margin-right:8px;">
Pesquisar palavras específicas dentro de ficheiros com <code>grep</code>
</p>

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/file.png" width="18" style="margin-right:8px;">
Analisar rapidamente ficheiros grandes
</p>

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/search.png" width="18" style="margin-right:8px;">
Extrair apenas a informação relevante de um ficheiro
</p>

---

<!-- Comandos -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/commands.png"
       width="70"
       style="margin-right: 12px;">
Comandos Relevantes
</h1>

Os comandos utilizados neste nível foram:

- `grep millionth data.txt` → procurar a palavra específica dentro do ficheiro  
- `cat data.txt` → visualizar todo o conteúdo do ficheiro (opcional)  
- `man grep` → consultar o manual do comando  

---

<!-- Erros comuns -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/ErrorX.png"
       width="70"
       style="margin-right: 12px;">
Erros comuns evitados
</h1>

Alguns erros que poderiam dificultar a resolução:

<p style="margin:0 0 14px 0; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png" width="18" style="margin-right:12px;">
Procurar manualmente dentro do ficheiro em vez de usar <code>grep</code>
</p>

<p style="margin:0 0 14px 0; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png" width="18" style="margin-right:12px;">
Escrever a palavra de pesquisa incorretamente
</p>

<p style="margin:0 0 14px 0; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png" width="18" style="margin-right:12px;">
Ignorar a utilização do manual (<code>man</code>)
</p>

---

<!-- Raciocínio aplicado -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Thought_process.png"
       width="70"
       style="margin-right: 12px;">
Raciocínio aplicado
</h1>

A estratégia utilizada foi simples e direta:

1. Identifiquei que a password estava **ao lado da palavra "millionth"**.  
2. Usei o comando `grep` para procurar essa palavra dentro do ficheiro `data.txt`.  
3. O terminal retornou a linha correta contendo a password.



---

<p align="center">
  <img src="https://img.shields.io/badge/Aprendizagem%20Consolidada-Grep%20%7C%20Pesquisa%20de%20Texto-A0FF2E?style=for-the-badge&logo=gnubash&logoColor=white" />

