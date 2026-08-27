# devops-ai-challenge

Um snapshot de configuração de pipeline e deploy de uma plataforma
fictícia com múltiplos serviços, para fins de revisão de arquitetura e
governança.

- `padrao/` é a referência: o padrão que todo serviço deveria seguir,
  descrito em [`padrao/POLICY.md`](padrao/POLICY.md).
- `frota/` contém três serviços reais, cada um em um estado diferente de
  aderência a esse padrão.

Os arquivos `.ci/pipeline.yml` aqui são cópias extraídas para revisão — não
é necessário (nem o objetivo) executar essa pipeline de verdade.

As instruções do exercício foram enviadas separadamente pelo entrevistador.
