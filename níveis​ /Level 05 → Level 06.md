# 🟪 Level 05 → Level 06

<p align="center">
  <img src="https://img.shields.io/badge/Nível-05%20%E2%86%92%2006-8A2BE2?style=for-the-badge&logo=linux&logoColor=white" />
</p>

---

## 📝 Resumo do desafio  
Neste nível, precisei localizar um ficheiro específico dentro do diretório `inhere`.  
O objetivo era encontrar um ficheiro **legível por humanos**, com **1033 bytes** e **não executável**, e depois ler o seu conteúdo para avançar para o próximo nível.

---

## 🧠 Conceitos aprendidos  
Aprofundei competências importantes sobre pesquisa avançada de ficheiros:

- 🔍 Como filtrar ficheiros com propriedades específicas usando `find`  
- 📏 Como identificar ficheiros pelo tamanho exato em bytes  
- 🧪 Diferença entre ficheiros legíveis e binários  
- 🚫 Como excluir ficheiros executáveis durante a pesquisa  

---

## 🛠 Comandos relevantes  
Utilizei comandos essenciais para localizar o ficheiro correto:

- `find -type f -readable ! -executable -size 1033c` → localizar ficheiro com todas as propriedades  
- `find -size 1033c` → alternativa rápida baseada apenas no tamanho  
- `cd inhere` → aceder ao diretório  
- `cat maybehere07/.file2` → ler o ficheiro encontrado  

---

## 🚫 Erros comuns evitados  
Mantive atenção para não cometer erros típicos deste nível:

- ❌ Esquecer de especificar unidades (`c` para bytes)  
- ❌ Procurar apenas por nome e ignorar propriedades  
- ❌ Tentar abrir ficheiros binários  
- ❌ Não excluir ficheiros executáveis na pesquisa  

---

## 🔎 Raciocínio aplicado  
A minha abordagem foi clara e eficiente:

1. Acedi ao diretório `inhere`.  
2. Usei `find` para filtrar ficheiros com as propriedades exigidas.  
3. Identifiquei o ficheiro correto: **`maybehere07/.file2`**.  
4. Li o conteúdo com `cat` para obter a password.  
5. Utilizei a informação para aceder ao próximo nível via SSH.

---

<p align="center">
  <img src="https://img.shields.io/badge/Aprendizagem%20Consolidada-Find%20%7C%20Filtros%20Avançados-8A2BE2?style=for-the-badge&logo=gnubash&logoColor=white" />
</p>
