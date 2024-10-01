<h2> Git Tutorial </h2> 

<h5>Introdução aos conceitos fundamentais do Git e GitHub.</h5>
<p>Git e Github são utilizados no dia a dia das pessoas que criam softwares por um motivo bem simples: ter uma forma fácil de gerenciar o código-fonte da aplicação, do sistema e do produto.
  
O Git é um sistema de controle de versão distribuído amplamente utilizado no desenvolvimento de software. Ele permite rastrear e gerenciar as alterações feitas nos arquivos ao longo do tempo, facilitando a colaboração entre desenvolvedores e ajudando a manter um histórico completo das modificações feitas em um projeto.

Basicamente, o Git funciona armazenando os arquivos do projeto em um repositório. Ele registra alterações nesses arquivos através de commits, que são snapshots (fotografias) do estado do projeto em determinado momento. Isso possibilita voltar a versões anteriores, criar e mesclar diferentes linhas de desenvolvimento (ramificações), e colaborar de maneira eficiente em equipes, minimizando conflitos.

</p>

<h5> Principais Comandos </h5>

<h6> Navegar até o Diretório </h6>

```bash 
  cd caminho/para/o/seu/repositório
```

<h6>Inicializar um Repositório Git</h6>

```bash
  git init
```

<h6>Configuração Inicial (Se ainda não configurou)</h6>

```bash
  git config --global user.name "SeuNome"
  git config --global user.email "seuemail@example.com"
```

<h6>Trocar branch</h6>

```bash
  git checkout main
 ```

<h6>Criar e Trocar para a branch</h6>

```bash
  git checkout -b nome_da_branch
 ```

<h6> Adicionar Arquivos ao Stage </h6>

```bash
  git add nome_do_arquivo_ou_pasta
  git add .  ->  Adiciona todos os arquivos
```

<h6> Verificar Status do Git </h6>

```bash
 git status
```

<h6>Obtenha o URL do Repositório Remoto</h6>
<p>No GitHub, vá até o seu repositório e clique no botão "Code". Certifique-se de escolher a opção "HTTPS" ou "SSH" para obter o URL correto.</p>

<h6> Adicione o Repositório Remoto ao seu Repositório Local </h6>

```bash
 git remote add origin URL_do_seu_repositório_no_GitHub
```

<p>Por exemplo, se estiver utilizando HTTPS<p>

```bash
 git remote add origin https://github.com/seu_usuario/seu_repositorio.git
```

<h6> Verificar a Origem Adicionada </h6>

```bash
  git remote -v
```

<h6> Criar o Commit </h6>

```bash
  git commit -m "Mensagem descritiva do commit"
```

<h6> Puxar arquivos do repositório remoto </h6>

```bash
  git pull origin nome_da_branch
```

<h6> Enviar Commits para a Origem Remota </h6>

```bash
  git push origin nome_da_branch
```
<p> Nesse momento, o terminal vai pedir suas credencias: username e password, porem a senha como chave de acesso foi descontinuada do github em 2021, e voce precisa substitui-la por um token de acesso, que pode ser gerado manualmente nas configuracoes de sua conta.</p>

</br>

<h5> Outros Comandos Úteis </h5>

<h6> Forca o comando push </h6>

```bash
 git push origin nome_da_branch -f

```

<h6> Permitir a União de Histórias Não Relacionadas </h6>

```bash
 git pull origin nome_da_branch --allow-unrelated-histories

```
<p> Necessário quando você está tentando mesclar duas branches que não têm históricos comuns, o que pode acontecer, por exemplo, quando você cria uma nova branch a partir de uma existente e o Git não reconhece a relação entre elas</p>

<h6> Excluir uma Branch </h6>

```bash
  git branch -d nome_da_branch   # Para remover localmente
  git push origin --delete nome_da_branch   # Para remover do repositório remoto

```



