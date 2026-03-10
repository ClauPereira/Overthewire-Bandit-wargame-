<div align="center">

  <!-- Linha separadora superior -->
  <hr style="border:1px solid #C4FF2E; width:40%; margin:auto 0 8px 0;">
  <!-- Badge principal -->
  <img src="https://img.shields.io/badge/Bandit-OverTheWire-C4FF2E?style=for-the-badge&logo=linux&logoColor=white"
       style="height:35px; display:block; margin:auto;" />
  <br>

  <!-- Badge nível -->
  <img src="https://img.shields.io/badge/Nível-06%20%E2%86%92%2007-C4FF2E?style=for-the-badge&logo=linux&logoColor=white"
       style="height:30px; display:block; margin:auto; margin-top:8px;" />

  <!-- Linha separadora inferior -->
  <hr style="border:1px solid #C4FF2E; width:40%; margin:auto 0 8px 0;">

</div>


<!-- Resumo -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Summary.png"
       width="70"
       style="margin-right: 12px;">
Resumo do Desafio
</h1>

Neste nível, a password para avançar encontra-se **em algum lugar no servidor**.  
O ficheiro correto precisava cumprir **três propriedades específicas**:

- Pertencer ao **utilizador `bandit7`**
- Pertencer ao **grupo `bandit6`**
- Ter **33 bytes de tamanho**

Como o ficheiro poderia estar em qualquer lugar do sistema, foi necessário pesquisar **a partir do diretório raiz (`/`)** usando o comando `find`.

---

<!-- Conceitos Aprendidos -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/concepts_learned.png"
       width="70"
       style="margin-right: 12px;">
Conceitos Aprendidos
</h1>

Durante este desafio pratiquei conceitos importantes de **pesquisa avançada no Linux**:

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/search.png" width="18" style="margin-right:8px;">
Pesquisar ficheiros em todo o sistema com `find`
</p>

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/user.png" width="18" style="margin-right:8px;">
Filtrar ficheiros pelo **utilizador proprietário**
</p>

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/file.png" width="18" style="margin-right:8px;">
Filtrar ficheiros pelo **grupo**
</p>

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/size.png" width="18" style="margin-right:8px;">
Localizar ficheiros pelo **tamanho exato em bytes**
</p>

---

<!-- Comandos -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/commands.png"
       width="70"
       style="margin-right: 12px;">
Comandos Relevantes
</h1>

Os comandos principais utilizados neste nível foram:

- `cd /` → navegar até ao diretório raiz  
- `pwd` → confirmar a localização atual  
- `find -user bandit7 -group bandit6 -size 33c` → procurar ficheiros com todas as propriedades  
- `cat /var/lib/dpkg/info/bandit7.password` → ler o ficheiro encontrado  

---

<!-- Erros comuns -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/ErrorX.png"
       width="70"
       style="margin-right: 12px;">
Erros comuns evitados
</h1>

Alguns erros comuns que poderiam dificultar a resolução:

<p style="margin:0 0 14px 0; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png" width="18" style="margin-right:12px;">
Não executar a pesquisa a partir da raiz (`/`)
</p>

<p style="margin:0 0 14px 0; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png" width="18" style="margin-right:12px;">
Esquecer de usar a unidade `c` ao definir tamanho em bytes
</p>

<p style="margin:0 0 14px 0; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png" width="18" style="margin-right:12px;">
Confundir permissões negadas com ficheiros incorretos
</p>

---

<!-- Raciocínio -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Thought_process.png"
       width="70"
       style="margin-right: 12px;">
Raciocínio aplicado
</h1>

A estratégia utilizada foi a seguinte:

1. Naveguei até ao **diretório raiz** do sistema.  
2. Usei o comando `find` para pesquisar ficheiros que correspondam às **três propriedades exigidas**.  
3. A pesquisa retornou vários resultados, mas a maioria apresentou **"Permission denied"**.  
4. Apenas um ficheiro pôde ser acedido.<br><br>
   

<p align="center">
  <img src="https://img.shields.io/badge/Aprendizagem%20Consolidada-Find%20%7C%20User%20%7C%20Group%20%7C%20Size-C4FF2E?style=for-the-badge&logo=gnubash&logoColor=white" />
</p>
