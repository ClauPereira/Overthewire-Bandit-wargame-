<div align="center">
  <!-- Linha separadora superior, centralizada -->
  <hr style="border:1px solid #2EFF3A; width:40%; margin:auto 0 8px 0;">

  <!-- Badge 1: Bandit OverTheWire -->
  <img src="https://img.shields.io/badge/Bandit-OverTheWire-2EFF3A?style=for-the-badge&logo=linux&logoColor=white" style="height:35px; display:block; margin:auto;" />

  <br>

  <!-- Badge nível -->
  <img src="https://img.shields.io/badge/Nível-10%20%E2%86%92%2011-2EFF3A?style=for-the-badge&logo=linux&logoColor=white" style="height:30px; display:block; margin:auto; margin-top:8px;" />

  <!-- Linha separadora inferior -->
  <hr style="border:1px solid #2EFF3A; width:40%; margin:auto 0 8px 0;">

</div>

<!-- Resumo -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Summary.png"
       width="70"
       style="margin-right: 12px;">
  Resumo do Desafio
</h1>

Neste nível, a password encontra-se armazenada no ficheiro **`data.txt`**, porém o conteúdo está **codificado em Base64**.

Base64 é um método comum de **codificação de dados**, utilizado para representar dados binários em formato texto.  
Para obter a password, foi necessário **descodificar o conteúdo do ficheiro** utilizando uma ferramenta apropriada.

---

<!-- Conceitos Aprendidos-->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/concepts_learned.png"
       width="70"
       style="margin-right: 12px;">
Conceitos Aprendidos
</h1>

Durante este desafio aprofundei conhecimentos importantes sobre **codificação de dados em sistemas Linux**:

<p style="margin: 0; line-height: 1.2; font-size: 12px; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/file.png"
       width="18"
       style="margin-right: 8px;">
  Identificar ficheiros com dados codificados
</p>

<p style="margin: 0; line-height: 1.2; font-size: 12px; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/structure.png"
       width="18"
       style="margin-right: 8px;">
  Compreender o funcionamento da codificação **Base64**
</p>

<p style="margin: 0; line-height: 1.2; font-size: 12px; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/reading.png"
       width="18"
       style="margin-right: 8px;">
  Decodificar dados no terminal Linux
</p>

<p style="margin: 0; line-height: 1.2; font-size: 12px; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/security.png"
       width="18"
       style="margin-right: 8px;">
  Reconhecer formatos de dados frequentemente utilizados em CTFs
</p>

---

<!-- Comandos-->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/commands.png"
       width="70"
       style="margin-right: 12px;">
Comandos Relevantes
</h1>

Neste nível utilizei comandos relacionados com **decodificação de dados**:

- `base64 -d data.txt` → decodificar conteúdo em Base64  
- `cat data.txt` → visualizar o ficheiro (opcional)  
- `file data.txt` → verificar o tipo de dados  

---

<!-- Erros comuns evitados-->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/ErrorX.png"
       width="70"
       style="margin-right: 12px;">
Erros comuns evitados
</h1>

Alguns erros comuns que poderiam dificultar a resolução:

<p style="margin: 0 0 14px 0; font-size: 12px; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
  Tentar interpretar manualmente o texto codificado
</p>

<p style="margin: 0 0 14px 0; font-size: 12px; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
  Esquecer o argumento <code>-d</code> no comando base64
</p>

<p style="margin: 0 0 14px 0; font-size: 12px; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
  Assumir que o ficheiro contém texto simples
</p>

---

<!-- Raciocínio aplicado -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Thought_process.png"width="70"style="margin-right: 12px;">
Raciocínio aplicado
</h1>

A minha abordagem foi:

1. Identificar que o ficheiro continha **dados codificados em Base64**.  
2. Utilizar a ferramenta `base64` disponível no Linux para realizar a descodificação.  
3. Executar o comando com o argumento **`-d`** para converter os dados novamente para texto legível.  
4. Ler a password resultante para avançar para o próximo nível.

---
<p align="center">
  <img src="https://img.shields.io/badge/Aprendizagem%20Consolidada-Base64%20%7C%20Decodificação%20de%20Dados-2EFF3A?style=for-the-badge&logo=gnubash&logoColor=white" />
</p>
