<div align="center">
  <!-- Linha separadora superior -->
  <hr style="border:1px solid #55FF2E; width:40%; margin:auto 0 8px 0;">
  <!-- Badge principal -->
  <img src="https://img.shields.io/badge/Bandit-OverTheWire-55FF2E?style=for-the-badge&logo=linux&logoColor=white"
       style="height:35px; display:block; margin:auto;" />

  <br>

  <!-- Badge nível -->
  <img src="https://img.shields.io/badge/Nível-09%20%E2%86%92%2010-55FF2E?style=for-the-badge&logo=linux&logoColor=white"
       style="height:30px; display:block; margin:auto; margin-top:8px;" />

  <!-- Linha separadora inferior -->
  <hr style="border:1px solid #55FF2E; width:40%; margin:auto 0 8px 0;">

</div>


<!-- Resumo -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Summary.png"
width="70"
style="margin-right: 12px;">
Resumo do Desafio
</h1>

Neste nível, a password encontra-se dentro do ficheiro **`data.txt`**, mas o ficheiro **não contém apenas texto ASCII**.

Isso significa que ele inclui **dados binários**, dificultando a leitura direta.  
A password está localizada **numa das poucas sequências legíveis por humanos**, precedida por vários caracteres **`=`**.

Para resolver o desafio, foi necessário **extrair apenas as sequências de texto legíveis** do ficheiro.

---

<!-- Conceitos Aprendidos -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/concepts_learned.png"
width="70"
style="margin-right: 12px;">
Conceitos Aprendidos
</h1>

Neste desafio pratiquei conceitos importantes de **análise de ficheiros binários no Linux**:

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/file.png" width="18" style="margin-right:8px;">
Identificar ficheiros que contêm dados binários
</p>

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/search.png" width="18" style="margin-right:8px;">
Extrair sequências de texto legíveis com <code>strings</code>
</p>

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/search.png" width="18" style="margin-right:8px;">
Filtrar resultados com <code>grep</code>
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

- `file data.txt` → identificar o tipo de ficheiro  
- `strings data.txt` → extrair sequências de texto legíveis  
- `grep ===` → filtrar linhas que começam com vários caracteres `=`  
- `|` → combinar comandos no terminal  

---

<!-- Erros comuns -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/ErrorX.png"
width="70"
style="margin-right: 12px;">
Erros comuns evitados
</h1>

Alguns erros comuns neste nível incluem:

<p style="margin:0 0 14px 0; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png" width="18" style="margin-right:12px;">
Tentar abrir o ficheiro diretamente com <code>cat</code>
</p>

<p style="margin:0 0 14px 0; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png" width="18" style="margin-right:12px;">
Ignorar que o ficheiro contém dados binários
</p>

<p style="margin:0 0 14px 0; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png" width="18" style="margin-right:12px;">
Não utilizar filtros para reduzir os resultados
</p>

---

<!-- Raciocínio aplicado -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Thought_process.png"
width="70"
style="margin-right: 12px;">
Raciocínio aplicado
</h1>

A estratégia utilizada foi:

1. Identificar que o ficheiro contém **dados binários**.  
2. Utilizar `strings` para extrair apenas as sequências legíveis por humanos.  
3. Filtrar essas sequências com `grep` para encontrar as que começam com **`===`**.


---

<p align="center">
  <img src="https://img.shields.io/badge/Aprendizagem%20Consolidada-Strings%20%7C%20Grep%20%7C%20Análise%20de%20Binários-55FF2E?style=for-the-badge&logo=gnubash&logoColor=white" />
</p>

---
