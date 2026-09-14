# devops-ai-challenge

Exercício prático de 1 hora para a vaga de especialista DevOps.

## Contexto

Você acabou de assumir a plataforma de pipeline e deploy de uma empresa com
vários serviços. Existe um padrão que todo serviço deveria seguir, e uma frota
que o segue em graus diferentes.

- `padrao/` é a referência: pipeline, Dockerfile e manifesto Kubernetes, com as
  regras descritas em [`padrao/POLICY.md`](padrao/POLICY.md).
- `frota/` contém três serviços: `servico-catalogo`, `servico-notificacoes` e
  `servico-pagamentos`.

Os arquivos `.ci/pipeline.yml` são cópias extraídas para revisão. Não é preciso
executar a pipeline.

Para executar o trabalho, você lidera **dois consultores terceiros**, também
especialistas. Eles são bons tecnicamente, mas não conhecem a plataforma: o que
eles fizerem depende de como você recortar e acompanhar o trabalho.

## O problema

A diretoria quer levar a frota para produção e precisa de uma resposta sua:

1. **Quais serviços podem ir para produção hoje, e quais não podem?** Por quê?
2. **O que precisa ser corrigido, em que ordem?** Considere os serviços e
   também o próprio padrão, se achar que ele tem problema.
3. **Como você distribuiria esse trabalho entre os dois consultores,** e como
   saberia que cada entrega está pronta?
4. **Faça você mesmo uma mudança concreta** no repositório: a que achar que
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
- **Pode perguntar** ao entrevistador a qualquer momento. Ele faz o papel da
  diretoria e responde sobre contexto e prioridades, mas não indica caminho.
- Não se espera que você termine tudo em 35 minutos. Escolher o que fica de
  fora, e dizer por quê, faz parte da resposta.

## O que será avaliado

- **Setup e uso de IA:** como seu ambiente está montado e como você usa a IA
  para explorar, decompor o problema e conferir o que ela devolve, e não só
  para gerar resposta.
- **Raciocínio de DevOps:** entender o problema antes de propor solução,
  priorizar por risco e questionar o que for preciso, inclusive o padrão.
- **Gestão:** recortar o trabalho em entregas que outra pessoa consiga executar
  e que você consiga verificar.
- **Execução:** uma mudança bem escolhida, com evidência de que resolve.

Não há pegadinha de ferramenta nem resposta única. Uma resposta curta e bem
justificada vale mais que uma lista longa de problemas.
