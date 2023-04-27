![logo do projeto](assets/logo.png){width="300" .center}

# Notas Musicais

## Como usar?

Você pode chamar as escalas via linha de comando. Por exemplo:

```bash
poetry run escalas
┏━━━┳━━━━┳━━━━━┳━━━━┳━━━┳━━━━┳━━━━━┓
┃ I ┃ II ┃ III ┃ IV ┃ V ┃ VI ┃ VII ┃
┡━━━╇━━━━╇━━━━━╇━━━━╇━━━╇━━━━╇━━━━━┩
│ C │ D  │ E   │ F  │ G │ A  │ B   │
└───┴────┴─────┴────┴───┴────┴─────┘
```

### Alterção na escala

O primeiro parâmetro do CLI é a tônica que deseja exibir. Desta forma, você pode alterar a escala retornada.

```bash
poetry run escalas F#
┏━━━━┳━━━━┳━━━━━┳━━━━┳━━━━┳━━━━┳━━━━━┓
┃ I  ┃ II ┃ III ┃ IV ┃ V  ┃ VI ┃ VII ┃
┡━━━━╇━━━━╇━━━━━╇━━━━╇━━━━╇━━━━╇━━━━━┩
│ F# │ G# │ A#  │ B  │ C# │ D# │ F   │
└────┴────┴─────┴────┴────┴────┴─────┘
```

### Alteração na tonalidade da escala

Você pode alterar a tonalidade da escala também! Esse é o segundo parâmetro da linha de comando. Por exemplo, a escala
de `D#` maior:

```bash
poetry run escalas D# maior
┏━━━━┳━━━━┳━━━━━┳━━━━┳━━━━┳━━━━┳━━━━━┓
┃ I  ┃ II ┃ III ┃ IV ┃ V  ┃ VI ┃ VII ┃
┡━━━━╇━━━━╇━━━━━╇━━━━╇━━━━╇━━━━╇━━━━━┩
│ D# │ F  │ G   │ G# │ A# │ C  │ D   │
└────┴────┴─────┴────┴────┴────┴─────┘
```

## Mais informaçõse sobre o CLI

Para descobrir outras opções, você pode usar a flag ``--help``

```bash
 Usage: escalas [OPTIONS] [TONICA] [TONALIDADE]

╭─ Arguments ─────────────────────────────────────────────────────────────╮
│   tonica          [TONICA]      Tônica da escala. [default: c]          │
│   tonalidade      [TONALIDADE]  Tonalidade da escala. [default: maior]  │
╰─────────────────────────────────────────────────────────────────────────╯
```