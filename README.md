# Skills para o grupo de estudos

Este diretório reúne três skills para apoiar estudos e busca de oportunidades profissionais:

- **`plano-estudos.skill`**: transforma materiais, ementas ou editais em um plano com etapas, sessões, estimativas de tempo, prática e revisões.
- **`tutor-estudos.skill`**: ensina, faz perguntas, propõe exercícios e acompanha o progresso usando o plano criado.
- **`busca-vagas-eng-dados.skill`**: pesquisa vagas remotas de Engenheiro de Dados, compara os requisitos com o currículo e prepara candidaturas para o usuário revisar.

As skills devem estar disponíveis no assistente ou ambiente em que o grupo vai trabalhar. Depois disso, pedidos em linguagem natural sobre planejamento, aprendizagem ou busca de vagas orientam o uso da skill adequada.

## Fluxo de estudos

### 1. Prepare o material e as informações

Para um plano mais preciso, reúna os materiais que serão estudados: PDFs, apostilas, slides, links, vídeos, ementa ou edital. Informe também:

- o objetivo (por exemplo, prova, disciplina ou aplicação no trabalho);
- o prazo ou a data da prova;
- quantas horas por semana e quais dias estão disponíveis;
- o que já sabe sobre o tema.

Cada estudante deve usar seu próprio plano, pois nível, agenda, objetivo e progresso são individuais.

### 2. Peça a criação do plano

Use `plano-estudos.skill` para criar, ajustar ou reorganizar um plano. Ela mapeia os tópicos para os trechos dos materiais, estima o tempo, ordena os assuntos por dependência e inclui prática, revisões e marcos de verificação.

A entrega tem dois formatos:

- **`plano-<tema>.md`**: roteiro estruturado que o tutor lê e atualiza; é a fonte de verdade se houver diferença entre os arquivos.
- **Documento de leitura**: visão geral, etapas, cronograma e materiais em formato mais fácil de consultar.

Confira as suposições e os tópicos marcados como sem material. Se o cronograma não couber no prazo, a skill deve apontar a diferença e sugerir prioridades, em vez de esconder o problema.

### 3. Estude com o tutor

Em cada sessão, anexe o `plano-<tema>.md` ou diga onde ele está. O tutor consulta o progresso, seleciona a próxima sessão e leva em conta os pontos de atenção e as notas anteriores. Também é possível pedir uma explicação, revisão, quiz, flashcards ou exercícios sobre um tema específico sem usar um plano.

O formato padrão de uma sessão alterna explicações curtas, perguntas de verificação e prática. O tutor espera sua tentativa antes de corrigir os exercícios. Se o objetivo ou o nível não estiver claro, ele pode fazer algumas perguntas rápidas para ajustar a aula.

### 4. Feche a sessão e continue depois

Ao encerrar uma sessão do plano, peça ou aguarde o resumo e a atualização do arquivo `.md`. O tutor registra o status, as notas da sessão, os pontos a reforçar, o progresso geral e a data no histórico. Guarde a versão atualizada e use-a na próxima sessão para continuar de onde parou.

Se mudar o prazo, a disponibilidade ou os materiais, peça um **ajuste do plano existente**. A skill deve preservar o histórico e os status das sessões já feitas, recalculando o que ainda está pendente.

## Fluxo de busca de vagas

Use `busca-vagas-eng-dados.skill` quando quiser buscar vagas novas ou atualizar a busca de Engenheiro de Dados remoto.

1. **Anexe ou cole seu currículo.** A skill precisa dele para avaliar as vagas sem inventar experiência. Se não houver currículo na conversa, ela pedirá que você o envie antes de começar.
2. **Informe preferências, se quiser alterar o padrão.** O padrão é Engenheiro de Dados remoto, vagas publicadas nas últimas 24 horas (aceita resultados de até 7 dias) e nota mínima 70. Diga se quer outra localidade, período ou corte de nota.
3. **Revise os resultados.** A skill pesquisa Gupy, Greenhouse, Lever, Ashby e Workable; abre e verifica cada vaga, incluindo se continua aberta, a data de publicação e se o trabalho remoto aceita candidatos no Brasil. Compara requisitos com o currículo e apresenta as vagas que atingem a nota de corte, com justificativa e candidatura curta no idioma da vaga.
4. **Confira e envie você mesmo.** A candidatura é um rascunho para revisar. A skill não envia candidaturas, e-mails ou formulários em seu nome. Se a data da vaga não puder ser confirmada, ela sinaliza isso para você verificar no link.

Cada pessoa deve usar seu próprio currículo e revisar as candidaturas geradas para seu perfil.

## Qual skill usar?

| O que você quer fazer | Skill |
|---|---|
| Criar um cronograma para uma prova ou disciplina | `plano-estudos` |
| Organizar uma ementa, edital ou conjunto de materiais | `plano-estudos` |
| Ajustar um plano porque mudou o prazo ou entrou material novo | `plano-estudos` |
| Aprender ou revisar um conceito | `tutor-estudos` |
| Praticar com exercícios, quiz ou flashcards | `tutor-estudos` |
| Continuar a próxima sessão de um plano existente | `tutor-estudos` |
| Buscar vagas remotas de Engenheiro de Dados | `busca-vagas-eng-dados` |
| Comparar vagas com o currículo e preparar candidaturas para revisar | `busca-vagas-eng-dados` |

## Exemplos de pedidos

**Criar um plano**

> Monte um plano de estudos para a prova de Banco de Dados em 20 de junho. Tenho 6 horas por semana. Já estudei SQL básico. Seguem a ementa e os slides.

**Começar ou continuar uma sessão**

> Vamos continuar meu plano de Python. Anexei o `plano-python.md` e os materiais. Faça a próxima sessão prevista e espere minhas respostas nos exercícios.

**Estudar sem plano**

> Me ensine funções de janela em SQL. Explique um conceito por vez e depois proponha um exercício sem mostrar a resposta antes.

**Replanejar**

> O prazo da prova mudou para 30 de junho e recebi um novo material. Atualize meu plano existente, preservando o que já concluí.

**Buscar vagas**

> Faça minha busca de vagas novas de Engenheiro de Dados remoto. Meu currículo está anexado. Mostre as vagas publicadas recentemente e prepare candidaturas para eu revisar.

## Observações sobre o arquivo do plano

O tutor depende da estrutura do `plano-<tema>.md` e dos campos definidos no modelo incluído em `plano-estudos.skill`. Evite renomear ou apagar sessões concluídas; os identificadores e o histórico permitem retomar o estudo sem perder o contexto.
