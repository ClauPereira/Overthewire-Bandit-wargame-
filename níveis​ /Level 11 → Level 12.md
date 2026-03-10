<div align="center">

  <!-- Linha separadora superior, centralizada -->
  <hr style="border:1px solid #2EFF66; width:40%; margin:auto 0 8px 0;">

  <!-- Badge 1: Bandit OverTheWire -->
  <img src="https://img.shields.io/badge/Bandit-OverTheWire-2EFF66?style=for-the-badge&logo=linux&logoColor=white" style="height:35px; display:block; margin:auto;" />

  <br>

  <!-- Badge 2: Nível -->
  <img src="https://img.shields.io/badge/Nível-11%20%E2%86%92%2012-2EFF66?style=for-the-badge&logo=linux&logoColor=white" style="height:30px; display:block; margin:auto; margin-top:8px;" />

  <!-- Linha separadora inferior -->
  <hr style="border:1px solid #2EFF66; width:40%; margin:auto 0 8px 0;">

</div>

<!-- Resumo -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Summary.png"
       width="70"
       style="margin-right: 12px;">
  Resumo do Desafio
</h1>

Neste nível, a password encontra-se armazenada no ficheiro **`data.txt`**, mas o texto foi **transformado usando o algoritmo ROT13**.

O método ROT13 consiste em **rodar cada letra do alfabeto 13 posições**, transformando letras em outras letras.  
Por exemplo:

- **A → N**
- **B → O**
- **N → A**

Para descobrir a password, foi necessário **reverter essa transformação**.

---

<!-- Conceitos Aprendidos-->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/concepts_learned.png"
       width="70"
       style="margin-right: 12px;">
Conceitos Aprendidos
</h1>

Durante este desafio pratiquei conceitos importantes de **transformação de texto no terminal Linux**:

<p style="margin: 0; line-height: 1.2; font-size: 12px; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/structure.png"
       width="18"
       style="margin-right: 8px;">
  Funcionamento da cifra **ROT13**
</p>

<p style="margin: 0; line-height: 1.2; font-size: 12px; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/reading.png"
       width="18"
       style="margin-right: 8px;">
  Transformação de caracteres com o comando <code>tr</code>
</p>

<p style="margin: 0; line-height: 1.2; font-size: 12px; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/slash.png"
       width="18"
       style="margin-right: 8px;">
  Utilização de **pipes (`|`)** para encadear comandos
</p>

<p style="margin: 0; line-height: 1.2; font-size: 12px; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/security.png"
       width="18"
       style="margin-right: 8px;">
  Reconhecimento de métodos simples de cifragem em desafios CTF
</p>

---

<!-- Comandos-->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/commands.png"
       width="70"
       style="margin-right: 12px;">
Comandos Relevantes
</h1>

Os comandos utilizados neste nível foram:

- `cat data.txt` → visualizar o conteúdo do ficheiro  
- `tr` → transformar caracteres  
- `|` → redirecionar saída entre comandos  

---

<!-- Erros comuns evitados-->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/ErrorX.png"
       width="70"
       style="margin-right: 12px;">
Erros comuns evitados
</h1>

Alguns erros comuns neste nível incluem:

<p style="margin: 0 0 14px 0; font-size: 12px; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
  Tentar decifrar manualmente o texto ROT13
</p>

<p style="margin: 0 0 14px 0; font-size: 12px; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
  Utilizar parâmetros desnecessários no comando <code>tr</code>
</p>

<p style="margin: 0 0 14px 0; font-size: 12px; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
  Esquecer de utilizar pipe para combinar comandos
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

1. Identificar que o ficheiro utilizava **ROT13**.  
2. Utilizar o comando `tr` para rotacionar novamente as letras do alfabeto.  
3. Encadear os comandos com um **pipe** para processar o conteúdo diretamente.

---

<p align="center">
  <img src="https://img.shields.io/badge/Aprendizagem%20Consolidada-ROT13%20%7C%20tr%20%7C%20Transformação%20de%20Texto-2EFF66?style=for-the-badge&logo=gnubash&logoColor=white" />
</p>
