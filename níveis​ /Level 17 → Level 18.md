<div align="center">

  <!-- Linha separadora superior -->
  <hr style="border:1px solid #2E9AFF; width:40%; margin:auto 0 8px 0;">
  <!-- Badge principal -->
  <img src="https://img.shields.io/badge/Bandit-OverTheWire-2E9AFF?style=for-the-badge&logo=linux&logoColor=white"
       style="height:35px; display:block; margin:auto;" />

  <br>

  <!-- Badge nível -->
  <img src="https://img.shields.io/badge/Nível-17%20%E2%86%92%2018-2E9AFF?style=for-the-badge&logo=linux&logoColor=white"
       style="height:30px; display:block; margin:auto; margin-top:8px;" />

  <!-- Linha separadora inferior -->
  <hr style="border:1px solid #2E9AFF; width:40%; margin:auto 0 8px 0;">

</div>


<!-- Resumo -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Summary.png"
width="70"
style="margin-right: 12px;">
Resumo do Desafio
</h1>

Neste nível existem **dois arquivos no diretório inicial**:

- `passwords.old`
- `passwords.new`

A senha para o próximo nível está em **`passwords.new`**, e é **a única linha que foi alterada** em relação ao arquivo `passwords.old`.

O objetivo foi **comparar os dois arquivos** para identificar exatamente qual linha mudou.

---

<!-- Conceitos Aprendidos -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/concepts_learned.png"
width="70"
style="margin-right: 12px;">
Conceitos Aprendidos
</h1>

Durante este desafio pratiquei conceitos importantes de **comparação de arquivos no Linux**:

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/structure.png" width="18" style="margin-right:8px;">
Como comparar arquivos utilizando o comando <code>diff</code>
</p>

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/search.png" width="18" style="margin-right:8px;">
Identificar diferenças entre versões de arquivos
</p>

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/slash.png" width="18" style="margin-right:8px;">
Compreender a saída do comando <code>diff</code>
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

- `ls` → listar os arquivos disponíveis no diretório  
- `cat` → visualizar o conteúdo dos arquivos  
- `diff passwords.old passwords.new` → comparar os dois arquivos  

---

<!-- Erros comuns -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/ErrorX.png"
width="70"
style="margin-right: 12px;">
Erros comuns evitados
</h1>

<p style="margin:0 0 14px 0; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png" width="18" style="margin-right:12px;">
Tentar analisar manualmente arquivos muito grandes
</p>

<p style="margin:0 0 14px 0; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png" width="18" style="margin-right:12px;">
Não perceber que apenas **uma linha foi alterada**
</p>

<p style="margin:0 0 14px 0; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png" width="18" style="margin-right:12px;">
Confundir a ordem dos arquivos no comando <code>diff</code>
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

1. Identificar os arquivos disponíveis com `ls`.  
2. Verificar que existem dois arquivos com versões diferentes de passwords.  
3. Utilizar `diff` para comparar os arquivos.  
4. Identificar a linha que aparece apenas em `passwords.new`.  
5. Essa linha corresponde à senha para o próximo nível.

Exemplo de comando utilizado:

```bash
diff passwords.old passwords.new
```
<p align="center"> <img src="https://img.shields.io/badge/Aprendizagem%20Consolidada-File%20Comparison%20%7C%20Diff%20%7C%20Linux%20CLI-2E9AFF?style=for-the-badge&logo=gnubash&logoColor=white" /> </p>


