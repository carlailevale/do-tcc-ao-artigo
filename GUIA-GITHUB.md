# Guia rápido: publicar a skill no GitHub (sem programar)

Tudo é feito pelo navegador, em github.com. Tempo estimado: 15 minutos.

## Antes de começar
1. No seu computador, descompacte o arquivo `do-tcc-ao-artigo-github.zip`. Vai aparecer a pasta `do-tcc-ao-artigo`.
2. Guarde também o arquivo `tcc-para-artigo.zip` (é o que as pessoas vão baixar).
3. Entre em https://github.com com seu usuário e senha.

## Passo 1 — Criar o repositório (a "pasta" do projeto)
1. No canto superior direito, clique no **+** e depois em **New repository**.
2. **Repository name**: `do-tcc-ao-artigo`
3. **Description**: `Skill de IA que transforma TCC, dissertação e tese em artigos científicos`
4. Marque **Public**.
5. **Não** marque "Add a README file" (você já tem um).
6. Clique em **Create repository**.

## Passo 2 — Enviar os arquivos
1. Na página que abrir, clique no link **uploading an existing file**.
2. Abra a pasta `do-tcc-ao-artigo` no seu computador, selecione **tudo o que está dentro dela** (README.md, LICENSE, CHANGELOG.md, GUIA-GITHUB.md e as pastas `tcc-para-artigo` e `prompt-unico`) e **arraste** para a área do navegador.
   - Use Chrome ou Edge: eles enviam as pastas com as subpastas.
3. Espere todos os arquivos aparecerem na lista.
4. Em **Commit changes**, escreva: `Versão 1.1.0`.
5. Clique em **Commit changes**.
6. Confira: a página inicial do repositório deve mostrar o README formatado e a pasta `tcc-para-artigo` contendo `SKILL.md`, `references` e `templates`.

## Passo 3 — Ajustar o link de citação
1. Clique em `README.md` e depois no ícone de **lápis** (Edit).
2. Procure `SEU-USUARIO` e troque pelo seu nome de usuário do GitHub.
3. Clique em **Commit changes** (duas vezes).

## Passo 4 — Criar a versão para download (Release)
1. Na página do repositório, à direita, clique em **Create a new release** (ou em **Releases → Draft a new release**).
2. Em **Choose a tag**, digite `v1.1.0` e clique em **Create new tag**.
3. **Release title**: `Do TCC ao Artigo 1.1.0`
4. Na descrição, cole: `Baixe tcc-para-artigo.zip e envie no Claude em Configurações → Capacidades → Skills → Upload skill.`
5. Arraste o arquivo `tcc-para-artigo.zip` para a área **Attach binaries**.
6. Clique em **Publish release**.

## Passo 5 — Deixar o projeto fácil de achar
1. Na página inicial, à direita, clique na **engrenagem** ao lado de **About**.
2. Em **Topics**, adicione: `agent-skills`, `claude-skill`, `chatgpt`, `gemini`, `escrita-cientifica`, `abnt`, `tcc`, `artigo-cientifico`.
3. Clique em **Save changes**.

## Passo 6 — Compartilhar
O endereço do seu projeto será: `https://github.com/SEU-USUARIO/do-tcc-ao-artigo`
Compartilhe esse link. Quem quiser usar baixa o .zip em **Releases**.

## Como atualizar no futuro
- **Trocar um arquivo**: abra o arquivo no GitHub → lápis (Edit) → altere → **Commit changes**.
- **Enviar arquivos novos**: **Add file → Upload files** (arquivos com o mesmo nome são substituídos).
- **Nova versão**: atualize o `version` no `SKILL.md` e o `CHANGELOG.md`, gere um novo .zip e crie uma nova Release (ex.: `v1.2.0`).

## Opcional — DOI para citar no Lattes
1. Entre em https://zenodo.org com sua conta do GitHub.
2. Em **GitHub**, ative o repositório `do-tcc-ao-artigo`.
3. Crie uma nova Release no GitHub: o Zenodo gera um DOI automaticamente.

## Nunca envie
- O PDF do livro (direitos autorais).
- TCCs, dados ou documentos de outras pessoas.
- Senhas ou informações pessoais.
