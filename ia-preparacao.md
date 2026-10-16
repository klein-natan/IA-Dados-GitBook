# Antes da Aula 6 · Prepare o Seu Computador

Nas próximas cinco aulas, você vai construir e publicar cinco projetos com agentes de IA. Se a instalação acontecer em casa, sobra tempo de aula para o que importa: entender a IA e usá-la bem.

Faça tudo abaixo antes da Aula 6. Leva de 40 minutos a uma hora. Tudo aqui é gratuito.

## Do que você precisa

* Um computador com **Windows 10 ou 11** ou **macOS 12 ou mais recente**. Celular e tablet não servem para os projetos.
* Uns **10 GB livres** no disco.
* Permissão para instalar programas. No laboratório da faculdade, você tem.
* Internet e um aplicativo autenticador no celular (Google Authenticator ou Microsoft Authenticator), para a segurança do GitHub.

{% hint style="info" %}
**Abrindo o terminal.** Vários passos pedem para digitar um comando. No **Windows**, abra o menu Iniciar, digite **PowerShell** e abra o aplicativo. No **macOS**, abra o **Terminal** (Aplicativos → Utilitários). Digite o comando e aperte Enter. Depois de instalar um programa, **feche o terminal e abra outro**: só o terminal novo enxerga o programa recém-instalado.
{% endhint %}

## Passo 1 · Conta Google pessoal

Você vai entrar no Antigravity com uma conta Google. Se já tem um Gmail pessoal, pule este passo. Se não tem, crie em accounts.google.com.

{% hint style="warning" %}
Use uma conta **pessoal** (terminada em gmail.com). Contas institucionais, do Google Workspace da faculdade ou da empresa, podem não funcionar no Antigravity.
{% endhint %}

## Passo 2 · Conta no GitHub

O GitHub guarda o código dos seus projetos e publica os seus sites.

1. Acesse **github.com/signup**.
2. Digite seu e-mail, crie uma senha e escolha o **nome de usuário**. Ele vira o endereço do seu site: o usuário `anasilva` publica em `anasilva.github.io`. Prefira algo curto e profissional, sem números aleatórios.
3. Confirme o e-mail com o código que o GitHub enviar.
4. Ative a **autenticação em dois fatores**, que o GitHub exige: vá em **Settings → Password and authentication → Enable two-factor authentication**, escolha **Authenticator app** e leia o QR code com o aplicativo autenticador do celular.
5. Baixe e guarde os **códigos de recuperação** que o GitHub mostrar. Sem eles, perder o celular pode significar perder a conta.

{% hint style="success" %}
Estudantes podem pedir o **GitHub Education** (education.github.com), que libera ferramentas pagas de graça, como o GitHub Copilot. A aprovação pode levar alguns dias.
{% endhint %}

## Passo 3 · Git

O Git tira "fotos" da sua pasta de projeto e as envia ao GitHub.

{% tabs %}
{% tab title="Windows" %}
1. Acesse **git-scm.com/downloads/win** e baixe o instalador **64-bit Git for Windows Setup**.
2. Abra o instalador e clique em **Next** em todas as telas, sem mudar nada. As opções padrão servem.
3. Clique em **Install** e depois em **Finish**.

Quem preferir o terminal pode instalar com um comando só:

```text
winget install --id Git.Git -e
```
{% endtab %}

{% tab title="macOS" %}
1. Abra o Terminal e digite `git --version`.
2. Se o Git não estiver instalado, o macOS oferece instalar as **Ferramentas de Linha de Comando**. Clique em **Instalar** e aguarde.

Quem usa o Homebrew pode instalar com `brew install git`.
{% endtab %}
{% endtabs %}

**Confira.** Abra um terminal novo e digite `git --version`. Deve aparecer algo como `git version 2.51.0`.

**Diga ao Git quem você é.** Cada "foto" leva o nome de quem a tirou. Digite os dois comandos abaixo, trocando pelo seu nome e pelo e-mail da conta do GitHub:

```text
git config --global user.name "Ana Silva"
git config --global user.email "ana.silva@gmail.com"
```

## Passo 4 · GitHub CLI

O GitHub CLI (o comando `gh`) deixa o agente criar repositórios e publicar sites no GitHub por você.

{% tabs %}
{% tab title="Windows" %}
1. Acesse **cli.github.com** e clique em **Download for Windows**.
2. Abra o arquivo `.msi` baixado e siga o instalador até o fim, sem mudar nada.

Pelo terminal:

```text
winget install --id GitHub.cli -e
```
{% endtab %}

{% tab title="macOS" %}
1. Acesse **cli.github.com** e baixe o instalador para macOS.
2. Abra o arquivo baixado e siga o instalador.

Quem usa o Homebrew pode instalar com `brew install gh`.
{% endtab %}
{% endtabs %}

**Confira.** Num terminal novo, digite `gh --version`. Deve aparecer algo como `gh version 2.80.0`.

## Passo 5 · Conecte o computador ao GitHub

Este é o único passo de GitHub que você faz à mão. Depois dele, o agente cuida do resto.

No terminal, digite o comando abaixo e responda às perguntas assim (use as setas do teclado e Enter):

```text
gh auth login
```

| O terminal pergunta | Você escolhe |
| --- | --- |
| Where do you use GitHub? | **GitHub.com** |
| What is your preferred protocol for Git operations? | **HTTPS** |
| Authenticate Git with your GitHub credentials? | **Yes** |
| How would you like to authenticate GitHub CLI? | **Login with a web browser** |

O terminal mostra um código de oito caracteres, como `A1B2-C3D4`. Copie o código e aperte Enter. O navegador abre a página do GitHub: entre na sua conta, cole o código e clique em **Authorize**.

**Confira.** Digite `gh auth status`. Deve aparecer `Logged in to github.com account seu-usuario`.

{% hint style="warning" %}
**No computador do laboratório**, ao fim de cada aula, digite `gh auth logout` e saia das suas contas no navegador e nos agentes. Assim, o próximo aluno não usa o seu GitHub.
{% endhint %}

## Passo 6 · Python

O Python só é usado na Aula 10, mas instale agora para não perder tempo depois.

{% tabs %}
{% tab title="Windows" %}
1. Acesse **python.org/downloads** e clique no botão amarelo **Download Python**.
2. Abra o instalador. Na primeira tela, **marque a caixa "Add python.exe to PATH"**, embaixo. Sem ela, o computador não encontra o Python depois.
3. Clique em **Install Now** e aguarde.
4. Se aparecer a opção **Disable path length limit**, clique nela. Depois clique em **Close**.
{% endtab %}

{% tab title="macOS" %}
1. Acesse **python.org/downloads** e clique no botão amarelo **Download Python**.
2. Abra o arquivo `.pkg` e siga o instalador.
3. No fim, dê dois cliques no arquivo **Install Certificates.command**, que aparece na pasta do Python. Ele evita erros de conexão segura.
{% endtab %}
{% endtabs %}

**Confira.** Num terminal novo, digite `python --version` no Windows ou `python3 --version` no macOS. Deve aparecer algo como `Python 3.14.0`.

{% hint style="info" %}
No Windows, se o comando `python` abrir a Microsoft Store em vez de mostrar a versão, vá em **Configurações → Aplicativos → Configurações avançadas de aplicativos → Aliases de execução de aplicativo** e desligue os dois itens do **Instalador de aplicativo (python.exe e python3.exe)**. Depois abra um terminal novo.
{% endhint %}

## Passo 7 · Os três agentes

Você vai conhecer três agentes de IA. Vale ter os três instalados: quando a cota gratuita de um acabar, você continua no outro.

**Google Antigravity**

{% tabs %}
{% tab title="Windows" %}
1. Acesse **antigravity.google** e clique em **Download**. Escolha a versão para Windows.
2. Abra o instalador e siga as telas até o fim.
3. Abra o Antigravity e clique em **Sign in with Google**. Entre com a conta Google pessoal do Passo 1.
4. Nas telas de configuração inicial, aceite as opções padrão.
{% endtab %}

{% tab title="macOS" %}
1. Acesse **antigravity.google** e clique em **Download**. Escolha a versão para o seu Mac (Apple Silicon para os modelos com chip M; Intel para os mais antigos).
2. Abra o arquivo `.dmg` e arraste o Antigravity para a pasta **Aplicativos**.
3. Abra o Antigravity e clique em **Sign in with Google**. Entre com a conta Google pessoal.
4. Aceite as opções padrão da configuração inicial.
{% endtab %}
{% endtabs %}

**OpenCode**

1. Acesse **opencode.ai** e baixe o **aplicativo de desktop** para o seu sistema. Instale como qualquer programa.
2. Abra o OpenCode, digite `/connect` na caixa de mensagem e escolha **opencode**.
3. O OpenCode pede uma chave. Acesse **opencode.ai/auth**, entre com a sua conta (pode usar o GitHub) e copie a chave mostrada.
4. Cole a chave no OpenCode. Pronto: você tem acesso aos modelos gratuitos do OpenCode Zen.

**Cursor**

1. Acesse **cursor.com** e clique em **Download**. Instale como qualquer programa.
2. Ao abrir pela primeira vez, crie uma conta ou entre com uma existente. Use o plano gratuito.
3. Se o Cursor perguntar se você quer importar configurações do VS Code, pode pular.

{% hint style="info" %}
Os planos gratuitos mudam com frequência. Em outubro de 2026, o Antigravity tinha uma cota semanal, o OpenCode oferecia modelos gratuitos que mudam de tempos em tempos, e o Cursor dava uma cota inicial com modelos Grok. O que importa: com três agentes, sempre há um disponível.
{% endhint %}

## Passo 8 · Conta no OpenRouter

O OpenRouter só é usado na Aula 10. Crie a conta agora em **openrouter.ai** → **Sign up**. Pode entrar com o Google ou com o GitHub. Não é preciso cadastrar cartão.

## Passo 9 · Teste final

Abra qualquer um dos agentes, crie uma pasta vazia chamada `teste-ia`, abra essa pasta no agente e peça:

```text
Verifique se git, gh e python estão instalados e me diga as versões.
Rode "gh auth status" e me diga com qual usuário do GitHub estou conectado.
Depois crie um arquivo ola.html com a frase "Funcionou!" e abra no navegador.
```

O agente vai pedir permissão para rodar comandos. Leia cada comando e aprove. Se ele disser as três versões e o seu usuário do GitHub, e aparecer "Funcionou!" no navegador, está tudo pronto.

**Lista final:**

* [ ] Conta Google pessoal
* [ ] Conta GitHub com autenticação em dois fatores e códigos de recuperação guardados
* [ ] `git --version` e `git config` feitos
* [ ] `gh auth status` mostra o seu usuário
* [ ] `python --version` (ou `python3 --version`) mostra a versão
* [ ] Antigravity, OpenCode e Cursor abrem e estão conectados às suas contas
* [ ] Conta no OpenRouter criada
* [ ] Teste final funcionou

## Se algo der errado

| Sintoma | O que fazer |
| --- | --- |
| "git", "gh" ou "python" não é reconhecido como comando | feche o terminal e abra outro; se continuar, reinstale o programa e reinicie o computador |
| `python` abre a Microsoft Store | desligue os aliases de execução (veja a caixa do Passo 6) |
| o instalador pede senha de administrador no laboratório | chame o professor ou o técnico do laboratório |
| `gh auth status` diz que você não está conectado | repita o Passo 5 |
| o GitHub pede um código de dois fatores e você perdeu o celular | use um dos códigos de recuperação do Passo 2 |
| o Antigravity não aceita a conta | use uma conta gmail.com pessoal |
| um agente parou com aviso de limite | os planos gratuitos têm cota; troque para outro agente ou trabalhe em dupla |
| o antivírus bloqueou um instalador | baixe de novo pelo site oficial listado aqui; nunca de sites de terceiros |

{% hint style="info" %}
Traga para a Aula 6 duas ou três informações sobre você que gostaria de mostrar num portfólio: formação, cursos, experiências, interesses. Nada de documento ou endereço.
{% endhint %}
