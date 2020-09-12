# satysfi-fss: Font Selection Scheme for SATySFi

This library provides a font selection scheme for [SATySFi](https://github.com/gfngfn/SATySFi).

## Installation

Use [Satyrographos](https://github.com/na4zagin3/satyrographos) to install this library.

```sh
opam install satysfi-fss
satyrographos install
```

## Usage

Import the following packages:

```satysfi
@require: fss/fss
@require: fss/fonts
@require: fss/style
```

### Font set

Use `\font-set` (inline) or `+font-set` (block) to apply a font set.
`fss/fonts` package provides a font set `Fonts.default-font-set`.

Example:

```satysfi
+font-set(Fonts.default-font-set) <
  +p {
    text \font-set(another-font-set){abc}
  }
>
```

### Font style

In satysfi-fss, font width, weight, style, and so on are managed as font styles.
Use `\font-style` (inline) or `+font-style` (block) to apply font styles.

Example:

```satysfi
+font-style[medium; upright] <
  +p {
    Here is roman text.
    \font-style[italic]{
      Italic text.
        \font-style[bold]{
          Bold italic text.
        }
    }
  }
>
```

`fss/fonts` package provides the following font style keywords.

- Weight: `medium`, `bold`
- Style: `upright`, `italic`
