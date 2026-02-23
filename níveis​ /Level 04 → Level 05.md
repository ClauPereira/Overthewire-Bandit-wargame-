# 🟥 Level 04 → Level 05

<p align="center">
  <img src="https://img.shields.io/badge/Nível-04%20%E2%86%92%2005-DC143C?style=for-the-badge&logo=linux&logoColor=white" />
</p>

---

## 📝 Resumo do desafio  
Neste nível, precisei encontrar um ficheiro específico dentro do diretório `inhere`.  
O objetivo era localizar o único ficheiro **legível por humanos**, com **1033 bytes** e **não executável**, e depois ler o seu conteúdo para avançar para o próximo nível.

---

## 🧠 Conceitos aprendidos  
Aprofundei conhecimentos importantes sobre análise de ficheiros em Linux:

- 🧪 Como identificar o tipo de um ficheiro com `file`  
- 📏 Como verificar o tamanho exato de um ficheiro  
- 🚫 Diferença entre ficheiros executáveis e não executáveis  
- 🔍 Como filtrar ficheiros com propriedades específicas  

---

## 🛠 Comandos relevantes  
Usei comandos essenciais para localizar o ficheiro correto:

- `ls` → listar ficheiros  
- `cd inhere` → aceder ao diretório  
- `file ./-file*` → identificar ficheiros legíveis por humanos  
- `du -b` → verificar tamanho em bytes  
- `cat -file07` → ler o conteúdo do ficheiro certo  

---

## 🚫 Erros comuns evitados  
Mantive atenção para não cometer erros típicos deste nível:

- ❌ Assumir que todos os ficheiros são legíveis  
- ❌ Ignorar o tamanho exato exigido (1033 bytes)  
- ❌ Tentar abrir ficheiros binários  
- ❌ Esquecer de usar `file` para confirmar o tipo de conteúdo  

---

## 🔎 Raciocínio aplicado  
A minha abordagem foi clara e direta:

1. Acedi ao diretório `inhere`.  
2. Listei os ficheiros e usei `file` para identificar qual era legível por humanos.  
3. Verifiquei o tamanho com `du -b` para confirmar os **1033 bytes**.  
4. Identifiquei o ficheiro correto: **`-file07`**.  
5. Li o conteúdo com `cat` e utilizei a password para avançar para o próximo nível.

---

<p align="center">
  <img src="https://img.shields.io/badge/Aprendizagem%20Consolidada-Análise%20de%20Ficheiros%20%7C%20file-DC143C?style=for-the-badge&logo=gnubash&logoColor=white" />
</p>
