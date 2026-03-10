<div align="center">

  <!-- Linha separadora superior, centralizada -->
  <hr style="border:1px solid #2EFF8F; width:40%; margin:auto 0 8px 0;">

  <!-- Badge 1: Bandit OverTheWire -->
  <img src="https://img.shields.io/badge/Bandit-OverTheWire-2EFF8F?style=for-the-badge&logo=linux&logoColor=white" style="height:35px; display:block; margin:auto;" />

  <br>

  <!-- Badge nível -->
  <img src="https://img.shields.io/badge/Nível-12%20%E2%86%92%2013-2EFF8F?style=for-the-badge&logo=linux&logoColor=white" style="height:30px; display:block; margin:auto; margin-top:8px;" />

  <!-- Linha separadora inferior -->
  <hr style="border:1px solid #2EFF8F; width:40%; margin:auto 0 8px 0;">

</div>

<!-- Resumo -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Summary.png"
       width="70"
       style="margin-right: 12px;">
  Resumo do Desafio
</h1>

Neste nível, a password encontra-se armazenada no ficheiro **`data.txt`**, mas o conteúdo está num **dump hexadecimal de um ficheiro que foi comprimido várias vezes**.

Isso significa que primeiro foi necessário **converter o hexdump para um ficheiro binário**, e depois **descomprimir sucessivamente várias camadas de compressão** até encontrar o conteúdo final.

Para trabalhar com segurança, foi recomendado criar um diretório temporário dentro de **`/tmp`**.

---

<!-- Conceitos Aprendidos-->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/concepts_learned.png"
       width="70"
       style="margin-right: 12px;">
Conceitos Aprendidos
</h1>

Durante este desafio pratiquei conceitos importantes de **análise e extração de ficheiros no Linux**:

<p style="margin: 0; line-height: 1.2; font-size: 12px; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/file.png"
       width="18"
       style="margin-right: 8px;">
  Converter dumps hexadecimais para ficheiros binários com <code>xxd</code>
</p>

<p style="margin: 0; line-height: 1.2; font-size: 12px; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/structure.png"
       width="18"
       style="margin-right: 8px;">
  Identificar tipos de ficheiros com <code>file</code>
</p>

<p style="margin: 0; line-height: 1.2; font-size: 12px; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/file.png"
       width="18"
       style="margin-right: 8px;">
  Extrair ficheiros comprimidos com <code>gzip</code>, <code>bzip2</code> e <code>tar</code>
</p>

<p style="margin: 0; line-height: 1.2; font-size: 12px; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/structure.png"
       width="18"
       style="margin-right: 8px;">
  Criar diretórios temporários para análise segura
</p>

---

<!-- Comandos-->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/commands.png"
       width="70"
       style="margin-right: 12px;">
Comandos Relevantes
</h1>

Os comandos utilizados neste nível incluem:

- `mktemp -d` → criar diretório temporário seguro  
- `cp` → copiar ficheiros  
- `mv` → renomear ficheiros  
- `xxd -r` → converter hexdump para binário  
- `file` → identificar tipo de ficheiro  
- `gunzip` → descomprimir gzip  
- `bunzip2` → descomprimir bzip2  
- `tar -xf` → extrair arquivos tar  

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
  Tentar extrair diretamente o hexdump sem convertê-lo primeiro
</p>

<p style="margin: 0 0 14px 0; font-size: 12px; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
  Não verificar o tipo do ficheiro com <code>file</code>
</p>

<p style="margin: 0 0 14px 0; font-size: 12px; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
  Ignorar extensões corretas antes de descomprimir
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

1. Criar um diretório temporário em **`/tmp`** para trabalhar com segurança.  
2. Copiar o ficheiro **`data.txt`** para esse diretório.  
3. Converter o dump hexadecimal para binário usando: xxd -r data.txt > newdata.txt
4. Identificar o tipo de ficheiro usando `file`.  
5. Descomprimir sucessivamente várias camadas utilizando `gzip`, `bzip2` e `tar`.  
6. Repetir o processo até obter o ficheiro final contendo **texto ASCII** com a password.

---

<p align="center">
  <img src="https://img.shields.io/badge/Aprendizagem%20Consolidada-Hexdump%20%7C%20xxd%20%7C%20Compression%20Tools-2EFF8F?style=for-the-badge&logo=gnubash&logoColor=white" />
</p>
