# Histórico de versões

## 0.6.1 — 2026-09-15

- Corrige o início automático do Secure MCP Tunnel: cada integração habilitada, configurada e marcada para início automático passa a ser avaliada ao abrir o launcher, sem bloqueio por configuração global antiga.
- Registra início, confirmação, falha e parada do túnel como eventos sanitizados na página Logs.
- Corrige a reconstrução visual das tabelas de conexões e integrações, removendo widgets antigos antes de redesenhar o status.
- Apresenta BI2 como conexão única no cadastro, com autenticação Windows e política somente leitura do catálogo corporativo.

## 0.6.0 — 2026-09-15

- Adiciona `integration_search_files` para localizar arquivos por nome ou caminho em todas as Bases de Soluções habilitadas.
- Adiciona `integration_read_file` para ler somente conteúdo já sanitizado de um resultado indexado, sem acesso livre ao disco.
- Orienta todos os clientes MCP a consultar os documentos autorizados antes de pedir anexos ao usuário.
- Migra o catálogo não sensível do BI2 para instalações existentes sem apagar conexões e passa a exibir seu estado no dashboard e nas tools MCP.

## 0.5.1 — 2026-09-15

- Indexa automaticamente Oracle Forms e Bases de Soluções logo após salvar uma pasta, sem exigir reinício do painel.
- Mantém cadastro de conexões em gravação atômica e usa a mesma pasta de dados no launcher e no servidor MCP instalado.
- Exibe o estado real de cada Base: acesso indisponível, sem arquivos compatíveis, não indexada ou quantidade efetiva de arquivos indexados.
- Restringe a pesquisa MCP às Bases habilitadas.

## 0.4.1 — 2026-09-14

- Remove a confirmação genérica exibida antes de o login OWNER terminar.
- Mantém o botão e o indicador em estado de autenticação até a resposta do Firebase.
- Confirma explicitamente quando a sessão não foi criada e registra somente a categoria sanitizada da falha.

## 0.4.0 — 2026-09-12

- Torna o Firebase Authentication por e-mail e senha o login principal da sessão OWNER temporária.
- Autoriza exclusivamente o UID OWNER confiável, exige e-mail verificado e valida assinatura, projeto e expiração do ID token.
- Mantém senha e tokens somente durante a autenticação, sem persistência, refresh automático, cadastro ou Firebase Admin no cliente.
- Exibe contagem regressiva de 15 minutos, logout imediato e acesso criptográfico de contingência.

## 0.3.1 — 2026-09-11

- Corrige upgrades que preservavam o `version.json` antigo e faziam o EXE novo continuar exibindo a versão anterior.
- Atualiza atomicamente a versão e a cadeia pública de confiança a partir do EXE instalado, preservando configurações e dados do usuário.

## 0.3.0 — 2026-09-11

- Adiciona acesso OWNER temporário por código de seis números enviado por e-mail e validado por serviço central HTTPS.
- Vincula o código ao desafio e à instalação, limita tentativas, aplica uso único e mantém sessão OWNER por 15 minutos.
- Preserva o fluxo por arquivo como recuperação quando o serviço central não estiver configurado.

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
