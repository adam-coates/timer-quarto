# timer

A countdown timer for Quarto revealjs slides.

```bash
quarto add adam-coates/timer-quarto
```

```yaml
filters:
  - timer
```

```markdown
::: {.timer #discuss seconds=120 starton=interaction}
:::
```

- `seconds`: length of the countdown (default 300).
- `starton`: `slide` (default) counts down while its slide is showing;
  `presentation` counts from when the deck opens, on any slide; `interaction`
  starts paused, and a click starts it.

The dial is 300 × 300 px; to place it, wrap it in an absolute box, for example
`::: {.absolute right=0 bottom=0 width=300px height=300px}`.
