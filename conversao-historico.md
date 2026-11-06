# Conversão de histórico em instruções do GitHub Copilot

Analise todo o histórico desta conversa e transforme o conhecimento técnico acumulado em arquivos de configuração para o GitHub Copilot integrado ao VS Code.

## Objetivo

Extrair decisões, convenções, padrões arquiteturais, regras de negócio, preferências de desenvolvimento e processos de trabalho que possam ser reutilizados em futuras interações com o Copilot.

## Processo

1. Analise o histórico disponível.
2. Identifique decisões técnicas explícitas e regras recorrentes.
3. Separe instruções permanentes de informações temporárias.
4. Elimine duplicações, contradições e informações obsoletas.
5. Não transforme sugestões rejeitadas em regras.
6. Não invente decisões ou convenções.
7. Quando houver incerteza, sinalize o que precisa de confirmação.
8. Não inclua credenciais, tokens ou informações sensíveis.

## Arquivos de saída

Organize o conteúdo conforme a necessidade:

- `.github/copilot-instructions.md`: contexto e regras gerais do projeto.
- `.github/instructions/architecture.instructions.md`: decisões e padrões arquiteturais.
- `.github/instructions/coding.instructions.md`: convenções de implementação.
- `.github/instructions/testing.instructions.md`: estratégias e critérios de testes.
- `.github/instructions/security.instructions.md`: regras de segurança.
- `.github/agents/pr-reviewer.agent.md`: comportamento de um agente especializado em revisão de Pull Requests, caso o histórico contenha requisitos suficientes.

Crie apenas os arquivos que tenham conteúdo relevante.

Para arquivos `*.instructions.md`, configure o frontmatter YAML com `applyTo` apropriado. Não use padrões excessivamente amplos sem necessidade.

## Requisitos de qualidade

- Escreva instruções claras, objetivas e acionáveis.
- Preserve decisões específicas do projeto.
- Evite orientações genéricas que não acrescentem valor.
- Não replique todo o histórico da conversa.
- Separe contexto técnico de instruções comportamentais.
- Evite regras conflitantes entre arquivos.
- Utilize Markdown compatível com o VS Code e GitHub Copilot.

## Entrega

Apresente primeiro a estrutura de diretórios proposta.

Depois, forneça o conteúdo completo de cada arquivo, identificando seu caminho.

Ao final, apresente as decisões extraídas, possíveis conflitos e pontos que precisam de validação humana.

Não modifique arquivos existentes sem minha autorização.
