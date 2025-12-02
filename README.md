🔄 Transações MySQL – Teste com a tabela cadastro

Este script apresenta uma demonstração clara de como funcionam as transações no MySQL, permitindo inserir dados, validar resultados e decidir se as alterações devem ser confirmadas ou desfeitas. É um recurso essencial para quem estuda integridade e controle de mudanças em banco de dados.

🧩 O que o script faz
🏗️ Criação da tabela de teste

A tabela cadastro contém dois campos básicos usados para simulações:

nome – nome da pessoa

docto – documento vinculado

🚦 Início da transação

START TRANSACTION;
A partir deste ponto, tudo que é inserido fica pendente, permitindo avaliação antes da confirmação.

📥 Inserção de registros

Três valores são adicionados temporariamente:

Andre — 12341244

Joao — 12341248

Pedro — 12341246

Essas linhas só passam a existir oficialmente no banco após o COMMIT.

⏪ Opção de desfazer

O script inclui a possibilidade de desfazer tudo com:

ROLLBACK;


(basta remover o comentário)

✅ Confirmação

COMMIT;
Confirma e grava as alterações de forma permanente.

🎯 Objetivo do material

Este exemplo mostra, na prática:

Como usar transações para testar mudanças

Como desfazer ações antes de confirmar

Como garantir consistência e segurança

Como funciona o ciclo Transação → Verificação → Commit/Rollback

É um ótimo exercício para estudantes em formação na área de banco de dados.
