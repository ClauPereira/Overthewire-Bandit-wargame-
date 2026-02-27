# 🟦 Level 00 → Level 01

<p align="center">
  <img src="https://img.shields.io/badge/Nível-00%20%E2%86%92%2001-1E90FF?style=for-the-badge&logo=linux&logoColor=white" />
</p>

---
<!-- Resumo -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Summary.png"
       width="70"
       style="margin-right: 12px;">
  Resumo do Desafio
</h1>

Neste nível, precisei aceder ao servidor remoto do **Bandit** via SSH utilizando as credenciais fornecidas.  
Depois de estabelecer a ligação, o objetivo foi localizar um ficheiro chamado **`readme`** no diretório inicial e extrair a informação necessária para avançar para o próximo nível.

---
<!-- Conceitos Aprendidos-->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/concepts_learned.png"
       width="70"
       style="margin-right: 12px;">
Conceitos Aprendidos
</h1>

Durante este nível, consolidei fundamentos essenciais para qualquer profissional de cibersegurança:

<p style="margin: 0; line-height: 1.2; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/security.png"
       width="18"
       style="margin-right: 8px;">
  Funcionamento da autenticação SSH (utilizador + password)
</p>

<p style="margin: 0; line-height: 1.2; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/structure.png"
       width="18"
       style="margin-right: 8px;">
  Estrutura correta de um comando SSH
</p>

<p style="margin: 0; line-height: 1.2; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/file.png"
       width="18"
       style="margin-right: 8px;">
  Navegação básica no sistema de ficheiros Linux
</p>

<p style="margin: 0; line-height: 1.2; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/reading.png"
       width="18"
       style="margin-right: 8px;">
  Leitura de ficheiros simples no terminal
</p>

<p style="margin: 0; line-height: 1.2; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/user.png"
       width="12"
       style="margin-right: 8px;">
  Importância de validar o utilizador ativo após a ligação
</p>

---
<!-- Comandos-->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/commands.png"
       width="70"
       style="margin-right: 12px;">
Comandos Relevantes
</h1>

Utilizei comandos fundamentais do ambiente Linux, reforçando a base necessária para níveis mais avançados:

- `ssh` → estabelecer ligação remota  
- `ls` → listar ficheiros  
- `cat` → visualizar conteúdo  
- `whoami` → confirmar o utilizador atual  

---

<!-- Erros comuns evitados-->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/ErrorX.png"
       width="70"
       style="margin-right: 12px;">
Erros comuns evitados
</h1>

Mantive atenção a pontos que normalmente causam dificuldades a iniciantes:

<!-- erros-->
<p style="margin: 0 0 14px 0; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
Esquecer de colocar o utilizador correto antes do @
</p>
<p style="margin: 0 0 14px 0; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
Tentar ligar na porta errada (o Bandit usa 2220)
</p>
<p style="margin: 0 0 14px 0; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
Procurar ficheiros sem verificar o diretório atual
</p>

---
<!-- Raciocínio aplicado -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Thought_process.png"
       width="70"

## Raciocínio aplicado  
A minha abordagem foi objetiva e estruturada:

1. Analisei as instruções para identificar o utilizador e a porta correta.  
2. Estabeleci a ligação SSH e confirmei o utilizador ativo.  
3. Explorei o diretório inicial para localizar o ficheiro **`readme`**.  
4. Li o conteúdo do ficheiro e compreendi como utilizá-lo para aceder ao nível seguinte.  
5. Reforcei o padrão que será repetido em todos os níveis:  
   **encontrar a informação → interpretar → usar via SSH para avançar**.

---

<p align="center">
  <img src="https://img.shields.io/badge/Aprendizagem%20Consolidada-Linux%20%7C%20SSH%20%7C%20Navegação%20Básica-1E90FF?style=for-the-badge&logo=gnubash&logoColor=white" />
</p>









