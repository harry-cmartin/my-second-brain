# **Versionamento de Código com Git**

## **O que é o Git?**

O Git é um sistema de controle de versão distribuído, criado por Linus Torvalds em 2005, para ajudar a gerenciar o desenvolvimento do kernel do Linux. Ele permite que os desenvolvedores acompanhem as mudanças no código-fonte ao longo do tempo, facilitando a colaboração e o gerenciamento de projetos de software.

- Para que serve: Ele monitora cada linha de código que você adiciona, altera ou apaga no seu projeto. Se você tentar implementar uma nova funcionalidade no backend e o servidor parar de rodar, o Git permite que você desfaça essas alterações e volte exatamente para a versão estável de minutos, dias ou meses atrás. Tudo isso de forma elegante, abolindo de vez a criação de pastas como projeto_final, projeto_final_agora_vai e projeto_final_v3

## **O que é o GitHub?**

O GitHub é uma plataforma de hospedagem em nuvem (um site) voltada para projetos que utilizam o Git.

- Para que serve: Enquanto o Git vive isolado na sua máquina, o GitHub é o lugar onde você guarda uma cópia segura do seu repositório na internet. Ele funciona como uma rede social para desenvolvedores e é a principal ferramenta de colaboração do mercado. Através dele, várias pessoas podem trabalhar no mesmo código simultaneamente sem que um apague o trabalho do outro. Além disso, serve como um portfólio vital para o mercado de trabalho.

## **Comandos essenciais do Git**

<center>

 
<div>
    <h1>Configuração inicial</h1> 
</div>


<table>
  <thead>
    <tr>
      <th align="left">Comando Git</th>
      <th align="left">O que ele faz na prática</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>git config --global user.name "Ada"</code></td>
      <td>Define o nome dos seus commits</td>
    </tr>
    <tr>
      <td><code>git config --global user.email you@x.com</code></td>
      <td>Define o e-mail dos seus commits</td>
    </tr>
    <tr>
      <td><code>git config --list</code></td>
      <td>Mostra toda a configuração atual</td>
    </tr>
    <tr>
      <td><code>git config --global init.defaultBranch main</code></td>
      <td>Nomeia a primeira branch de novos repositórios como main</td>
    </tr>
    <tr>
      <td><code>git config --global core.editor "code --wait"</code></td>
      <td>Define seu editor padrão</td>
    </tr>
    <tr>
      <td><code>git --version</code></td>
      <td>Exibe a versão do Git instalada</td>
    </tr>
  </tbody>
</table>

<div>
    <h1>Inicie um novo repositório ou copie um existente.</h1> 
</div>



<table>
  <thead>
    <tr>
      <th align="left">Comando Git</th>
      <th align="left">O que ele faz na prática</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>git init</code></td>
      <td>Cria um novo repositório na pasta atual</td>
    </tr>
    <tr>
      <td><code>git clone &lt;url&gt;</code></td>
      <td>Copia um repositório remoto localmente</td>
    </tr>
    <tr>
      <td><code>git clone &lt;url&gt; mydir</code></td>
      <td>Clona em uma pasta com nome definido</td>
    </tr>
    <tr>
      <td><code>git clone --depth 1 &lt;url&gt;</code></td>
      <td>Clone raso (apenas o commit mais recente)</td>
    </tr>
    <tr>
      <td><code>git clone -b dev &lt;url&gt;</code></td>
      <td>Clona e faz checkout da branch dev</td>
    </tr>
  </tbody>
</table>


<div>
    <h1>Preparar e commitar</h1> 
</div>

<table>
  <thead>
    <tr>
      <th align="left">Comando Git</th>
      <th align="left">O que ele faz na prática</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>git add file.txt</code></td>
      <td>Prepara um arquivo</td>
    </tr>
    <tr>
      <td><code>git add .</code></td>
      <td>Prepara todas as alterações no diretório atual</td>
    </tr>
    <tr>
      <td><code>git add -p</code></td>
      <td>Prepara trechos selecionados de forma interativa</td>
    </tr>
    <tr>
      <td><code>git commit -m "message"</code></td>
      <td>Commita as alterações preparadas</td>
    </tr>
    <tr>
      <td><code>git commit -am "message"</code></td>
      <td>Prepara arquivos rastreados e commita</td>
    </tr>
    <tr>
      <td><code>git commit --amend</code></td>
      <td>Edita o último commit</td>
    </tr>
    <tr>
      <td><code>git rm file.txt</code></td>
      <td>Remove um arquivo e prepara a exclusão</td>
    </tr>
  </tbody>
</table>



<div>
    <h1>Branches</h1> 
</div>

<table>
  <thead>
    <tr>
      <th align="left">Comando Git</th>
      <th align="left">O que ele faz na prática</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>git branch</code></td>
      <td>Lista as branches locais</td>
    </tr>
    <tr>
      <td><code>git branch feature</code></td>
      <td>Cria uma nova branch</td>
    </tr>
    <tr>
      <td><code>git switch feature</code></td>
      <td>Muda para uma branch existente</td>
    </tr>
    <tr>
      <td><code>git switch -c feature</code></td>
      <td>Cria e muda em um único passo</td>
    </tr>
    <tr>
      <td><code>git checkout feature</code></td>
      <td>Forma antiga de trocar de branch</td>
    </tr>
    <tr>
      <td><code>git branch -d feature</code></td>
      <td>Exclui uma branch já mesclada</td>
    </tr>
    <tr>
      <td><code>git branch -m newname</code></td>
      <td>Renomeia a branch atual</td>
    </tr>
  </tbody>
</table>





<div>
    <h1>Merge e rebase</h1> 
</div>

<table>

  <thead>
    <tr>
      <th align="left">Comando Git</th>
      <th align="left">O que ele faz na prática</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>git merge feature</code></td>
      <td>Mescla feature na branch atual</td>
    </tr>
    <tr>
      <td><code>git merge --no-ff feature</code></td>
      <td>Sempre cria um commit de merge</td>
    </tr>
    <tr>
      <td><code>git rebase main</code></td>
      <td>Reaplica seus commits sobre a main</td>
    </tr>
    <tr>
      <td><code>git rebase -i HEAD~3</code></td>
      <td>Edita os últimos 3 commits de forma interativa</td>
    </tr>
    <tr>
      <td><code>git rebase --continue</code></td>
      <td>Continua após resolver conflitos</td>
    </tr>
    <tr>
      <td><code>git rebase --abort</code></td>
      <td>Cancela um rebase em andamento</td>
    </tr>
    <tr>
      <td><code>git cherry-pick &lt;hash&gt;</code></td>
      <td>Aplica um commit nesta branch</td>
    </tr>
  </tbody>
</table>




<div>
    <h1>Remotos (push, pull, fetch)</h1> 
</div>

<table>
  <thead>
    <tr>
      <th align="left">Comando Git</th>
      <th align="left">O que ele faz na prática</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>git remote -v</code></td>
      <td>Lista os remotos configurados</td>
    </tr>
    <tr>
      <td><code>git remote add origin &lt;url&gt;</code></td>
      <td>Vincula um remoto chamado origin</td>
    </tr>
    <tr>
      <td><code>git fetch</code></td>
      <td>Baixa alterações remotas sem mesclar</td>
    </tr>
    <tr>
      <td><code>git pull</code></td>
      <td>Baixa e mescla a branch remota</td>
    </tr>
    <tr>
      <td><code>git push</code></td>
      <td>Envia commits para o remoto</td>
    </tr>
    <tr>
      <td><code>git push -u origin main</code></td>
      <td>Faz push e define a branch upstream</td>
    </tr>
    <tr>
      <td><code>git push origin --delete feature</code></td>
      <td>Exclui uma branch remota</td>
    </tr>
  </tbody>
</table>




<div>
    <h1>Inspecionar (status, log, diff)</h1> 
</div>


<table>
  <thead>
    <tr>
      <th align="left">Comando Git</th>
      <th align="left">O que ele faz na prática</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>git status</code></td>
      <td>Mostra arquivos preparados, não preparados e não rastreados</td>
    </tr>
    <tr>
      <td><code>git log</code></td>
      <td>Mostra o histórico de commits</td>
    </tr>
    <tr>
      <td><code>git log --oneline --graph</code></td>
      <td>Histórico compacto com um gráfico de branches</td>
    </tr>
    <tr>
      <td><code>git diff</code></td>
      <td>Alterações não preparadas vs o index</td>
    </tr>
    <tr>
      <td><code>git diff --staged</code></td>
      <td>Alterações preparadas vs o último commit</td>
    </tr>
    <tr>
      <td><code>git show &lt;hash&gt;</code></td>
      <td>Mostra as alterações de um único commit</td>
    </tr>
    <tr>
      <td><code>git blame file.txt</code></td>
      <td>Mostra quem alterou cada linha por último</td>
    </tr>
  </tbody>
</table>



<div>
    <h1>Desfazer alterações</h1> 
</div>


<table>
  <thead>
    <tr>
      <th align="left">Comando Git</th>
      <th align="left">O que ele faz na prática</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>git restore file.txt</code></td>
      <td>Descarta alterações não preparadas de um arquivo</td>
    </tr>
    <tr>
      <td><code>git restore --staged file.txt</code></td>
      <td>Remove um arquivo da área de preparo (mantém as alterações)</td>
    </tr>
    <tr>
      <td><code>git reset --soft HEAD~1</code></td>
      <td>Desfaz o último commit, mantendo as alterações preparadas</td>
    </tr>
    <tr>
      <td><code>git reset --hard HEAD~1</code></td>
      <td>Desfaz o último commit e descarta as alterações</td>
    </tr>
    <tr>
      <td><code>git revert &lt;hash&gt;</code></td>
      <td>Cria um novo commit que desfaz outro</td>
    </tr>
    <tr>
      <td><code>git stash</code></td>
      <td>Guarda alterações para depois</td>
    </tr>
    <tr>
      <td><code>git stash pop</code></td>
      <td>Reaplica o stash mais recente</td>
    </tr>
  </tbody>
</table>

</center>

#### Bibliografia 

>  


#### Histórico de Versões



| Versão |    Data    | Descrição                                 | Autor(es)                                       | Revisor(es)                                    |
| ------ | :--------: | ----------------------------------------- | ----------------------------------------------- | ---------------------------------------------- |
| 1.0    | 30/05/2026 | Criação do documento                        | [Harryson](https://github.com/harry-cmartin) |       |
