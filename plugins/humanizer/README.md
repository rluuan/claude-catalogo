# humanizer (português)

Skill que revisa textos e tira as marcas de escrita de IA: contrastes do tipo "não é X, é Y", frases de efeito no fim do parágrafo, listas forçadas de três, travessões por toda parte, linguagem de propaganda, negrito em tudo e por aí vai. São 26 padrões, cada um com exemplo de antes e depois.

## Crédito

O autor original é **blader (Siqi Chen)**: [github.com/blader/humanizer](https://github.com/blader/humanizer). O trabalho de verdade é dele; aqui só tem a tradução.

Esta versão foi traduzida da 3.1.0 (commit `0ef9fe5`). Algumas partes foram adaptadas porque não fazem sentido em português:

- §10 falava do hífen em adjetivos compostos do inglês; virou estrangeirismos e jargão de efeito.
- §12 (palavras típicas de IA) ganhou uma lista em português.
- §20 explica que título com Todas As Palavras Em Maiúscula é costume do inglês.
- §8 abre exceção para o travessão de diálogo em ficção.

A licença MIT original está em [LICENSE](LICENSE).

## Como usar

Depois de instalar o plugin (veja o README da raiz), é só pedir no Claude Code:

```
/humanizer revisa esse texto: ...
```

Ou pedir em linguagem normal, tipo "tira a cara de IA desse post", que o Claude carrega a skill sozinho.
