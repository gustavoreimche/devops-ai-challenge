# devops-ai-challenge

Exercício prático de 1 hora para a vaga de especialista DevOps.

## Contexto

Você acabou de assumir a plataforma de pipeline e deploy de uma empresa com
vários serviços. Existe um padrão que todo serviço deve seguir para ir para
produção, e uma frota que o segue em graus diferentes.

- `padrao/` é a referência: pipeline, Dockerfile e manifesto Kubernetes. As
  regras estão em [`padrao/POLICY.md`](padrao/POLICY.md): um serviço só pode ir
  para produção quando cumpre as cinco ao mesmo tempo.
- `frota/` contém três serviços: `servico-catalogo`, `servico-notificacoes` e
  `servico-pagamentos`.

Os arquivos `.ci/pipeline.yml` são cópias extraídas para revisão. Não é preciso
executar a pipeline.

Você lidera **dois consultores terceiros**, especialistas que conhecem muito bem
a plataforma. Eles executam; o que depende de você é a direção: o que fazer
primeiro, como recortar o trabalho e como saber que cada entrega está pronta.

## O problema

A frota vai para produção na próxima leva, e a plataforma precisa garantir que
o padrão está sendo cumprido. Sua tarefa:

1. **Avalie os três serviços contra a `POLICY.md`.** Quais estão em
   conformidade e quais não estão? Mostre a evidência em cada caso.
2. **Avalie o próprio padrão.** Ele garante o que a política promete? Se não,
   onde falha?
3. **Priorize as correções** e diga em que ordem devem acontecer, e por quê.
4. **Distribua o trabalho entre os dois consultores,** com o critério de pronto
   de cada entrega e como você vai acompanhar.
5. **Faça você mesmo uma mudança concreta** no repositório: a que achar que
   mais reduz risco.

## Como vai ser

| Tempo | O quê |
|---|---|
| 5 min | Leitura deste README e perguntas iniciais |
| 35 min | Mão na massa, com a tela compartilhada |
| 10 min | Você apresenta o que encontrou e o que fez |
| 10 min | Conversa com o entrevistador |

- Faça um fork ou clone do repositório e trabalhe no **seu ambiente, com o seu
  setup de IA**, do jeito que usa no dia a dia: assistentes, agents, skills,
  comandos próprios. Não existe ferramenta certa.
- **Pense em voz alta.** Conte o que está tentando, por que pediu algo à IA e o
  que achou da resposta.
- **Pode perguntar** ao entrevistador a qualquer momento sobre contexto e
  prioridades. Ele não indica caminho.
- Não se espera que você termine tudo em 35 minutos. Escolher o que fica de
  fora, e dizer por quê, faz parte da resposta.

## O que será avaliado

- **Setup e uso de IA:** como seu ambiente está montado e como você usa a IA
  para explorar, decompor o problema e conferir o que ela devolve, e não só
  para gerar resposta.
- **Raciocínio de DevOps:** entender o problema antes de propor solução,
  priorizar por risco e questionar o que for preciso, inclusive o padrão.
- **Gestão:** dar direção a especialistas: recortar o trabalho em entregas
  verificáveis e acompanhar sem microgerenciar.
- **Execução:** uma mudança bem escolhida, com evidência de que resolve.

Não há pegadinha de ferramenta nem resposta única. Uma resposta curta e bem
justificada vale mais que uma lista longa de problemas.
