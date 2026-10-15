# Antes da Aula 6 · Prepare o Seu Computador

Nas próximas cinco aulas, você vai construir e publicar cinco projetos com agentes de IA. Se a instalação acontecer em casa, sobra tempo de aula para o que importa: entender a IA e usá-la bem.

Faça tudo abaixo antes da Aula 6. O computador do laboratório também serve: lá você pode instalar o que precisar. Tudo aqui é gratuito.

## As contas

| Conta | Para quê | Onde |
| --- | --- | --- |
| **Google pessoal** (gmail.com) | entrar no Antigravity | accounts.google.com |
| **GitHub** | guardar o código e publicar os sites | github.com |
| **OpenCode** | usar os modelos gratuitos do OpenCode | opencode.ai |
| **Cursor** | entrar no Cursor | cursor.com |
| **OpenRouter** | usar modelos de IA por API na Aula 10 | openrouter.ai |

{% hint style="warning" %}
Use uma conta Google **pessoal**. Contas institucionais (do Google Workspace da faculdade ou da empresa) podem não funcionar no Antigravity.
{% endhint %}

No GitHub, escolha o nome de usuário com cuidado. Ele vira o endereço do seu site: o usuário `anasilva` publica em `anasilva.github.io`. Prefira algo profissional e curto.

## Os programas

**1. Git.** Tira "fotos" da sua pasta de projeto e as envia ao GitHub. No Windows, baixe em git-scm.com e aceite as opções padrão do instalador. No macOS, abra o Terminal e digite `git --version`; se não estiver instalado, o sistema oferece a instalação.

**2. GitHub CLI.** Permite que o agente crie repositórios e publique sites no GitHub por você. Baixe em cli.github.com e instale.

**3. Os três agentes.** Você vai conhecer três, e vale ter os três instalados: quando a cota gratuita de um acabar, você continua no outro.

* **Google Antigravity:** baixe em antigravity.google e entre com a conta Google pessoal.
* **OpenCode:** baixe o aplicativo de desktop em opencode.ai (também existe versão para o terminal). Ao abrir, use o comando `/connect`, escolha **opencode** e cole a chave que aparece em opencode.ai/auth. Assim você usa os modelos gratuitos do OpenCode Zen.
* **Cursor:** baixe em cursor.com e crie a conta.

**4. Python.** Só é usado na Aula 10, mas instale agora. Baixe a versão mais recente em python.org.

{% hint style="warning" %}
No instalador do Python para Windows, marque a caixa **"Add python.exe to PATH"** na primeira tela. Sem ela, o computador não encontra o Python depois.
{% endhint %}

## Conecte o GitHub uma única vez

Este é o único passo de GitHub que você faz à mão. Depois dele, o agente cuida do resto.

Abra o terminal (no Windows, o **PowerShell**), digite o comando abaixo e responda às perguntas assim:

```text
gh auth login
```

| O terminal pergunta | Você escolhe |
| --- | --- |
| Where do you use GitHub? | **GitHub.com** |
| What is your preferred protocol for Git operations? | **HTTPS** |
| Authenticate Git with your GitHub credentials? | **Yes** |
| How would you like to authenticate GitHub CLI? | **Login with a web browser** |

O terminal mostra um código de oito caracteres. Aperte Enter, o navegador abre, cole o código e autorize. Pronto: o seu computador agora pode criar repositórios e publicar no seu nome.

## Teste de cinco minutos

Abra qualquer um dos agentes, crie uma pasta vazia chamada `teste-ia` e peça:

```text
Verifique se git, gh e python estão instalados e me diga as versões.
Rode "gh auth status" e me diga com qual usuário do GitHub estou conectado.
Depois crie um arquivo ola.html com a frase "Funcionou!" e abra no navegador.
```

O agente vai pedir permissão para rodar comandos. Leia cada comando e aprove. Se ele disser o seu usuário do GitHub e aparecer "Funcionou!" no navegador, está tudo pronto.

## Se algo der errado

| Sintoma | O que fazer |
| --- | --- |
| "git" ou "gh" não é reconhecido como comando | reinstale o programa e reinicie o computador |
| "python não é reconhecido" | reinstale o Python marcando "Add python.exe to PATH" |
| `gh auth status` diz que você não está conectado | repita `gh auth login` |
| o Antigravity não aceita a conta | use uma conta gmail.com pessoal |
| um agente parou com aviso de limite | os planos gratuitos têm cota; troque para outro agente ou trabalhe em dupla |

{% hint style="info" %}
Traga para a Aula 6 duas ou três informações sobre você que gostaria de mostrar num portfólio: formação, cursos, experiências, interesses. Nada de documento ou endereço.
{% endhint %}
