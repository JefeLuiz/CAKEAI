# CAKEIA: Encontre e adapte receitas usando IA generativa do Google

## Descrição
Este projeto explora o poder da IA generativa do Google para criar uma experiência culinária interativa e personalizada. Através da combinação de embeddings semânticos e geração de texto avançada, o Bolo IA permite que você encontre e adapte receitas de bolo de forma intuitiva e eficiente.

## Funcionalidades
Busca semântica: Descreva o bolo que você deseja em linguagem natural. A IA utiliza embeddings para encontrar a receita mais similar na base de dados.
Adaptação inteligente: Informe suas restrições alimentares ou preferências (sem glúten, vegano, etc.) e a IA ajustará a receita automaticamente.

## Demonstração
```Qual bolo iremos assar hoje? um bolo red velvet ```

Após encontrar a receita base, você pode personalizá-la:

```tenho alergia ao glutem, altere os ingredientes nocivos para mim.```

O Bolo IA fornecerá a receita modificada, pronta para ser preparada!

## Como funciona
**Criação de embeddings:** Embeddings (representações matemáticas de texto) são geradas para cada receita utilizando o modelo `models/embedding-001` do Google Generative AI.
Busca por similaridade: A IA calcula o produto escalar entre o embedding da sua descrição e os embeddings das receitas para identificar a melhor correspondência.

## Adaptação de receita: O modelo `gemini-1.0-pro` gera texto para substituir ingredientes, garantindo que a receita atenda às suas necessidades.

## Tecnologias
**Google Generative AI:** `models/embedding-001` para embeddings e `gemini-1.0-pro` para geração de texto.
**Pandas:** Manipulação e análise de dados.
**NumPy:** Computação numérica.

## Próximos passos
Expandir a base de dados com mais receitas.
Criar uma interface gráfica amigável.
Implementar suporte para mais restrições e preferências.
Contribua
Sinta-se à vontade para contribuir com este projeto! Abra issues, envie pull requests ou compartilhe suas ideias.
Disclaimer
As informações geradas por IA são sugestões e devem ser revisadas por um humano antes da utilização.
