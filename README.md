# Do TCC ao Artigo

Skill de IA que transforma **TCC, monografia, dissertação, tese, relatório de pesquisa ou dados coletados** em **artigos científicos** para revistas e congressos, nacionais ou internacionais, de **todas as áreas**, e ajuda a **responder aos pareceristas**.

Funciona com **Claude**, **ChatGPT** e **Gemini** (formato aberto [Agent Skills](https://agentskills.io) — arquivo `SKILL.md`), e também como instruções de GPT personalizado, Gem ou Projeto.

**Autor:** Carlaile L. do Vale — Cientista da Computação · carlailevale@gmail.com
**Versão:** 1.1.0 · **Licença:** CC BY-NC 4.0 (uso não comercial)

---

## O que a skill faz
1. Mostra um **aviso sobre o uso ético da IA**, **privacidade** (anonimizar dados, desligar o treinamento com suas conversas) e **autoplágio**.
2. Pede o documento e faz uma **entrevista**: tipo de trabalho, revista ou congresso, nacional ou internacional, edital/link, autores, prazo, **revistas com ou sem taxa** e **formato de entrega (DOCX, LaTeX ou template da revista)**.
3. Analisa o documento e monta um **Mapa do Trabalho**, inclusive a idade das referências (se forem antigas, pergunta se deve buscar literatura recente).
4. Sugere **quantos artigos** podem sair do material, normalmente **3 propostas** com título, objetivo, mini-resumo e onde publicar.
5. Pesquisa as **normas da revista** e as **normas atualizadas** da área.
6. Escreve **seção por seção** com os critérios do livro de Italo de Souza Aquino.
7. Faz a **revisão final** e entrega o manuscrito, o abstract, a carta ao editor e a **declaração de uso de IA**.
8. **Depois da submissão**: organiza os pareceres, redige a carta de resposta e ajuda na ressubmissão.

A skill **nunca inventa** dados nem referências: o que faltar fica marcado como `[PREENCHER]` ou `[VERIFICAR]`.

## Estrutura
```
do-tcc-ao-artigo/
├── README.md
├── LICENSE
├── CHANGELOG.md
├── GUIA-GITHUB.md                ← passo a passo para quem nunca usou o GitHub
├── tcc-para-artigo/              ← a skill (esta pasta vira o .zip)
│   ├── SKILL.md
│   ├── references/
│   │   ├── criterios-aquino.md
│   │   ├── normas-atualizadas.md
│   │   ├── areas.md
│   │   ├── etica-ia.md
│   │   └── questionario.md
│   └── templates/
│       ├── proposta-artigos.md
│       ├── estrutura-artigo.md
│       ├── checklist-revisao.md
│       └── resposta-pareceristas.md
└── prompt-unico/
    └── instrucoes-gpt-gem.md     ← versão para GPT personalizado / Gem / Projeto
```

## Como instalar

### Claude (claude.ai, app desktop ou celular)
1. Baixe `tcc-para-artigo.zip` em **Releases** (lado direito desta página).
2. Vá em **Configurações → Capacidades → Skills → Upload skill** e envie o .zip.
3. Ative a skill e peça: *"Quero transformar minha dissertação em artigo"*.

### Claude Code, Codex CLI, Gemini CLI, Copilot, Cursor
Copie a pasta `tcc-para-artigo/` para a pasta de skills da ferramenta (ex.: `~/.claude/skills/`, `~/.codex/skills/`, `~/.gemini/skills/`).

### ChatGPT e Gemini (app)
- Se a sua conta já tem **Skills**, envie o mesmo .zip pela área de skills.
- Se não tem: crie um **GPT personalizado** (ChatGPT) ou um **Gem** (Gemini), cole o texto de `prompt-unico/instrucoes-gpt-gem.md` em *Instruções* e anexe os arquivos de `references/` e `templates/` como *Conhecimento*. Ative a busca na web.

## Uso responsável
Ferramenta de **apoio**. A responsabilidade científica, ética e legal do artigo é dos autores. Declare o uso de IA conforme as normas da revista ou do evento ([COPE](https://publicationethics.org/guidance/cope-position/authorship-and-ai-tools), [SciELO](https://wp.scielo.org/wp-content/uploads/Guia-de-uso-de-ferramentas-e-recursos-de-IA-20230914.pdf)).

## Base metodológica
AQUINO, Italo de Souza. *Como escrever artigos científicos: sem "arrodeio" e sem medo da ABNT*. 7. ed. São Paulo: Saraiva, 2010.
Os critérios do livro foram **resumidos com palavras próprias**; o livro não é distribuído aqui. Para aprofundar, adquira a obra.

## Licença
[CC BY-NC 4.0](LICENSE) — pode usar, adaptar e compartilhar **sem fins comerciais**, citando o autor *Carlaile L. do Vale*. Usar a skill para escrever os seus próprios artigos é permitido. Para uso comercial, contate o autor.

## Como citar
VALE, Carlaile L. do. **Do TCC ao Artigo**: skill de IA para transformar trabalhos acadêmicos em artigos científicos. Versão 1.1.0. 2026. Disponível em: https://github.com/carlailevale/do-tcc-ao-artigo.

## Contribuições
Sugestões e correções são bem-vindas via *Issues* ou *Pull Requests*, ou pelo e-mail carlailevale@gmail.com.
