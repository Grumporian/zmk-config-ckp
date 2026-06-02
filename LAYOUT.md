# BT65 Keymap Reference

ANSI 65% on a US-International host layout. `MO1` = raise (FN), `MO2` = german (umlauts/symbols).

---

## Special characters cheat sheet

Hold `MO2` (the key right of `/`), then press:

| Press         | You get                  |
|---------------|--------------------------|
| `ESC`         | `~`                      |
| `R`           | `€`                      |
| `U`           | `ü`  (Shift → `Ü`)       |
| `O`           | `ö`  (Shift → `Ö`)       |
| `A`           | `ä`  (Shift → `Ä`)       |
| `S`           | `ß`                      |

Default layer extras (no layer needed):
- `'` always types a literal `'` (Shift+`'` → `"`) — the macro double-taps to escape US-Intl's dead acute.

---

## Layer 0 — Default

```
┌──────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┐
│ ESC  │  1  │  2  │  3  │  4  │  5  │  6  │  7  │  8  │  9  │  0  │  -  │  =  │BKSP │ ▶❚❚ │
├──────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┤
│ TAB  │  Q  │  W  │  E  │  R  │  T  │  Z  │  U  │  I  │  O  │  P  │  [  │  ]  │  \  │HOME │
├──────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┴─────┼─────┤
│ CAPS │  A  │  S  │  D  │  F  │  G  │  H  │  J  │  K  │  L  │  ;  │  '  │   ENTER   │ DEL │
├──────┴─┬───┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┴─┬───────┬─┴─────┤
│ SHIFT  │ Y │  X  │  C  │  V  │  B  │  N  │  M  │  ,  │  .  │  /  │  MO2  │   ↑   │  END  │
├────┬───┴┬──┴──┬──┴─────┴─────┴─────┴─────┴─────┴───┬─┴─────┴┬──────┬────┴┬─────┬─┴┬─────┤
│CTRL│ GUI│ ALT │              SPACE                 │  RALT  │ MO1  │CTRL │  ←  │ ↓│  →  │
└────┴────┴─────┴────────────────────────────────────┴────────┴──────┴─────┴─────┴──┴─────┘
```

Notes:
- `Z` and `Y` are swapped (QWERTZ-style on a US-Intl host).
- `'` is the `doubleSQT` macro — two taps under the hood to escape the dead acute.
- Encoder: rotate = volume ± , press = `▶❚❚` (top-right key).

---

## Layer 1 — Raise (hold `MO1`)

```
┌──────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┐
│ ESC  │ F1  │ F2  │ F3  │ F4  │ F5  │ F6  │ F7  │ F8  │ F9  │ F10 │ F11 │ F12 │ BL  │ RGB │
│      │     │     │     │     │     │     │     │     │     │     │     │     │ TOG │ TOG │
├──────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┤
│      │BT0  │BT1  │BT2  │BT3  │BT4  │     │     │     │     │ EXT │     │     │SYS  │ RGB │
│      │     │     │     │     │     │     │     │     │     │ PWR │     │     │RST  │ HUI │
├──────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┴─────┼─────┤
│      │PREV │SLEEP│NEXT │     │     │     │     │     │     │     │     │   BOOT    │ RGB │
│      │     │     │     │     │     │     │     │     │     │     │     │  LOADER   │ HUD │
├──────┴─┬───┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┴─┬───────┬─┴─────┤
│        │   │     │BT   │     │     │     │     │     │     │     │       │  RGB  │ BL    │
│        │   │     │CLR  │     │     │     │     │     │     │     │       │  BRI  │ INC   │
├────┬───┴┬──┴──┬──┴─────┴─────┴─────┴─────┴─────┴───┬─┴─────┴┬──────┬────┴┬─────┬─┴┬─────┤
│BT  │BT  │ BT  │                                    │        │      │     │PREV │RGB│NEXT │
│PRV │NXT │ CLR │                                    │        │      │     │     │BRD│     │
└────┴────┴─────┴────────────────────────────────────┴────────┴──────┴─────┴─────┴──┴─────┘
```

Notes:
- `BT_CLR` appears twice (raise+D, raise+ALT) — pressing either clears the current pairing.
- `BOOTLOADER` puts the board into UF2 mode for flashing.

---

## Layer 2 — German (hold `MO2`)

```
┌──────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┐
│  ~   │     │     │     │     │     │     │     │     │     │     │     │     │     │     │
├──────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┤
│      │     │     │  €  │     │     │     │  ü  │     │  ö  │     │     │     │     │     │
├──────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┴─────┼─────┤
│      │  ä  │  ß  │     │     │     │     │     │     │     │     │     │           │     │
├──────┴─┬───┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┴─┬───────┬─┴─────┤
│        │   │     │     │     │     │     │     │     │     │     │       │       │       │
├────┬───┴┬──┴──┬──┴─────┴─────┴─────┴─────┴─────┴───┬─┴─────┴┬──────┬────┴┬─────┬─┴┬─────┤
│    │    │     │                                    │        │      │     │     │   │     │
└────┴────┴─────┴────────────────────────────────────┴────────┴──────┴─────┴─────┴──┴─────┘
```

All blank cells are `&trans` (passes through to the default layer below).

---

## Host setup required

Both Linux and Windows must be on **United States-International** keyboard layout. Without it, the umlaut macros produce literal `"a` instead of `ä` because they rely on the OS treating `Shift+'` as a dead diaeresis.

- **Linux:** add "English (US, intl., with dead keys)" in your DE's keyboard settings.
- **Windows:** add "United States-International" and remove plain "US" so `Win+Space` can't toggle you off it.

---

## Macro internals

| Macro         | What it sends                              | Why                                                           |
|---------------|--------------------------------------------|---------------------------------------------------------------|
| `ae/oe/ue`    | `Shift+'` → vowel                          | US-Intl dead diaeresis + vowel                                |
| `scharfes_s`  | `RAlt+S`                                   | US-Intl AltGr position for `ß`                                |
| `euro`        | `RAlt+5`                                   | US-Intl AltGr position for `€`                                |
| `wave`        | `Shift+\`` × 2                             | First tap arms dead tilde, second tap commits literal `~`     |
| `doubleSQT`   | `'` × 2 (or `"` × 2 with Shift)            | First tap arms dead acute/diaeresis, second tap commits it    |

Tuning: `wait-ms = 60`, `tap-ms = 40`. Lower `wait-ms` if macros feel sluggish; raise it if Windows occasionally drops the dead-key sequence.
