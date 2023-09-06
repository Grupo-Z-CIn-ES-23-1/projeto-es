# Modelo Entidade-Relacionamento para a Aplicação de Previsão de Enchentes

## Entidades e Atributos

### Usuário
- **username** (PK): String (identificador único para o usuário)
- **password**: String

## Relações

Atualmente, temos apenas uma entidade, que é o "Usuário", e não temos relações específicas no banco de dados, pois a maioria das funcionalidades consome dados em tempo real sem armazená-los. 

## Notas Adicionais

1. **Localização:** A localização é fornecida pelo usuário a cada consulta e não é armazenada no banco de dados.
2. **Dados Meteorológicos e Previsões de Enchente:** Ambos os dados são consumidos em tempo real e não são armazenados no banco de dados. Isso significa que não há entidades específicas para eles no modelo ER.
3. **Funcionalidades Futuras:** À medida que novas funcionalidades forem adicionadas, como alertas ou armazenamento de previsões históricas, o modelo ER pode precisar ser atualizado para refletir as novas entidades e relações.
