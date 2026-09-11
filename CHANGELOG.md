# Histórico de versões

## 0.2.2 — 2026-09-11

- Corrige o fechamento pelo X para minimizar à bandeja ou encerrar completamente quando a bandeja do Windows estiver indisponível.
- Adiciona encerramento cooperativo do launcher antes da desinstalação, evitando processo invisível e arquivo bloqueado.

## 0.2.1 — 2026-09-11

- Disponibiliza a verificação de atualizações diretamente na Visão Geral para usuários com perfil Visualizador.
- Mantém o acesso às demais funções administrativas protegido pelas permissões existentes.

## 0.2.0 — 2026-09-10

- Adiciona instalador Windows por usuário com upgrade e desinstalação segura.
- Separa binários dos dados persistentes e torna o servidor MCP autônomo no EXE.
- Adiciona diagnóstico sanitizado e log de bootstrap com rotação limitada.
- Permite solicitar acesso OWNER temporário em qualquer instalação por desafio assinado, sem transferir a chave privada OWNER.

## 0.1.2 — 2026-09-10

- Implementa OWNER global com cadeia Ed25519 e challenge-response anti-replay.
- Adiciona licença corporativa assinada, enforcement central e versão mínima.
- Provisiona chaves distintas para OWNER, licença e release em cofre do Windows.
- Adiciona restauração autenticada do backup OWNER com dry-run e teste isolado.
- Publica o instalador oficial com manifesto e assinatura delegada de release.

## 0.1.1 — 2026-09-10

- Automatiza commits e pushes com validação de branch, remote e fast-forward.
- Comprova atualização self-contained A→B, preservação e rollback.
- Adiciona infraestrutura de migrações locais versionadas e reversíveis.

## 0.1.0 — 2026-09-10

- Consolida o launcher executivo, conexões multibanco e integrações de IA.
- Amplia a indexação e as consultas estruturais de Oracle Forms.
- Endurece as políticas somente leitura em PROD/GOLD, privacidade e auditoria.
- Prepara o canal público, versionamento SemVer e atualização com validação e rollback.
