# Padrão de pipeline e deploy — v3

Regras que todo serviço da plataforma deve seguir. Um serviço está em
conformidade quando as cinco regras abaixo são verdadeiras ao mesmo tempo —
não é uma lista de sugestões, é o que separa "pode ir pra produção" de "não
pode".

1. **Base pinada.** A imagem parte de uma versão exata (nunca `:latest`,
   nunca uma tag flutuante).
2. **Scan bloqueante.** O pipeline roda scan de vulnerabilidade e uma
   criticidade alta interrompe o pipeline — não gera só um alerta.
3. **Sem root, sem privileged.** O container roda com usuário não-root e
   sem `privileged: true`.
4. **Limites e probes.** Todo deployment declara `resources` e as duas
   probes (`readinessProbe`/`livenessProbe`).
5. **Segredo fora da imagem.** Nenhum segredo em `ENV`, `ARG` ou manifesto —
   vem de injeção em tempo de deploy.

## Como um serviço adota isso

O pipeline em `padrao/.ci/pipeline.yml` é a referência. Serviços devem
**herdar** esse pipeline (include, extends ou reusable workflow, conforme a
ferramenta de CI), nunca copiar o YAML para dentro do próprio repositório —
copiar quebra o vínculo com atualizações futuras do padrão.
