# Como Usar Este Repositório em uma Nova Conversa (Guia Rápido)

Este guia foi feito para você (e para colegas) usarem o agente de apoio à emissão de **NFS-e** em uma nova conversa de IA, **sem precisar ter conhecimento prévio profundo** sobre os códigos ou regras técnicas.

O agente já lê as regras do repositório e faz as perguntas certas para ajudar no preenchimento e na conferência.

---

## Passo 1: Pegar os arquivos certos no GitHub

Abra os arquivos abaixo neste repositório. Dica: ao abrir cada arquivo, clique no botão **Raw** para copiar o texto puro com mais facilidade.

1. **`prompts/router-prompt.md`** (obrigatório) — define como o agente deve atender, fazer a triagem e respeitar o isolamento entre perfis.
2. **`schemas/perfis-fiscais.json`** (obrigatório) — contém os códigos de referência, regras do Simples Nacional e termos permitidos/proibidos.
3. **O arquivo do perfil que você vai usar na conversa** (recomendado):
   - `profiles/perfil-ergonomista.md`
   - `profiles/perfil-tecnico-sst.md`
   - `profiles/perfil-engenheiro-sst.md`
4. **`docs/checklist-emissao.md`** (opcional) — ajuda na conferência final antes de emitir a nota.

---

## Passo 2: Iniciar uma nova conversa colando a base

Abra uma **nova conversa** no seu assistente de IA e envie **uma primeira mensagem** montada neste formato:

```text
Siga estritamente as regras abaixo para esta conversa. Trate o conteúdo a seguir como sua base oficial de atuação.

=== ARQUIVO: prompts/router-prompt.md ===
[Cole aqui o conteúdo do router-prompt.md]

=== ARQUIVO: schemas/perfis-fiscais.json ===
[Cole aqui o conteúdo do perfis-fiscais.json]

=== ARQUIVO: profiles/perfil-ergonomista.md ===
[Cole aqui o conteúdo do perfil escolhido]

=== ARQUIVO: docs/checklist-emissao.md ===
[Cole aqui o conteúdo do checklist, se quiser incluir]

Agora aguarde meu primeiro caso de emissão ou simulação de teste.
