## 1️⃣ O que é um Repositório Local e Remoto

- *Repositório Local:*  
 Um repositório local é a cópia do seu projeto que reside no seu próprio computador onde você  edita e versiona os arquivos com o Git.

- *Repositório Remoto:*  
  Um repositório remoto é uma versão do seu projeto que é hospedada em um          servidor na internet (em plataformas como *GitHub, **GitLab* ou *Bitbucket*)
, servindo como um ponto centralizado para compartilhar e sincronizar o trabalho.

2️⃣ Comandos Básicos do Git
Comando	Descrição
bash  

git  --> init	Cria um novo repositório Git dentro da pasta atual

git  --> status	Mostra o estado atual dos arquivos

git  --> add .	Adiciona todos os arquivos modificados à área de preparação (staging area)

git  --> commit -m "mensagem"	Salva (confirma) as alterações com uma mensagem explicando o que foi feito

git  --> log	Mostra o histórico de commits

git   --> branch	Lista, cria ou deleta branches do projeto

git  --> checkout	Troca de branch ou restaura versões antigas de arquivos

git merge -->	Junta as alterações de uma branch com outra

git push  -->	Envia os commits do repositório local para o remoto

git pull   -->	Baixa as atualizações do remoto e mescla com o local
`

3️⃣ Criar um Repositório Remoto passo a passo :

PASSO 1: Acesse o GitHub e abra sua conta

PASSO 2: Criar um novo repositório;
                 acesse a Dashboard do site depois vai no canto superior direito, clique no “+”  ou            “New repository”.

PASSO 3: Preencha as informações do repositório
Campo

O que colocar       
Repository namNome do seu repositório (ex: meu-projeto)
Description (opcional)
Uma breve descrição do projeto
Visibility
Escolha Public (visível a todos) ou Private (apenas você)
Initialize this repository with:
Pode deixar desmarcado se for clonar depois, ou marcar Add a README se quiser começar com um README


Acesse https://github.com
 e faça login.

Clique no botão “+” → “New repository”.

Escolha um nome para o repositório, adicione uma descrição opcional e defina se será público ou privado.

Deixe desmarcadas as opções de inicialização (como “Add a README”) se já tiver um repositório local.

Clique em “Create repository”.

Copie a URL do repositório remoto que aparece após a criação.

4️⃣ Clonar um Repositório

Use o comando abaixo para baixar uma cópia completa de um repositório remoto para sua máquina:

git clone https://github.com/seuusuario/meu-projeto.git


Isso cria uma nova pasta com todos os arquivos e o histórico do projeto.

5️⃣ O que é Conventional Commits

Conventional Commits é um padrão para mensagens de commit.
Ele define um formato padronizado para descrever claramente o tipo de mudança feita no código, tornando o histórico mais organizado e fácil de entender.

💡 Estrutura básica:
<tipo>(<escopo>): <descrição>


tipo: define o tipo da mudança (ex: feat, fix, docs, etc.)

escopo: indica onde foi feita a mudança (ex: api, login, readme) — opcional

descrição: um resumo curto e claro do que foi feito

🔹 Tipos mais comuns:
bash
Tipo	Significado
feat	adiciona uma nova funcionalidade
fix	corrige um erro
docs	mudanças apenas na documentação
style	ajustes visuais ou de formatação (sem alterar código funcional)
refactor	melhora o código sem mudar o comportamento
test	adiciona ou altera testes
chore	tarefas de manutenção (build, dependências, etc.)


6️⃣ Fazer o Primeiro Commit com Conventional Commits
Exemplo:

Crie ou edite o arquivo README.md e depois execute:

git add README.md
git commit -m "docs(readme): add initial README with project description"
git branch -M main
git remote add origin https://github.com/seuusuario/meu-projeto.git
git push -u origin main


💬 Explicação do commit:

docs → porque é documentação

(readme) → escopo da alteração

add initial README with project description → descrição clara e curta
