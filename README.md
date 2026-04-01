INFO[0000] Using docker host 'unix:///var/run/docker.sock', and daemon socket 'unix:///var/run/docker.sock'
Stage  Job ID             Job name           Workflow name       Workflow file              Events
0      teste-basico       teste-basico       Hello Local         01-hello-local.yml         push,workflow_dispatch
0      setup-e-lint       setup-e-lint       Pipeline Principal  02-pipeline-principal.yml  push
1      testes-unitarios   testes-unitarios   Pipeline Principal  02-pipeline-principal.yml  push
1      scan-de-seguranca  scan-de-seguranca  Pipeline Principal  02-pipeline-principal.yml  push
2      build-e-deploy     build-e-deploy     Pipeline Principal  02-pipeline-principal.yml  push

VALIDAÇÃO DA PARTE 04:
O Job 2 o Job 3 rodaram em paralelo porque estão no Stage 1, o que indica que possuem as mesmas dependências e foram executados simultaneamente
