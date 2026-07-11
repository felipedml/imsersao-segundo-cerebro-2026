# Imersão Segundo Cérebro — Sistema de Clone Acadêmico

**Felipe Asensi** | Salvador/BA | Julho de 2026

---

## O que é isto?

A **Imersão Segundo Cérebro** é um sistema que transforma uma IA genérica em seu **clone acadêmico pessoal** — uma versão que pensa e escreve como você, comanda um squad de robôs especialistas, e acelera todo o ciclo de pesquisa sem nunca inventar referências ou perder sua voz autoral.

Este repositório contém a **arquitetura completa** do sistema: a metodologia, o perfil-chave que personaliza tudo, e os 7 agentes especializados que trabalham na sua voz.

---

## Por que existe

Pesquisadores enfrentam **dores reais**:
- Ficam presos entre escrever tudo sozinho (lento) e usar IA genérica (perde a voz, alucina referências).
- Gastar energia em estrutura quando poderiam focar em ideias.
- Não ter um par crítico antes de submeter.

**Este sistema resolve** porque:
- ✅ Acelera sem copiar (você continua sendo o autor)
- ✅ Preserva sua voz em tudo (tom, estrutura, argumentação)
- ✅ Nunca inventa referência (marca `[verificar]` quando em dúvida)
- ✅ Oferece parecerista rigoroso antes da banca
- ✅ Transforma texto em entregáveis (slides, apostilas, apps)

---

## Estrutura do Repositório

```
imsersao-segundo-cerebro-2026/
│
├── 📖 CLAUDE.md                         ← Instruções do sistema (leia primeiro)
├── 📖 COMECE-AQUI.md                    ← Guia de 3 passos para começar
├── 📖 metodo-felipe-asensi.md           ← Metodologia compartilhada (todas as seções)
├── 📋 perfil-do-pesquisador.md          ← Seu perfil (preenchido pelo clonador)
├── 📋 README.md                         ← Este arquivo
│
├── .claude/
│   └── agents/                          ← Squad de 7 agentes especializados
│       ├── clonador.md                  ← Entrevista e cria seu perfil
│       ├── arquiteto-da-pesquisa.md     ← Desenha pesquisa (Promessa → Metodologia)
│       ├── revisao-de-literatura.md     ← Busca, tria e sintetiza literatura
│       ├── escritor.md                  ← Redige pelo Método 1em10
│       ├── peer-review.md               ← Avalia em 5 dimensões
│       ├── produtor-de-materiais.md     ← Transforma em slides, apostilas, dashboards
│       └── arquiteto-de-apps.md         ← Cria apps HTML acadêmicos
│
├── minhas-amostras/                     ← Onde você deixa seus textos
│   └── LEIAME.md                        ← Instruções (2–3 trechos que o clone aprende)
│
└── meu-projeto/                         ← Onde os robôs entregam
    └── LEIAME.md                        ← Instruções (rascunhos, projetos, pareceres)
```

---

## Os 7 Agentes — O Squad Acadêmico

Cada robô lê seu **perfil** (`perfil-do-pesquisador.md`) e trabalha na sua mente e voz. Nenhum inventa referência.

### 1️⃣ **Clonador**
- **Função:** Entrevista você uma única vez (≈20 min) e escreve `perfil-do-pesquisador.md`
- **Extrai:** Mente (como pensa), Voz (como escreve), Repertório (com o que trabalha)
- **Resultado:** Perfil que define seu clone; você dá um nome a ele
- **Quando chamar:** Na PRIMEIRA vez (se perfil está vazio) ou quando disser *"quero me clonar"*

### 2️⃣ **Arquiteto da Pesquisa**
- **Função:** Desenha pesquisa antes da escrita
- **Fluxo:** Promessa → Problema → Hipótese → Objetivo Geral → Objetivos Específicos → Metodologia
- **Resultado:** Esqueleto decisório com 4 decisões de metodologia (coleta, análise, ética)
- **Quando chamar:** No começo da pesquisa, quando tem vontade vaga

### 3️⃣ **Revisão de Literatura**
- **Função:** Levanta e sintetiza literatura orientada pelo **problema** (não tema)
- **Fluxo:** String booleana → busca em bases abertas → PRISMA → síntese em 4 passos → quadro comparativo → lacuna
- **Bases automáticas:** PubMed, OpenAlex, Crossref, Semantic Scholar, Zenodo, SciELO, LILACS
- **Bases fechadas:** Entrega string adaptada para Scopus/WoS (você exporta `.ris/.bib`)
- **Resultado:** Síntese argumentativa com lacuna específica
- **Regra de ouro:** Nunca inventa referência — todo DOI é verificável

### 4️⃣ **Escritor**
- **Função:** Redige produtos acadêmicos pelo **Método 1em10**
- **Tipos:** Artigos, projetos, TCCs, dissertações, teses, resumos, relatórios
- **Fluxo:** Esqueleto → ITPR (Isca·Tema·Promessa·Rota) → argumentos + citações → autoralidade → PRLDF (Promessa·Rota·Limites·Desdobramentos·Finalização)
- **Resultado:** Rascunho na sua voz (última palavra é sua)
- **Garantia:** Nunca reescreve sem pedido; preserva voz autoral

### 5️⃣ **Peer Review**
- **Função:** Parecerista rigoroso nas 5 dimensões
  1. **Coerência:** Alinhamento problema → hipótese → OE → metodologia
  2. **Especificidade:** Texto autoexplicativo?
  3. **Viabilidade:** Método executável no prazo?
  4. **Persuasão:** Convence um avaliador externo?
  5. **Vícios:** Juízo de valor, sujeito oculto, verbo no passado?
- **Resultado:** Diagnóstico completo → 3 problemas mais críticos → localizável + reescrita sugerida
- **Quando chamar:** Antes de submeter à banca, periódico ou edital

### 6️⃣ **Produtor de Materiais**
- **Função:** Transforma qualquer entrega em artefato pronto
- **Formatos:** Slides (defesa, aula), apostilas, guias, tutoriais, dashboards, sites/landing pages, planilhas
- **Resultado:** Arquivo pronto para abrir e usar (Word, PDF, HTML, Excel)
- **Quando chamar:** Quando tem um texto e quer virar *apresentação, apostila ou dashboard*

### 7️⃣ **Arquiteto de Apps**
- **Função:** Cria mini apps acadêmicos HTML (sem você programar)
- **Exemplos:** Dashboard de andamento, organizador de referências, Kanban de escrita, calculadora de amostra, checklist PRISMA, quiz interativo, gerador de string booleana
- **Resultado:** Arquivo `.html` único que abre no navegador, offline, sem instalar nada
- **IA BYOK:** Se quiser recurso com IA (revisor na sua voz, resumidor, gerador de hipóteses), você plugava sua própria chave OpenAI — nunca vem embutida
- **Quando chamar:** Quando quer uma ferramenta interativa para organizar, calcular, testar ou divulgar

---

## Como Começar — 3 Passos

### 1. Abrir no Claude Code
- No app do Claude Code, clique em **Open Folder**
- Selecione esta pasta
- Quando perguntar "Trust workspace?", clique em **Confiar**

### 2. Dizer "oi"
Na caixa de conversa, escreva simples: **"oi"**

O sistema vai perceber que você ainda não se clonou e vai chamar o **Clonador**:
- Faz uma entrevista rápida (≈20 min)
- Olha 2–3 textos seus (você pode colar ou arrastar para `minhas-amostras/`)
- Escreve seu perfil
- Você dá um **nome ao clone**

### 3. Usar seu clone
Abra uma **conversa nova** (cada trabalho = conversa nova, contexto limpo) e converse em português natural:
- *"Desenha minha pesquisa sobre X"* → chama o **Arquiteto da Pesquisa**
- *"Levanta a literatura sobre Y"* → chama a **Revisão de Literatura**
- *"Escreve o artigo sobre Z"* → chama o **Escritor**
- *"Faz um parecer neste texto"* → chama o **Peer Review**
- *"Transforma isto em slides"* → chama o **Produtor de Materiais**
- *"Cria um app de Kanban para minha escrita"* → chama o **Arquiteto de Apps**

---

## Metodologia: Método Felipe Asensi

O sistema inteiro usa a **metodologia Felipe Asensi**, documentada em `metodo-felipe-asensi.md`. 11 seções:

1. **Premissas inegociáveis** — Nunca inventar, voz autoral, rigor
2. **A Promessa** — O coração de tudo (Eu prometo…)
3. **Método 1em10** — Escrever em menos tempo, mais qualidade
4. **Escrita acadêmica** — Fundamentos (claro, objetivo, coerente)
5. **Frameworks nomeados** — POA+A, Esqueleto, ITPR, PRLDF, SAEE
6. **Projeto de pesquisa** — Sequência: Problema → Hipótese → OG → OE → Metodologia
7. **Revisão de literatura** — Funil temático, string, PRISMA, síntese
8. **Peer Review** — 5 dimensões críticas (localização exata, reescrita)
9. **Formatação e referências** — ABNT, APA, Vancouver, Chicago, OSCOLA
10. **Como o método vira squad** — Mapa agente ↔ método
11. **Tom e voz** — Português BR, acolhedor com você; impessoal 3ª pessoa no produto

**Tudo é baseado em:** rigor científico, voz autoral, nunca inventar referência.

---

## Seu Perfil — O Cordão Umbilical

`perfil-do-pesquisador.md` define você para o clone. O clonador preenche:

### MENTE (como você pensa)
- Área e tema/problema atual
- Campo epistemológico (positivista, interpretativo, crítico, pragmático)
- Autores e teorias de cabeceira
- Método preferido (quali, quanti, misto)
- Ancoragem (teoria, empiria, método, diálogo com autores)
- Postura (o que defende, o que rejeita)
- Lacuna que persegue

### VOZ (como você escreve)
- Tom (formal impessoal, reflexivo, didático, argumentativo)
- Estrutura de frase e parágrafo (períodos longos ou curtos)
- Vocabulário característico (termos que repetem)
- Conectivos típicos ("nesse sentido", "cumpre destacar")
- Como abre e fecha textos
- Marcas proibidas (o que você nunca escreve)
- Tom por tipo de texto (artigo × projeto × aula)

### REPERTÓRIO (com o que trabalha)
- Trabalhos já publicados
- Bases preferidas (PubMed, SciELO, Google Acadêmico, etc.)
- Norma (ABNT, APA, Vancouver, Chicago)
- Gaps conhecidos

**Todos os 7 agentes leem este arquivo antes de trabalhar.**

---

## Limites (Honestidade)

### ✅ O Clone Replica Bem
- Seu raciocínio e linha argumentativa
- Seu tom e estilo de escrita
- Sua postura teórica
- Seus autores e métodos de referência
- O padrão dos seus textos

### ⚠️ O Clone NÃO Faz
- Inventar referência ou dado (marca `[verificar]` quando em dúvida)
- Pensar com material que você não deu
- Substituir seu julgamento final
- Garantir aprovação ou publicação

**A IA acelera; quem decide e assina é você.**

---

## Estrutura de Pastas de Trabalho

### `minhas-amostras/`
**O que entra:** 2–3 textos seus que o clone vai aprender a sua voz
- Um parágrafo de artigo
- Um pedaço de projeto
- Um capítulo de dissertação
- Formatos: `.txt`, `.md`, `.docx`, `.pdf`

**Por quê:** O clonador analisa sua escrita real (não perguntas genéricas) para extrair tom, estrutura, vocabulário, conectivos — tudo que te faz ser você.

### `meu-projeto/`
**O que entra:** Tudo que os robôs entregam
- Rascunhos de artigos
- Projetos de pesquisa
- Revisões de literatura
- Pareceres
- Slides
- Apps
- Apostilas

**Organização:** Os robôs salvam automaticamente aqui. Você volta quando quer continuar ou revisar um trabalho.

---

## Uso Prático — Exemplo

**Dia 1 — Clonagem**
```
Você: oi
Clonador: [entrevista 20 min] → escreve seu perfil → você dá nome ao clone
```

**Dia 2 — Desenhar pesquisa**
```
Você (nova conversa): Desenha minha pesquisa sobre impacto de IA na educação médica
Arquiteto da Pesquisa: [faz 2 perguntas] → entrega Promessa final + Problema + Hipótese + OG + OE + esboço de metodologia
```

**Dia 3 — Levantamento**
```
Você: Levanta a literatura sobre IA + educação médica
Revisão de Literatura: [monta string] → busca em bases → traz 40 artigos → tria → sintetiza → quadro comparativo → lacuna
```

**Dia 4 — Escrita**
```
Você: Escreve o artigo
Escritor: [monta esqueleto] → escreve ITPR + argumentos + citações → autoralidade → PRLDF → rascunho na sua voz
```

**Dia 5 — Revisão**
```
Você: Faz um parecer neste texto
Peer Review: [lê] → diagnóstico em 5 dimensões → 3 problemas mais críticos → localização exata + reescrita sugerida
```

**Dia 6 — Entregável**
```
Você: Transforma em slides para a defesa
Produtor de Materiais: [gera PowerPoint ou HTML] → pronto para apresentar
```

---

## Regras de Ouro

1. **Nunca inventa referência.** Se não houver base real, marca `[verificar]`.
2. **Voz autoral acima de tudo.** O clone acelera; quem decide e assina é você.
3. **Pergunte 1–2 coisas cirúrgicas.** Não um interrogatório.
4. **Cada trabalho, uma conversa nova.** Contexto limpo, clone sempre igual.
5. **Portugês Brasil, simples.** Com você é acolhedor; no produto é 3ª pessoa impessoal.

---

## Tecnologia

- **Base:** Metodologia Felipe Asensi (11 seções, destilada de 5 manuais)
- **Personalização:** Perfil do pesquisador (Mente + Voz + Repertório)
- **Execução:** 7 agentes especializados, cada um com ferramentas próprias
- **Armazenamento:** `meu-projeto/` local; você controla tudo
- **Segurança:** Nenhuma chave de API embutida; BYOK para recursos de IA
- **Responsabilidade:** Você é sempre o autor; IA é acelerador

---

## Próximos Passos

1. **Leia** `COMECE-AQUI.md` (3 minutos)
2. **Abra** no Claude Code
3. **Diga** "oi" na caixa de conversa
4. **Deixe** o Clonador conduzir (≈20 min)
5. **Batize** seu clone
6. **Abra** uma conversa nova e use o clone

---

## Licença e Autoria

Desenvolvido por **Felipe Asensi** | Imersão Segundo Cérebro  
Julho de 2026, Salvador/BA

Proibida a venda, revenda, reprodução ou redistribuição não autorizadas.

---

**Bora clonar você. 🎓**
```

---

Você pode copiar este markdown, colar diretamente no seu repositório (atualizando o README.md), e fazer commit!
