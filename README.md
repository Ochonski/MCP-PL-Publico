# MCP PL — canal público

Repositório público oficial para manifests assinados, revogação de licenças e metadados de releases do MCP PL.

Este repositório não contém código-fonte, configuração Oracle, credenciais ou chaves privadas. Binários oficiais futuros devem ser distribuídos preferencialmente como GitHub Release Assets.

O `version.json` informa versão SemVer, build, canal, URL do GitHub Release Asset, tamanho e SHA-256. A assinatura permanece vazia e o estado `PREPARED` até a assinatura externa pela chave privada oficial; o repositório nunca contém essa chave. Um manifesto sem assinatura não pode ser aplicado pelo MCP PL.

Este canal não contém `.git` copiado, código-fonte privado, configurações locais, credenciais, logs ou dados operacionais.
