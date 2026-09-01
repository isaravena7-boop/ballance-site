# O que o site ainda não responde

Este arquivo existe porque a página tem uma regra: **só vai ao ar o que está
confirmado**. Não há tarja "a confirmar", campo vazio nem preço de mentira em
`index.html` — quando falta o dado, a seção simplesmente não existe.

O efeito colateral é que a falta some de vista. Este documento é o antídoto —
e ele separa duas coisas que se parecem e não são:

- **Parte I — decidido: não vai ao site.** Não está faltando nada. A direção
  decidiu que aquilo não se publica. Não leve estes itens a ninguém.
- **Parte II — falta a resposta.** Aqui sim é buraco: a escola tem a
  informação, ela só não chegou. Cada item é uma pergunta endereçada, com o que
  precisa vir de volta e o que acontece na página quando chegar. O HTML de cada
  um já está pensado; só falta a resposta.

Confundir as duas é o erro caro: buraco alguém preenche de boa-fé.

> **Endereçamos por função, não por nome de pessoa.** É a mesma razão pela qual
> a página não publica nome de professor: os professores são PJ, e nome de gente
> colado a papel fixo é vínculo aparente. Vale aqui também.

---

# Parte I — decidido: não vai ao site

Estes dois itens **não são falta de dado**. São decisão da direção, tomada em
17/08/2026. Ficam registrados aqui para que ninguém, daqui a seis meses, os
confunda com buraco e "resolva" preenchendo.

## D1. Preço — NÃO PUBLICAR

| | |
|---|---|
| **Decisão** | Preço não aparece no site. Direção, 17/08/2026 |
| **Vale para** | Mensalidade, taxa de matrícula, desconto de irmão, "a partir de R$", faixa de preço, e qualquer forma de estimativa |
| **Consequência aceita** | Quem quer saber o valor abre o WhatsApp. É o degrau que a escola escolhe manter |
| **Como isto é defendido** | `02-automacoes-python/site/verificar_site.py`, bloco [7], reprova a página se um preço aparecer — no texto, na meta description, no og:description ou no JSON-LD |

## D2. Faixa etária em anos — NÃO PUBLICAR

| | |
|---|---|
| **Decisão** | Idade em anos não aparece no site. Direção, 17/08/2026 |
| **Vale para** | Idade mínima, idade máxima, "a partir de N anos", faixa por nível |
| **O que a página usa no lugar** | O vocabulário da escola, que já está publicado: Baby, Infantil, Infanto-juvenil, Juvenil, Adulto, e os níveis do syllabus. O encaixe é confirmado por uma pessoa quando a família visita |
| **Consequência aceita** | A mãe que sabe a idade da filha e não sabe traduzir para "Baby 2" pergunta. A escola prefere responder isso caso a caso a errar por escrito |
| **Como isto é defendido** | `verificar_site.py`, bloco [7], reprova a página se uma idade em anos aparecer, nas mesmas superfícies |

---

# Parte II — falta a resposta

Aqui sim é buraco: a escola tem a informação, ela só não chegou. Cada item traz
o que exatamente precisa vir de volta e o que acontece na página quando chegar.

## 1. Aula experimental — RESPONDIDA em 01/09/2026, com quatro pontas soltas

A direção respondeu, e a resposta virou conteúdo: seção `#experimental` (entre
localização e o CTA final), item no menu, segundo botão do herói e uma linha no
fim da grade. Publicado: que existe, que é **paga e o valor volta na primeira
mensalidade** quando a família fecha o plano, que dura uma aula inteira, que se
agenda até a véspera conforme a disponibilidade, que vale para qualquer turma da
grade, o que levar, que o responsável assiste de fora, e que é uma por
modalidade.

**O valor não foi publicado, e não é esquecimento:** D1 vale para ele também. O
fato forte — é paga e volta como desconto — se diz inteiro sem citar número.

| | |
|---|---|
| **Quem responde as pontas** | Secretaria |
| **O que ainda falta** | (a) **Cabelo**: precisa ir preso? (b) **Sapatilha**: a meia antiderrapante serve nos níveis do syllabus também, ou dali para cima já se pede sapatilha? (c) **Prazo do desconto**: a experimental de hoje ainda abate a mensalidade de daqui a dois meses? (d) **Quando a família não fecha**, o valor fica com a escola? |
| **Por que não viraram texto** | Nenhuma das quatro estava na resposta, e nenhuma se adivinha. A de sapatilha muda o que a mãe compra **antes** de vir; a de prazo muda se ela marca hoje ou depois das férias |
| **Quando chegar** | (a) e (b) entram na caixa "O que levar"; (c) e (d), na caixa "É paga — e o valor volta" |

## 2. Uniforme e sapatilha

| | |
|---|---|
| **Quem responde** | Secretaria (o que é exigido) + financeiro (onde se compra, quanto custa) |
| **O que precisa vir** | O que é obrigatório por modalidade e por nível, se a escola vende ou indica loja, e a partir de quando é cobrado |
| **Por que trava** | É custo de entrada invisível. Quem descobre depois se sente enganado |
| **Quando chegar** | Nota curta dentro da seção de cada modalidade, ou uma linha na grade por família |

## 3. Espetáculo e calendário

| | |
|---|---|
| **Quem responde** | Coordenação pedagógica |
| **O que precisa vir** | Existe espetáculo de fim de ano? Em que mês? Participar é obrigatório? O figurino é cobrado à parte? Início e fim do ano letivo, e recessos |
| **Por que trava** | Muda o compromisso do ano inteiro, e o figurino é uma despesa real que a família não vê ao se matricular |
| **Quando chegar** | Seção "O ano na Ballance", entre a grade e a localização |

> Existe cobrança de figurino rodando na operação (4 parcelas, dia 13, de julho
> a outubro). Isso confirma que **há** figurino cobrado à parte — mas não diz
> para qual evento, nem se participar é obrigatório. Por isso não está na página.

## 4. Quais níveis fazem exame da Royal Academy of Dance

| | |
|---|---|
| **Quem responde** | Coordenação pedagógica |
| **O que precisa vir** | Quais dos 5 níveis do syllabus (Pre-Primary, Primary, Grade 1, Grade 2, Intermediate Foundation) prestam exame, em que época do ano, e se a inscrição é opcional |
| **Por que trava** | A seção "A Escola" hoje diz a verdade pela metade: separa os 5 degraus com nome do syllabus RAD dos 3 de preparação da casa, e afirma que a escola inscreve alunos no Exame da RAD — mas **não diz quem faz o exame**, porque isso não está confirmado |
| **O que se sabe** | A operação cobra "Parcela 1/2 do Exame da Royal Academy of Dance" com vencimento em maio e junho de 2026, a partir de uma aba própria de planilha. Prova que o exame acontece; não diz de quais turmas |
| **Quando chegar** | Cada degrau da escada ganha "termina em exame" ou "preparação"; hoje o selo diz apenas de quem é o nome do nível |

> **A palavra "certificação" saiu da página em 17/08/2026.** Ela aparecia sem
> qualificador nenhum em toda superfície que o Google indexa e o WhatsApp
> mostra no preview do link — meta description, og:description, og:image:alt,
> JSON-LD, badge do herói e o rodapé. "Certificação Royal Academy of Dance" afirma uma
> **credencial da escola**, e o lastro que existe é outra coisa: a escola usa
> os nomes do syllabus da RAD nos níveis de ballet (a aba TURMAS prova) e
> inscreve alunos no Exame da RAD (a cobrança de 2026 prova). Nenhuma das
> duas equivale a ser registrada ou certificada pela RAD.
>
> Todas passaram a dizer **"ballet no syllabus da Royal Academy of Dance"** —
> que é exatamente o que se prova, e continua sendo a coisa mais forte que a
> escola tem a dizer. O verificador reprova se "certificação Royal Academy"
> voltar ao texto publicado.
>
> **Se a escola for mesmo registrada na RAD, isto vira uma pendência de
> resposta curta:** peça à direção o número de registro ou o certificado. Com
> o documento na mão a palavra volta — e volta com o número junto.

## 5. Expediente da secretaria

| | |
|---|---|
| **Quem responde** | Secretaria |
| **O que precisa vir** | O horário em que **alguém atende** — não o horário em que há aula |
| **Por que trava** | A página mostra hoje as faixas em que existe aula na grade, com a ressalva "faixas em que há aula". Quem quer visitar não sabe se vai achar alguém |
| **Quando chegar** | O `<dl class="loc-horas">` passa a ter as duas colunas (aula / atendimento) e o `openingHoursSpecification` passa a ser o do atendimento |

> **O CEP saiu desta lista em 17/08/2026** — resolvido, e está na página. É
> `13049-252`, conferido em duas fontes independentes: a geocodificação do
> endereço pelo Google e a base dos Correios via ViaCEP, que lista esse CEP para
> a Av. Dermival Bernardes Siqueira no Swiss Park. Está no endereço visível e no
> `postalCode` do JSON-LD.

> O `openingHoursSpecification` do JSON-LD hoje declara **as faixas de aula**, e
> só. Quando o expediente vier, ele substitui isso — é o que o Google mostra
> como "horário de funcionamento", e hoje está tecnicamente certo e
> praticamente enganoso.

## 6. Fotos da escola, e o Instagram

| | |
|---|---|
| **Quem responde** | Direção |
| **O que precisa vir** | 6 a 9 fotos com autorização de uso de imagem — sala, barra, espelho, aula acontecendo — **sem rosto identificável de aluno menor**, salvo autorização assinada |
| **Por que trava** | Havia uma seção "Siga nosso Movimento" com rótulo, título, subtítulo e um botão — e **nenhuma foto**. Um convite para ver o dia a dia sem nada para ver. Foi removida; o @ continua no rodapé |
| **Quando chegar** | A seção volta, com as fotos. E a **primeira** troca é a do herói, não a seção nova |

> **A foto do herói é banco de imagem** — uma bailarina profissional num
> ciclorama branco — e até 01/09/2026 o `alt` dela afirmava "durante aula na
> Ballance Escola de Dança". A página declarava que uma foto comprada era uma
> aula daqui: era isso que o leitor de tela lia em voz alta e o Google
> indexava. O `alt` agora descreve só o que está no quadro. A imagem em si
> continua sendo a comprada, e é a primeira que sai quando as fotos reais
> chegarem — aí o `alt` volta a poder dizer onde ela foi feita.

---

## Coisas que a página deliberadamente **não** vai ter

Não são pendências. São decisões, e ficam registradas para não voltarem como
sugestão a cada rodada.

- **Preço, em qualquer forma** — ver D1. Nem valor, nem "a partir de", nem faixa.
- **Idade em anos** — ver D2. A página fala em Baby, Infantil, Juvenil e Adulto,
  que é como a escola fala; o encaixe é confirmado por uma pessoa, na visita.
- **Nome de professor** — em nenhum lugar: texto, `aria-label`, atributo,
  texto pré-montado de `wa.me`, placeholder, meta tag, JSON-LD, comentário de
  código. Os professores
  são PJ; nome de pessoa ao lado de dia e horário fixos é vínculo aparente, e
  ninguém consentiu em ter o nome numa página pública. Se alguém pedir, a
  resposta é não — esse dado pertence à conversa, não ao HTML.

  > **Isto já foi só uma promessa, e a promessa falhou duas vezes.** Até
  > 17/08/2026 este documento e o cabeçalho do `index.html` afirmavam que o
  > índice da busca estava limpo, enquanto duas linhas publicavam o primeiro
  > nome de um professor num atributo `data-busca` escrito à mão. Não era
  > resíduo invisível: o filtro da grade casava o que se digitava contra esse
  > atributo, então **buscar esse nome no site público devolvia as duas turmas
  > dele, com dia e hora fixos** — exatamente a peça que a blindagem PJ existe
  > para não produzir. Sobrou também um `", e"` no meio da string, marca de
  > uma lista de três nomes apagada à mão.
  >
  > Em 27/08/2026 o atributo deixou de existir. O índice da busca é **derivado
  > em JavaScript do que a linha já publica** — nome, hora, dias, frequência,
  > mais o título da família e os dias por extenso que o filtro já lê em
  > `data-dias`. Índice montado a partir do texto visível não tem como
  > carregar o que a página não publica; escrito à mão, tinha.
  >
  > **A segunda falha foi deste lado.** Este documento afirmava que a lista de
  > nomes "não está versionada em lugar nenhum" — e o primeiro nome de uma
  > pessoa do cadastro estava, em texto puro, num comentário de
  > `site/grade_publica.py`. O nome saiu, e a frase deixou de ser promessa:
  > o bloco [1] de `02-automacoes-python/site/verificar_site.py` varre
  > `index.html`, **este arquivo**, `grade_publica.py` e o próprio
  > `verificar_site.py` atrás do primeiro nome e do sobrenome de todo
  > professor do cadastro — texto, atributo, comentário, CSS, `wa.me` com
  > percent-encoding desfeito — e sai com erro se achar um. A lista continua
  > saindo da planilha na hora: uma lista de nomes commitada seria o mesmo
  > vazamento com outra roupa.
- **Número de alunos, ano de fundação, prêmio, depoimento** — nada disso está
  confirmado, e número de vaidade inventado é a coisa mais fácil de desmentir.
- **Número da sala** — não existe na fonte.
- **Tarja "a confirmar" na página** — é o que este arquivo existe para evitar.
  Estrutura vazia esperando dado não é entrega; é dívida com cara de recurso.

---

## A página é derivada. Rode o verificador.

O `index.html` não é um texto: é um **relatório da aba TURMAS**, escrito à mão.
As 54 turmas, os 8 contadores de família (cada um dito duas vezes — no
cabeçalho da grade e no cartão da modalidade), os 8 degraus da escada, as
faixas de funcionamento dos 6 dias e o total repetido em oito superfícies são
~30 asserções que saem todas da mesma planilha. Uma turma que mude de horário
lá não quebra nada aqui — ela só transforma todas essas frases em mentira,
**em silêncio**, para quem chegou pelo Google.

```
cd 02-automacoes-python && python3 site/verificar_site.py
```

Ele lê a aba TURMAS, deriva a grade pública de novo e confronta com o HTML:
turma por turma (nome, dias, hora de início e de fim, `data-dias`,
`data-adulto`, frequência, texto do `wa.me` e `aria-label`), contador por
contador — no cabeçalho da família **e** no cartão da modalidade —, degrau por
degrau (selo, contagem e dias), faixa por faixa no `<dl>` visível **e** no
JSON-LD, que é o que o Google publica como horário de funcionamento. Confere
ainda que nenhuma cor da marca foi reescrita fora do `:root`, que nenhum link
interno cai no vazio, que nenhum ícone sobra sem uso, e aplica as regras da
Parte I também no que ninguém lê na tela — meta tags e
JSON-LD, que é onde "certificação" morou mais tempo. Mais a varredura de nome
de professor, nele e neste arquivo. Sai com código 1 quando diverge, e diz o
que mudou dos dois lados. Rode depois de mexer na página **e** depois de mexer
na planilha.

```
python3 site/verificar_site.py --automutacao
```

Este segundo modo é a prova de que o primeiro presta: ele estraga a página de
32 jeitos diferentes (em memória, nunca em disco) — planta o primeiro nome de
um professor num `aria-label`, cega a própria varredura de nomes, muda o
horário de uma turma, troca o dia no atributo que o filtro lê, marca turma
infantil como de adulto, infla um contador de família, faz um degrau da casa
se dizer RAD, estica a faixa de sábado no `<dl>` e no JSON-LD, esconde um
preço só na meta description, devolve "certificação" ao og:description,
reescreve uma cor da marca fora da paleta, devolve o horário de término e a
ressalva do funcionamento a um cinza ilegível, quebra uma âncora, apaga o nome de
uma linha para ver se a leitura percebe que ficou cega — e estraga **também este documento**, envelhecendo uma contagem e
mentindo sobre o próprio número de mutações. Exige que o verificador reprove
em cada um. Trava que não falha quando o defeito volta é decoração; este modo
é o que impede a trava de virar decoração sem ninguém notar.

**O que o verificador não faz:** ele confere o que a página AFIRMA contra a
planilha. Ele não sabe se falta alguma coisa na página — isso é o que a lista
acima existe para lembrar.

---

## Como usar isto

Cada item da **Parte II** é uma mensagem pronta. O caminho mais curto é levar um
por vez a quem responde. A **aula experimental**, que era o primeiro da fila, foi
respondida em 01/09/2026 e está no ar; do item 1 sobraram quatro pontas curtas,
que cabem numa única pergunta à secretaria. A partir daí a ordem que rende mais é
**uniforme** — é custo de entrada invisível, e quem descobre depois se sente
enganado.

Quando uma resposta chegar, ela entra como **conteúdo** — e o item sai daqui.

**Os itens da Parte I não entram nessa fila.** Não leve D1 (preço) nem D2 (idade
em anos) a ninguém: eles não estão esperando resposta, foram decididos. Se a
decisão mudar um dia, quem muda é a direção, e aí muda também o bloco [7] do
`verificar_site.py` — que hoje reprova a página se qualquer um dos dois
aparecer.
