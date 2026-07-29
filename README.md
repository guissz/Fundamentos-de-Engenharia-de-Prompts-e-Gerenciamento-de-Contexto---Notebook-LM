# Fundamentos de Engenharia de Prompts e Gerenciamento de Contexto - Notebook-LM

Projeto desenvolvido como desafio prático do Bootcamp Bradesco | DIO - GenIA, Dados e Cyber

## Sobre o Projeto

Este repositório reúne a documentação do meu Caderno Temático desenvolvido utilizando o **NotebookLM**, com foco em **Fundamentos da Engenharia de Prompt e Gerenciamento de Contexto**.

O objetivo deste projeto é consolidar os conhecimentos adquiridos durante o módulo de Inteligência Artificial Generativa por meio da curadoria de conteúdos, elaboração de prompts estratégicos e produção de um material de estudo reutilizável.

---

## Objetivos de Estudo

- Compreender os funcionamentos da Engenharia de Prompt;
- Entender a importância do gerenciamento de contexto em modelos de IA.
- Aprender boas práticas para escrever prompts mais eficientes.
- Explorar diferentes estratégias de interação com LLMs.
- Produzir um guia de consulta para estudos futuros.

---

## Tecnologias e Ferramentas Utilizadas

- NotebookLM
- GitHub
- Markdown
- Modelos de Linguagem (LLMs)

---

## Principais Fontes

| Fonte | Tipo | Link |
|-------|------|------|
| Engenharia de comandos: visão geral e guia | Documentação | https://cloud.google.com/discover/what-is-prompt-engineering |
| COSTAR Prompt Engineering: What It Is and Why It Matters | Artigo | https://portkey.ai/blog/what-is-costar-prompt-engineering/ |
| O que é engenharia de prompts? | Artigo | https://www.ibm.com/br-pt/think/topics/prompt-engineering |
| Engenharia de Contexto: A Chave para Construir Agentes de IA que Realmente Funcionam (com exemplos) | Vídeo | https://www.youtube.com/watch?v=aMJUnOeOs2k |
| Engenharia de Prompt: O Guia Definitivo | Vídeo | https://www.youtube.com/watch?v=1VDcke66TRE |

---

## Processo de Aprendizagem

### Estratégia de Estudo

Durante o desenvolvimento do meu Caderno Temático, eu reuni diversas fontes de conteúdo que englobam o tema principal para me auxiliar à obter informações relevantes sobre o tema. Após isso formulei algumas perguntas e desafios para a ferramenta que fossem capazes de satisfazer as minhas principais dúvidas.

---

## Engenharia de Prompts

Nesta seção estão registrados os principais prompts utilizados durante o estudo.

### Prompt 1

O objetivo deste Prompt era obter um exemplo de como seria uma estrutura ideal para reunir informações autênticas e concretas para um livro ambientado na Grécia Antiga, para isto, pedi que a IA se passasse por um usuário consultando uma outra IA sobre o problema em questão.

**Prompt Utilizado:**

```
Me dê um exemplo de um prompt bem estruturado para resolver o seguinte problema: Imagine que você esteja escrevendo um livro ambientado na Grécia Antiga e precisa reunir algumas informações relevantes. Para isso, você pede à uma IA te trazer uma lista de tópicos sobre como era a sociedade naquela época, quais eram suas crenças e como era a sua cultura.
Separe o prompt por estruturas, detalhando exatamente a técnica utilizada na construção do mesmo.
```

**Resultado Obtido:**

```
Para resolver o seu problema de pesquisa para um livro sobre a Grécia Antiga, um prompt bem estruturado deve ir além de uma pergunta simples. Utilizando as diretrizes de frameworks como CO-STAR, RISEN e os 5 Pilares do Google, aqui está um exemplo de prompt otimizado:
Exemplo de Prompt Estruturado
[Contexto]: Estou escrevendo um romance histórico ambientado na Grécia Antiga, especificamente no século V a.C. (Período Clássico). Preciso de informações autênticas para construir o mundo e a ambientação da história
.
[Persona]: Aja como um historiador acadêmico especialista em Antiguidade Clássica, com foco em vida cotidiana, antropologia cultural e história das religiões
.
[Tarefa/Objetivo]: Elabore uma lista abrangente de tópicos essenciais sobre a sociedade, as crenças e a cultura daquela época. Foque em três pilares:
Sociedade: Classes sociais, o papel das mulheres e a rotina dos escravos.
Crenças: Rituais domésticos, a importância dos oráculos e a relação prática com os deuses.
Cultura: Vestuário, festivais públicos e hábitos alimentares
.
[Formato]: Entregue o conteúdo usando Markdown. Utilize cabeçalhos (##) para as categorias principais e listas com marcadores para os tópicos. Para cada item da lista, adicione uma frase explicando um detalhe sensorial que seria útil para a escrita de um livro
.
[Restrições/Narrowing]: Utilize apenas fatos históricos precisos e evite anacronismos. Se houver divergências entre cidades-estado (como Atenas vs. Esparta), destaque brevemente essa diferença
.
Detalhamento das Técnicas Utilizadas
A construção deste prompt baseia-se em princípios fundamentais da engenharia de prompt para garantir que a IA não gere respostas genéricas ou "alucine" fatos
.
Context Injection (Injeção de Contexto): Ao especificar que o livro é no século V a.C., você "vetora" a IA para um período específico, evitando que ela misture informações do período micênico ou helenístico
.
Role Prompting (Método da Persona): A instrução "Aja como um historiador" ativa no modelo um subconjunto de dados mais técnico e acadêmico, elevando o nível de vocabulário e a precisão dos detalhes históricos
.
Task Clarity (Clareza de Tarefa): O uso de verbos de ação claros como "Elabore" e a divisão em tópicos numerados ajuda a IA a processar a instrução como um comando direto, reduzindo a ambiguidade
.
Output Structure (Estruturação de Saída): Solicitar o formato Markdown e cabeçalhos específicos garante que a resposta seja organizada e pronta para uso em ferramentas de escrita, como o Obsidian ou editores de texto
.
Narrowing (Restrições de Escopo): Definir o que a IA deve evitar (anacronismos) e o que deve focar (detalhes sensoriais e diferenças entre cidades-estado) atua como um trilho de segurança, impedindo que o modelo se perca em informações irrelevantes
.
Positive Instructions (Instruções Positivas): O prompt diz exatamente o que deve ser feito (ex: "destaque as diferenças"), o que é processado de forma muito mais estável pelos modelos do que comandos negativos ("não faça tal coisa")
```

### Prompt 2

Para a estruturação do Prompt a seguir, utilizei a resposta do anterior como base. Neste, eu gostaria de saber mais e me aprofundar sobre Engenharia de Prompt, por isso utilizei o modelo da resposta passado anteriormente para obter informações relevantes.

**Prompt Utilizado:**

```
Quero saber mais sobre o que Engenharia de Prompt, para que ela serve, quais são suas principais vantagens e quais são os principais métodos utilizados para a estruturação de um bom prompt.
Para isto, aja como um engenheiro de prompt profissional que tenha um ótimo conhecimento sobre o tema e com anos de experiência no mercado. Imagine que este engenheiro esteja explicando o conceito para uma pessoa totalmente leiga no assunto.
Elabore um resumo que explique detalhadamente cada um dos tópicos a seguir:

1. Qual é o conceito da Engenharia de Prompt.

2. Como se descobriu a melhor maneira de escrever um bom prompt que atenda a necessidade do usuário.

3. Quais são os principais métodos utilizados na construção de um bom prompt.

4. As principais vantagens de aplicar a Engenharia de Prompt à ferramentas de IA mesmo quando a solicitação do usuário não seja algo tão complexo.

Entregue o resultado em um formato de texto com o máximo de 6 parágrafos, e para cada item que foi passado como parâmetro, dê um exemplo de aplicação.
```

**Resposta Obtida:**

```
A Engenharia de Prompt é a disciplina técnica de desenvolver, otimizar e avaliar instruções textuais para direcionar o comportamento de modelos de linguagem de grande escala (LLMs)
. Imagine-a como um "mapa" ou roteiro que guia a inteligência artificial para que ela entenda sua real intenção e responda de forma útil e precisa
. Diferente de uma simples barra de pesquisa, tratamos a IA como uma ferramenta de raciocínio, onde o engenheiro atua reduzindo a incerteza do modelo para que ele gere saídas altamente alinhadas às expectativas de formato e tom
. Aplicação: Em vez de pedir apenas "ideias de marketing", um engenheiro diria: "Aja como um estrategista de redes sociais especializado em B2B e crie 5 conceitos de posts para LinkedIn focados em geração de leads"
.
No início, a interação com IAs era baseada puramente em tentativa e erro intuitivo
. Contudo, a Engenharia de Prompt consolidou-se como ciência quando pesquisadores descobriram que pequenos ajustes estruturais ativavam capacidades latentes de raciocínio nos modelos
. Descobriu-se, por exemplo, que incluir a frase "Vamos pensar passo a passo" (método Zero-shot CoT) forçava a IA a realizar ciclos de planejamento interno, eliminando até 80% das alucinações em tarefas complexas
. Aplicação: Se a IA falha ao resolver um enigma, você pode "destravar" o raciocínio dela instruindo: "Resolva este problema pensando passo a passo em um bloco oculto antes de me dar a resposta final"
.
Para garantir previsibilidade e consistência, utilizamos frameworks que funcionam como "receitas" para prompts
. O método CO-STAR (Contexto, Objetivo, Estilo, Tom, Audiência e Resposta) é o padrão de ouro para comunicações de marketing e negócios por separar a estrutura visual (Estilo) da qualidade emocional (Tom)
. Outro método essencial é o RISEN, focado em tarefas procedurais, onde definimos claramente o Papel (Role), Instruções, Passos (Steps), Meta Final e as Restrições (Narrowing)
. Aplicação: Para criar um anúncio, usaria o CO-STAR definindo que a [Audiência] são diretores de tecnologia e o [Tom] deve ser autoritativo, mas amigável
.
A técnica de Few-shot Prompting é um dos métodos mais poderosos para estruturação, consistindo em fornecer de 3 a 8 exemplos reais de "pergunta e resposta" dentro do próprio prompt
. Isso calibra o comportamento da IA e garante que ela entenda padrões de dados específicos de uma empresa que não estavam em seu treinamento original
. Somado a isso, o Role Prompting fixa a IA em uma identidade especialista, fechando a janela de contexto apenas para o conhecimento técnico necessário
. Aplicação: Para formatar relatórios, forneça dois [Exemplos] de relatórios anteriores para que a IA aprenda a estrutura visual e o vocabulário técnico exigido
.
Mesmo em solicitações simples, aplicar Engenharia de Prompt traz vantagens cruciais: ela otimiza custos ao reduzir o uso desnecessário de "tokens" e evita que a IA se distraia com informações irrelevantes em conversas longas
. Além disso, garante escalabilidade, permitindo que diferentes membros de uma equipe usem o mesmo prompt padronizado para obter resultados idênticos de alta qualidade, sem precisar de reedição manual
. Aplicação: Ao pedir um resumo de e-mail, um prompt estruturado garante que a IA sempre entregue uma [Tabela] com Decisões e Prazos, economizando o tempo que você gastaria reorganizando um texto corrido
.
Em última análise, a Engenharia de Prompt é a ponte entre a programação tradicional e a orquestração de sistemas inteligentes
. Dominar essa habilidade transforma a IA de um simples chatbot em um "funcionário virtual" eficiente, capaz de automatizar processos, analisar dados complexos em linguagem natural e aumentar a produtividade organizacional em até 70%
. Aplicação: Para treinar um novo vendedor, você pode criar um [Agente] com regras estritas de engajamento, simulando um cliente difícil que só aceita a venda se argumentos específicos forem usados
.
```

---

## Trubleshooting ("Cicatrizes")

O principal problema que eu tive durante o desenvolvimento foi justamente não ter conhecimento algum sobre uma boa estruturação para um Prompt. Como já utilizava ferramentas de IA há algum tempo, estava acostumado a escrever perguntas, solicitações e instruções genéricas que acabavam resultando em respostas genéricas e algumas vezes até fora de contexto.

Com o auxílio do curso da DIO e das anotações do Notebook LM, fui capaz de pensar em instruções melhores que acabaram por resolver algumas dúvidas e problemas que eu tinha. Dentro da própria ferramenta utilizei modelos de Prompt que trouxeram respostas condizentes e coesas ao que eu havia solicitado.

## Miniguia de Estudos

---

### Resumo Estruturado

A Engenharia de Prompt é a disciplina técnica de desenvolver, otimizar e avaliar instruções textuais para guiar modelos de inteligência artificial (LLMs) em direção a resultados precisos e úteis
. Imagine a IA como o estagiário mais inteligente do mundo, que leu todos os livros, mas não possui experiência de vida ou contexto sobre sua necessidade específica; sem instruções claras, ela tende a fornecer respostas genéricas ou até inventar fatos, fenômeno conhecido como alucinação
. Essa prática funciona como uma "ponte" entre a linguagem natural humana e a lógica computacional, reduzindo a incerteza do modelo e permitindo que ele funcione não apenas como um buscador, mas como uma ferramenta de raciocínio capaz de melhorar o desempenho em tarefas complexas em até 70%
.
Para estruturar um bom prompt, profissionais utilizam frameworks que servem como "receitas", como o CO-STAR (focado em estilo, tom e audiência) ou o RISEN (ideal para tarefas técnicas e processos sequenciais)
. As principais técnicas incluem o Role Prompting, onde se atribui uma identidade à IA (ex: "Aja como um historiador"), o Few-shot Prompting, que consiste em fornecer exemplos práticos antes do comando, e a Cadeia de Pensamento (CoT), que instrui o modelo a "pensar passo a passo" para resolver problemas lógicos
. Mesmo em solicitações simples, aplicar esses métodos traz vantagens cruciais: otimiza o uso de tokens (reduzindo custos), garante que a IA não se perca em conversas longas e permite a criação de agentes — funcionários virtuais que seguem regras estritas para automatizar processos com consistência e segurança
.

---

## Glossário

### Fundamentos e Conceitos Básicos

LLM (Modelo de Linguagem de Grande Escala): É o "cérebro" da IA. Um modelo treinado com milhões de livros e textos para entender padrões de linguagem e prever a próxima palavra mais provável em uma frase

Prompt: É a instrução ou pergunta que você envia para a IA. É o ponto de partida que define o que o modelo deve fazer

Token: A menor unidade de texto que a IA processa. Pode ser uma palavra, parte dela ou até um sinal de pontuação. A IA não lê palavras como nós, ela lê "fatias" chamadas tokens

Janela de Contexto (Context Window): É o limite de "memória de curto prazo" da IA durante uma conversa. Se a conversa ficar longa demais e ultrapassar esse limite, a IA começa a esquecer as primeiras mensagens

Stateless (Sem Estado): Significa que, nativamente, a IA não tem memória própria entre sessões. Cada vez que você abre um novo chat, ela é uma "folha em branco" e precisa que você forneça o contexto novamente

Alucinação: Quando a IA gera informações que parecem verdadeiras, mas são inventadas. Isso geralmente acontece por falta de contexto ou instruções vagas.

### Técnicas de Estruturação

Persona / Role Prompting: Técnica de atribuir um papel ou identidade à IA (ex: "Aja como um advogado"). Isso ajuda o modelo a filtrar o vocabulário e o tom corretos para a tarefa

Zero-shot: Quando você pede algo diretamente, sem dar nenhum exemplo anterior

Few-shot: Quando você fornece alguns exemplos (de 3 a 8) de "pergunta e resposta" antes de fazer o seu pedido real, para que a IA aprenda o padrão desejado

Cadeia de Pensamento (Chain-of-Thought - CoT): Instruir a IA a "pensar passo a passo". Isso força o modelo a realizar um raciocínio lógico antes de entregar a resposta final, o que reduz erros em tarefas complexas

Delimitadores: Símbolos como ###, """ ou tags XML (<instrução></instrução>) usados para separar claramente onde termina uma ordem e onde começa um texto que você quer que ela analise


### Frameworks (Modelos estruturados)

CO-STAR: Focado em comunicação e marketing. Divide o prompt em: Contexto, Objetivo, Stilo, Tom, Audiência e Resposta

RISEN: Focado em tarefas técnicas e processos. Divide o prompt em: Role (Papel), Instruções, Steps (Passos), End Goal (Meta Final) e Narrowing (Restrições)

### Parâmetros Técnicos e Avançados

Temperatura: Um "botão" que regula a criatividade. Perto de 0, a IA é factual e direta; acima de 0.7, ela se torna mais criativa e aleatória

RAG (Geração Aumentada de Recuperação): Técnica que permite à IA consultar "livros externos" (como seus PDFs ou manuais da empresa) em tempo real para responder com fatos atualizados, em vez de depender apenas do seu treinamento original

Modelos Deliberativos (Reasoning Models): Nova geração de IAs (como o OpenAI o1) que possuem um "raciocínio profundo" nativo, planejando a resposta internamente antes de começar a escrever

---

## Biblioteca de Prompts

### Explicar um conceito

```
[Persona]: Aja como um [ESPECIALISTA NO ASSUNTO] com foco em educação e didática simples
.
[Contexto]: O objetivo é explicar o conceito de [CONCEITO] para uma audiência de [PÚBLICO-ALVO: ex. Iniciantes/Executivos], que possui pouco conhecimento prévio sobre o tema
.
[Tarefa]: Forneça uma explicação clara e abrangente. Utilize uma analogia do mundo real para facilitar a compreensão
.
[Formato]: Estruture a resposta em Markdown com os seguintes títulos: 1) O que é (em uma frase), 2) Analogia prática, 3) Como funciona e 4) Por que é importante
.
[Restrição]: Evite jargões técnicos excessivos. Se precisar usar um termo complexo, defina-o brevemente entre parênteses
.
```

### Criar um resumo

```
Ação: Resuma o conteúdo delimitado pelas triplas aspas abaixo
.
Propósito: Preciso de uma visão geral de [TEMPO: ex. 2 minutos] para me preparar para uma [SITUAÇÃO: ex. Reunião de liderança/Prova]
.
Expectativa: Identifique os 5 pontos principais e entregue-os em uma lista com marcadores (bullets). Ao final, inclua uma seção de "Próximos Passos" ou "Principais Conclusões"
.
Conteúdo: """ [COLE O TEXTO AQUI] """
```

### Comparar conceitos

```
[Role]: Você é um Analista Estratégico com anos de experiência em [ÁREA DO CONHECIMENTO]
.
[Instructions]: Compare tecnicamente o [CONCEITO A] com o [CONCEITO B]
.
[Steps]:
Defina brevemente cada conceito
.
Identifique 3 semelhanças fundamentais
.
Destaque as 3 principais diferenças em termos de aplicação e custo
.
Conclua indicando qual é mais recomendado para [CASO DE USO ESPECÍFICO]
.
[End Goal]: O resultado final deve permitir uma tomada de decisão rápida e informada
.
[Narrowing]: Apresente a comparação técnica exclusivamente em uma Tabela Markdown para facilitar a visualização
.
```

### Gerar questões

```
[Contexto]: Acabamos de estudar o material sobre [ASSUNTO]. Sou um instrutor que precisa validar o conhecimento da turma
.
[Objetivo]: Gere um conjunto de questões que desafiem a compreensão profunda e o raciocínio lógico dos alunos
.
[Estilo/Tone]: Use um estilo acadêmico, porém encorajador. O tom deve ser profissional e imparcial
.
[Audiência]: Estudantes de nível [NÍVEL: ex. Superior/Certificação Técnica], que já dominam os fundamentos
.
[Resposta]: Forneça 5 questões de múltipla escolha com 4 alternativas cada. Importante: Inclua o gabarito justificado em uma seção oculta ou ao final, explicando por que a alternativa correta está certa com base no conteúdo
.
```

---

## Principais Aprendizados

Ao final deste projeto foi possível:

- Compreender melhor a Engenharia de Prompt;
- Aprender técnicas de gerenciamento de contexto;
- Melhorar a qualidade das perguntas feitas para LLMs;
- Desenvolver pensamento crítico sobre respostas geradas por IA;
- Construir um material de consulta permanente.
