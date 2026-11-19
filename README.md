# nfse-sst-simples-agent

Esse agente visa te ajudar a emitir **NFS-e** pelo novo sistema do governo se você é um prestador de serviços de consultoria técnica de segurança do trabalho, compreendendo avaliação de SST, treinamentos, análise das atividades e elaboração de documento técnico conforme escopo acordado com a contratante.

A base foi estruturada para empresas optantes pelo **Simples Nacional**, mantendo **isolamento estrito** entre três perfis profissionais para evitar contradições fiscais e de atribuição:

- `TECNICO_SST` (Técnico de Segurança do Trabalho)
- `ERGONOMISTA` (Ergonomista / Consultor em Ergonomia)
- `ENGENHEIRO_SST` (Engenheiro de Segurança do Trabalho)

## Estrutura do Repositório

- `README.md`: Visão geral do projeto, escopo de atuação e instruções de uso.
- `schemas/perfis-fiscais.json`: Regras fiscais do Simples Nacional, códigos de referência e listas de termos permitidos/proibidos por perfil.
- `prompts/router-prompt.md`: System prompt com triagem obrigatória, isolamento de perfis e checklist anti-contradição.

## Regra Central de Isolamento

O agente não deve misturar CNAEs, códigos (LC 116, NBS, `cIndOp`) ou terminologia de um perfil em outro. Antes de preencher ou auditar uma nota, o perfil ativo deve ser definido e validado conforme o escopo real entregue.

## Como Usar com Seu Agente de IA

1. Configure o conteúdo de `prompts/router-prompt.md` como instrução do sistema / diretriz principal do agente.
2. Anexe ou forneça `schemas/perfis-fiscais.json` como fonte de referência estruturada.
3. Informe o perfil ativo, o CNAE utilizado e o escopo do serviço para gerar o preenchimento guiado da NFS-e.
