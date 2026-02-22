# 🟦 Level 00 → Level 01

<p align="center">
  <img src="https://img.shields.io/badge/Nível-00%20%E2%86%92%2001-1E90FF?style=for-the-badge&logo=linux&logoColor=white" />
</p>

---

## 📝 Resumo do desafio  
Neste nível, precisei aceder ao servidor remoto do **Bandit** via SSH utilizando as credenciais fornecidas.  
Depois de estabelecer a ligação, o objetivo foi localizar um ficheiro chamado **`readme`** no diretório inicial e extrair a informação necessária para avançar para o próximo nível.

---

## 🧠 Conceitos aprendidos  
Durante este nível, consolidei fundamentos essenciais para qualquer profissional de cibersegurança:

- 🔐 Funcionamento da autenticação SSH (utilizador + password)  
- 🧩 Estrutura correta de um comando SSH  
- 📂 Navegação básica no sistema de ficheiros Linux  
- 📄 Leitura de ficheiros simples no terminal  
- 🧍‍♂️ Importância de validar o utilizador ativo após a ligação  

---

## 🛠 Comandos relevantes  
Utilizei comandos fundamentais do ambiente Linux, reforçando a base necessária para níveis mais avançados:

- `ssh` → estabelecer ligação remota  
- `ls` → listar ficheiros  
- `cat` → visualizar conteúdo  
- `whoami` → confirmar o utilizador atual  

---

## 🚫 Erros comuns evitados  
Mantive atenção a pontos que normalmente causam dificuldades a iniciantes:

- ❌ Esquecer de colocar o utilizador correto antes do `@`  
- ❌ Tentar ligar na porta errada (o Bandit usa **2220**)  
- ❌ Procurar ficheiros sem verificar o diretório atual  

---

## 🔎 Raciocínio aplicado  
A minha abordagem foi objetiva e estruturada:

1. Analisei as instruções para identificar o utilizador e a porta correta.  
2. Estabeleci a ligação SSH e confirmei o utilizador ativo.  
3. Explorei o diretório inicial para localizar o ficheiro **`readme`**.  
4. Li o conteúdo do ficheiro e compreendi como utilizá-lo para aceder ao nível seguinte.  
5. Reforcei o padrão que será repetido em todos os níveis:  
   **encontrar a informação → interpretar → usar via SSH para avançar**.

---

<p align="center">
  <img src="https://img.shields.io/badge/Aprendizagem%20Consolidada-Linux%20%7C%20SSH%20%7C%20Navegação%20Básica-2E8B57?style=for-the-badge&logo=gnubash&logoColor=white" />
</p>
