# Plano de Execução — Provérbios para a Vida v2

> Status: planejamento fechado. Este documento define a execução futura das 31 aulas. Durante a elaboração deste plano, nenhum conteúdo adicional das aulas deve ser alterado.

## 1. Objetivo da reforma

Atualizar as 31 lições de **Provérbios para a Vida** para um padrão pedagógico único, teologicamente responsável e apropriado para crianças de 7–12 anos, preservando a publicação estática existente no GitHub Pages.

A reforma deve melhorar conteúdo e experiência de ensino sem transformar o projeto em uma refatoração de software.

## 2. Fonte de verdade

A fonte editorial da reforma é:
1. conteúdo atual de cada capítulo no repositório;
2. `MODELO_PEDAGOGICO_V2.md`, incluindo a matriz individual das 31 aulas;
3. padrão de profundidade e organização aprovado nas Lições 8 e 9.

Nenhuma aula será gerada apenas a partir do título. O conteúdo atual deve ser preservado quando estiver correto e reescrito quando houver ganho exegético, pedagógico ou pastoral.

## 3. Contrato editorial de uma aula

Cada aula deve possuir, de forma coerente entre os materiais:

### Núcleo
- número e capítulo;
- título;
- grande ideia em linguagem memorizável;
- texto(s)-base;
- versículo-chave;
- pergunta-chave;
- frase para repetir;
- objetivo cognitivo: o que compreender;
- objetivo afetivo: o que valorizar;
- objetivo prático: o que praticar.

### Guia do professor
1. visão geral;
2. preparação do professor;
3. contexto literário;
4. explicação dos textos escolhidos;
5. termos/conceitos que precisam de definição;
6. cuidado exegético;
7. cuidado pastoral;
8. conexão canônica e evangelho;
9. roteiro completo de 55–60 minutos;
10. abertura;
11. desenvolvimento em 3–5 movimentos;
12. perguntas durante a exposição;
13. dinâmica principal;
14. aplicações concretas;
15. perguntas finais;
16. memorização;
17. desafio semanal/familiar;
18. oração;
19. erros a evitar;
20. cola de 30 segundos.

### Roteiro de aula
Documento operacional para quem já estudou o guia:
- cronograma;
- materiais necessários;
- falas/transições essenciais;
- textos a ler;
- perguntas;
- instruções da dinâmica;
- fechamento no evangelho;
- oração;
- lembrete do desafio.

### Resumo rápido
Uma página para consulta imediatamente antes da aula:
- grande ideia;
- versículo;
- pergunta;
- 3 movimentos;
- dinâmica;
- evangelho;
- aplicação;
- erros críticos;
- duração.

### Desafio da semana
Uma folha infantil/familiar:
- versículo;
- desafio observável e específico;
- espaço de registro;
- oração curta;
- atividade familiar;
- pergunta para conversar com pais/responsáveis;
- atividade criativa quando útil.

O desafio não deve ser uma cópia genérica com o título da aula substituído.

## 4. Regra de linguagem por público

### Professor
Pode receber termos como literatura sapiencial, personificação, soberania, santificação, justificação e contexto canônico, desde que explicados quando necessário.

### Criança
Preferir frases curtas, situações concretas e imagens do próprio texto. Termos teológicos importantes podem permanecer, mas precisam ser explicados em linguagem acessível.

Faixa-base: **7–12 anos**. Para perguntas/dinâmicas, sempre que fizer sentido:
- opção simples: 7–9;
- aprofundamento: 10–12.

## 5. Regra exegética

- O tema precisa nascer do capítulo.
- Provérbios são sabedoria, não contratos mecânicos de causa e efeito.
- Distinguir descrição geral de promessa absoluta.
- Não transformar toda personificação da Sabedoria diretamente em Jesus.
- Conexões cristológicas devem preferir textos explícitos do NT ou relações canônicas justificáveis.
- Não importar para o versículo um significado popular que o contexto não sustenta.
- Quando a aplicação extrapolar o sentido imediato, identificá-la como aplicação/conexão, não como significado original.

## 6. Regra do evangelho

Cada aula deve evitar dois extremos:
1. moralismo: “faça isso e seja uma criança boa”;
2. conexão artificial: inserir Jesus sem relação compreensível com a verdade ensinada.

Fluxo preferido:
**verdade de Deus → nossa necessidade/pecado → graça/obra de Cristo → resposta de fé e obediência pelo Espírito.**

Nem toda aula precisa usar exatamente as mesmas frases ou os mesmos textos cristológicos.

## 7. Salvaguardas infantis

Especialmente nas aulas sobre autoridade, amizade, conflito, perdão, humildade e coragem:
- não ensinar criança a ocultar abuso, ameaça ou toque inadequado;
- não confundir perdão com permanecer em perigo;
- não exigir reconciliação imediata em situação insegura;
- não tratar obediência a autoridade como absoluta quando há ordem pecaminosa/perigosa;
- incentivar procura de pais/responsáveis/líder adulto seguro;
- não usar culpa ou medo como técnica de controle;
- não apresentar sofrimento como evidência automática de que Deus está punindo ou “refinando” especificamente um pecado.

## 8. Identidade visual

Manter a identidade já estabelecida:
- verde escuro;
- dourado;
- creme;
- Playfair Display + Inter no site;
- visual mais lúdico apenas no Desafio da Semana;
- responsividade e controles atuais de fonte.

A reforma não migrará o site para React/Next.js e não criará dependência de backend.

### Melhorias permitidas
- uniformizar cabeçalhos;
- uniformizar cartões/blocos;
- melhorar hierarquia visual;
- incluir indicadores “Essencial” e “Aprofunde”;
- melhorar impressão;
- corrigir duplicação visual evidente quando isso puder ser feito sem aumentar o risco.

## 9. Arquivos-alvo

Por lição:
- `licoes/licao-NN.html`
- `guia-professor/leitura/Licao_NN.html`
- `roteiro-aula/leitura/Licao_NN.html`
- `resumo-rapido/leitura/Licao_NN.html`
- `desafio-semana/leitura/Licao_NN.html`

Total editorial HTML: **155 arquivos**.

Além disso:
- `index.html`;
- PDFs correspondentes;
- documentação e scripts auxiliares, se necessários.

## 10. Estratégia de produção

### Etapa A — conteúdo canônico por aula
Antes de montar HTML, criar internamente para cada lição um objeto editorial contendo todos os campos do contrato. Esse objeto impede divergências entre guia, roteiro, resumo e desafio.

### Etapa B — geração dos cinco materiais
A partir do mesmo conteúdo canônico:
- página da lição apresenta os quatro materiais;
- guia recebe versão completa;
- roteiro recebe versão operacional;
- resumo recebe condensação;
- desafio recebe aplicação infantil/familiar.

### Etapa C — PDFs
Os PDFs devem refletir as versões de leitura. Não manter conteúdo diferente em PDF e HTML.

Sempre que possível, usar uma geração determinística para que futuras correções não exijam editar HTML e PDF manualmente em separado.

## 11. Estratégia de commits

Não criar 155 commits.

Sugestão:
1. `content: implementa lições 01-08 no modelo v2`
2. `content: implementa lições 09-16 no modelo v2`
3. `content: implementa lições 17-24 no modelo v2`
4. `content: implementa lições 25-31 no modelo v2`
5. `build: atualiza PDFs das 31 lições`
6. `qa: corrige navegação e inconsistências da série v2`
7. `docs: registra conclusão da migração pedagógica v2`

O conteúdo pode ser preparado em lote e publicado nesses grupos para facilitar revisão e rollback.

## 12. Ordem de execução

1. congelar títulos, capítulos, grandes ideias e perguntas-chave;
2. preparar conteúdo canônico 1–31;
3. revisão de coerência horizontal para detectar duplicações;
4. revisão exegética dos pontos sensíveis;
5. gerar os 155 HTMLs;
6. atualizar `index.html`;
7. gerar PDFs;
8. validar estrutura/links;
9. validar visual em desktop/mobile/print;
10. revisão de conteúdo por amostragem + verificações automatizadas em todas;
11. atualizar PR;
12. somente então retirar Draft.

## 13. Validações automatizadas

Criar/verificar rotinas que falhem quando:
- faltar qualquer número de 01 a 31 em uma das cinco famílias;
- título divergir entre materiais;
- capítulo divergir;
- link de “voltar” quebrar;
- link de PDF apontar para arquivo inexistente;
- houver referência a título antigo da Lição 9;
- faltar versículo-chave;
- faltar grande ideia;
- faltar desafio;
- HTML tiver estrutura essencial incompleta;
- index não listar exatamente 31 aulas;
- houver caminho local/temporário inserido por engano.

## 14. Validação editorial

Checklist por aula:
- [ ] tema sustentado pelo capítulo;
- [ ] grande ideia compreensível;
- [ ] versículo-chave realmente relacionado;
- [ ] professor recebe contexto suficiente;
- [ ] linguagem infantil não distorce o texto;
- [ ] dinâmica ensina, não apenas diverte;
- [ ] aplicações são concretas;
- [ ] evangelho evita moralismo;
- [ ] conexão com Cristo é justificável;
- [ ] provérbio não virou promessa absoluta;
- [ ] salvaguardas pastorais aplicadas quando pertinentes;
- [ ] guia/roteiro/resumo/desafio não se contradizem.

## 15. Validação visual

Amostra obrigatória:
- Lição 1 — início da série;
- Lição 8 — padrão de referência;
- Lição 9 — conteúdo reconstruído;
- Lição 16 — meio;
- Lição 22 — salvaguarda de autoridade;
- Lição 31 — encerramento.

Em cada amostra:
- desktop;
- largura mobile;
- impressão/PDF;
- fonte aumentada;
- links de navegação.

Depois da amostra, executar verificações estruturais nas 31.

## 16. Pontos de atenção já identificados

- Lição 5: tratar pureza/santidade de forma apropriada à idade.
- Lição 8: não identificar automaticamente a Sabedoria personificada com Cristo.
- Lição 9: Sabedoria × Insensatez; título v2 “Dois Convites, Dois Caminhos”.
- Lição 10 × 11: integridade ≠ honestidade, embora relacionadas.
- Lição 12 × 15: palavras em geral ≠ resposta em conflito.
- Lição 13: autocontrole ≠ repressão emocional.
- Lição 17 × 27: lealdade na dificuldade ≠ amizade que corrige e forma.
- Lição 18/19/22/24: aplicar salvaguardas de segurança infantil.
- Lição 22: Pv 22:6 como princípio sapiencial, não garantia mecânica.
- Lição 25: Pv 25:4–5 — não confundir aplicação de santificação com sentido imediato.
- Lição 28: diligência não garante riqueza.
- Lição 29: Pv 29:18 fala de revelação/instrução divina, não de “ter uma visão de liderança”.
- Lição 30: distinguir palavra de Deus em Pv 30:5 e o Logos de Jo 1 ao fazer conexão canônica.
- Lição 31: preservar o referente feminino do poema sem transformá-lo em checklist de aprovação.

## 17. Critérios para o PR sair de Draft

Todos precisam ser verdadeiros:
- 31/31 conteúdos canônicos revisados;
- 155/155 HTMLs atualizados;
- 31 páginas de lição coerentes com o index;
- PDFs atualizados e acessíveis;
- nenhuma referência antiga indevida à Lição 9;
- validação estrutural sem erro;
- amostra visual aprovada;
- pontos exegéticos sensíveis revisados;
- salvaguardas infantis presentes;
- diff final revisado;
- nenhum merge automático.

## 18. Fora de escopo deste PR

- migrar para Next.js/React;
- banco de dados;
- login;
- painel administrativo;
- CMS;
- analytics;
- gamificação digital;
- reconstrução total da identidade visual;
- merge automático em `main`.

Essas melhorias podem ser projetos posteriores sem misturar risco técnico com a reforma pedagógica.

## 19. Resultado esperado

Ao final, um professor deve conseguir:
1. abrir a aula;
2. estudar profundamente pelo Guia;
3. ministrar usando o Roteiro;
4. consultar o Resumo minutos antes;
5. entregar à criança um Desafio realmente ligado à aula;
6. repetir esse fluxo nas 31 semanas com a mesma lógica.

A criança deve perceber uma única jornada: **começar aprendendo que o temor do Senhor é o princípio da sabedoria (Pv 1:7) e terminar vendo o retrato de uma vida formada por esse temor (Pv 31:30).**
