<h2> GitHub Tutorial </h2> 

<h5>Introdução aos conceitos fundamentais do Git e GitHub.</h5>
<p>Git e Github são utilizados no dia a dia das pessoas que criam softwares por um motivo bem simples: ter uma forma fácil de gerenciar o código-fonte da aplicação, do sistema e do produto.
  
O Git é um sistema de controle de versão distribuído amplamente utilizado no desenvolvimento de software. Ele permite rastrear e gerenciar as alterações feitas nos arquivos ao longo do tempo, facilitando a colaboração entre desenvolvedores e ajudando a manter um histórico completo das modificações feitas em um projeto.

Basicamente, o Git funciona armazenando os arquivos do projeto em um repositório. Ele registra alterações nesses arquivos através de commits, que são snapshots (fotografias) do estado do projeto em determinado momento. Isso possibilita voltar a versões anteriores, criar e mesclar diferentes linhas de desenvolvimento (ramificações), e colaborar de maneira eficiente em equipes, minimizando conflitos.

</p>

<h5> Principais Comandos </h5>


<h6>Inicializar um Repositório Git</h6>

``` 
  git init
```

<h6>Configuração Inicial (Se ainda não configurou)</h6>

```
  git config --global user.name "SeuNome"
  git config --global user.email "seuemail@example.com"
```

<h6> Navegar até o Repositório </h6>

``` 
 cd caminho/para/o/seu/repositório
```

<h6> Adicionar Arquivos ao Stage </h6>

```
 git add nome_do_arquivo_ou_pasta
 git add .  ->  Adiciona todos os arquivos
```

<h6> Verificar Status do Git </h6>

```
 git status
```

<h6>Obtenha o URL do Repositório Remoto</h6>
<p>No GitHub, vá até o seu repositório e clique no botão "Code". Certifique-se de escolher a opção "HTTPS" ou "SSH" para obter o URL correto.</p>

<h6> Adicione o Repositório Remoto ao seu Repositório Local </h6>

```
 git remote add origin URL_do_seu_repositório_no_GitHub
```

<p>Por exemplo, se estiver utilizando HTTPS<p>

```
 git remote add origin https://github.com/seu_usuario/seu_repositorio.git
```

<h6> Verificar a Origem Adicionada </h6>

```
git remote -v
```

<h6> Criar o Commit </h6>

```
git commit -m "Mensagem descritiva do commit"
```


<h6> Puxar arquivos do repositório remmoto </h6>

```
git pull origin nome_da_branch
```

<h6> Enviar Commits para a Origem Remota </h6>

```
git push origin nome_da_branch
```









