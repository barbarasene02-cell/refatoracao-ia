# Refatorando código com apoio de IA

Atividade: revisar um script Python com problemas propositais usando IA e aplicar melhorias.

## Arquivos
- `programa_notas_original.py`: código original, sem alterações
- `programa_notas_revisado.py`: código revisado após as sugestões da IA

## Prompt usado
> Revise este código Python e sugira melhorias de legibilidade, estrutura e tratamento de erro: (código colado)

IA utilizada: Claude

## Sugestões da IA
- Trocar nomes de uma letra por nomes descritivos
- Separar a lógica em funções (`ler_nota`, `calcular_media`, `main`)
- Tratar erros de entrada com `try/except` (texto, zero notas)
- Validar o intervalo das notas (0 a 10)
- Trocar o número solto `6` por uma constante (`MEDIA_MINIMA`)
- Usar `sum()` e `if __name__ == "__main__"`

## Comparação
A versão original fazia tudo em um bloco único, com variáveis de uma letra e sem proteção contra entradas inválidas, o que causava erro com texto ou com zero notas. Na versão revisada, renomeei as variáveis, separei a lógica em funções e adicionei tratamento de erro com `try/except` e validação do intervalo das notas. Com isso, o código ficou mais legível, reutilizável e não quebra com entradas incorretas.
