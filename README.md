## Geral

Nesta seção, são apresentadas diretrizes gerais para a nomenclatura de tabelas e colunas em um banco de dados.

- Os nomes das tabelas e colunas devem estar em letras minúsculas (exemplo: `nome_da_tabela`, `nome_da_coluna`).
- As palavras devem ser separadas por um underscore (`_`). Isso é conhecido como padrão "snake case" (exemplo: `nome_composto`).
- Todos os termos devem estar em inglês, com exceção de alguns termos que não possuem uma tradução apropriada para o inglês.
- É recomendado usar nomes descritivos que explicitem claramente o conteúdo da tabela ou coluna.
- Evite ao máximo o uso de contrações, optando por palavras completas e mais descritivas.

## Tabelas

Esta seção aborda especificamente a nomenclatura de tabelas.

- Os nomes de tabelas devem estar no plural (exemplo: `users`, `posts`, `roles`, `room_categories`).
- Evite usar singularidades para nomes de tabelas (exemplo ruim: `user`, `post`, `grupo`, `quarto_categoria`).

## Colunas

Esta seção aborda a nomenclatura de colunas.

- Os nomes de colunas devem estar no singular (exemplo: `cpf`, `name`, `age`).
- Evite usar pluralidades para nomes de colunas (exemplo ruim: `enderecos`, `posts`, `idades`).

## Chaves Estrangeiras (Foreign Keys)

Nesta seção, são fornecidas instruções para a nomenclatura de chaves estrangeiras.

- Todas as chaves estrangeiras devem seguir o padrão `nome_da_tabela_no_singular_id` (exemplo: `role_id`).
- Este padrão ajuda a identificar claramente a relação entre tabelas.

### Exemplo:

- Se a tabela `users` tem um relacionamento com a tabela `roles`, o nome da coluna de chave estrangeira na tabela `users` deve ser `role_id`.

## Chaves Primárias (Primary Keys)

Aqui são apresentadas as diretrizes para a nomenclatura de chaves primárias.

- A chave primária de toda tabela deve ser uma coluna de inteiros com incremento automático, e deve ser chamada de `id`.

## Timestamps

Esta seção trata da definição de colunas para armazenar timestamps.

- Toda tabela deve ter duas colunas para armazenar timestamps: `created_at` e `updated_at`.
- A coluna `created_at` é preenchida automaticamente com o timestamp do momento em que o registro é criado.
- A coluna `updated_at` é preenchida automaticamente com o timestamp do momento em que o registro é alterado.
