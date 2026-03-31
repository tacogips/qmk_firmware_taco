# Ergo68 / ErgoDash Layout Compare

比較前提:

- `Ergo68`: QMK `yushakobo/ergo68`
- `ErgoDash`: [`/Users/taco/gits/tacogips/ergodash_keymap/keymap.c`](/Users/taco/gits/tacogips/ergodash_keymap/keymap.c)
- `top layer` のみ
- `1セル = 1物理キー`
- 各セルは `key` と `m[row,col]`
- 共通位置は同じ列にそろえている

## Difference Summary

- 共通のメイン配列はほぼ同じ
- 物理形状の差は `ErgoDash` の親指上部 2 キーが左右に 1 組ずつあること
- 差分は `4 positions`
- `Ergo68` にはその 4 ポジションが無い

## Ergo68

| prow | L0 | L1 | L2 | L3 | L4 | L5 | L6 |  | R6 | R5 | R4 | R3 | R2 | R1 | R0 |
|---:|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 0 | `KC_ESC`<br>`m[0,0]` | `KC_1`<br>`m[0,1]` | `KC_2`<br>`m[0,2]` | `KC_3`<br>`m[0,3]` | `KC_4`<br>`m[0,4]` | `KC_5`<br>`m[0,5]` |  |  |  | `KC_6`<br>`m[5,5]` | `KC_7`<br>`m[5,4]` | `KC_8`<br>`m[5,3]` | `KC_9`<br>`m[5,2]` | `KC_0`<br>`m[5,1]` | `KC_PSCR`<br>`m[5,0]` |
| 1 | `KC_TAB`<br>`m[1,0]` | `KC_Q`<br>`m[1,1]` | `KC_W`<br>`m[1,2]` | `KC_E`<br>`m[1,3]` | `KC_R`<br>`m[1,4]` | `KC_T`<br>`m[1,5]` | `KC_LBRC`<br>`m[1,6]` |  | `KC_RBRC`<br>`m[6,6]` | `KC_Y`<br>`m[6,5]` | `KC_U`<br>`m[6,4]` | `KC_I`<br>`m[6,3]` | `KC_O`<br>`m[6,2]` | `KC_P`<br>`m[6,1]` | `KC_BSLS`<br>`m[6,0]` |
| 2 | `KC_CAPS`<br>`m[2,0]` | `KC_A`<br>`m[2,1]` | `KC_S`<br>`m[2,2]` | `KC_D`<br>`m[2,3]` | `KC_F`<br>`m[2,4]` | `KC_G`<br>`m[2,5]` | `KC_MINS`<br>`m[2,6]` |  | `KC_EQL`<br>`m[7,6]` | `KC_H`<br>`m[7,5]` | `KC_J`<br>`m[7,4]` | `KC_K`<br>`m[7,3]` | `KC_L`<br>`m[7,2]` | `KC_SCLN`<br>`m[7,1]` | `KC_ENT`<br>`m[7,0]` |
| 3 | `KC_LSFT`<br>`m[3,0]` | `KC_Z`<br>`m[3,1]` | `KC_X`<br>`m[3,2]` | `KC_C`<br>`m[3,3]` | `KC_V`<br>`m[3,4]` | `KC_B`<br>`m[3,5]` | `KC_DEL`<br>`m[3,6]` |  | `KC_BSPC`<br>`m[8,6]` | `KC_N`<br>`m[8,5]` | `KC_M`<br>`m[8,4]` | `KC_COMM`<br>`m[8,3]` | `KC_DOT`<br>`m[8,2]` | `KC_SLSH`<br>`m[8,1]` | `KC_RSFT`<br>`m[8,0]` |
| 4 | `KC_LCTL`<br>`m[4,0]` | `KC_LGUI`<br>`m[4,1]` | `KC_LALT`<br>`m[4,2]` | `MO(1)`<br>`m[4,3]` |  |  | `KC_SPC`<br>`m[4,4]` |  | `KC_SPC`<br>`m[9,4]` |  |  | `KC_SPC`<br>`m[9,3]` | `KC_RALT`<br>`m[9,2]` | `KC_APP`<br>`m[9,1]` | `KC_LCTL`<br>`m[9,0]` |
| 5 |  |  |  |  | `KC_SPC`<br>`m[4,5]` | `KC_SPC`<br>`m[4,6]` |  |  |  | `KC_SPC`<br>`m[9,6]` | `KC_SPC`<br>`m[9,5]` |  |  |  |  |

## ErgoDash

| prow | L0 | L1 | L2 | L3 | L4 | L5 | L6 |  | R6 | R5 | R4 | R3 | R2 | R1 | R0 |
|---:|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 0 | `KC_ESC`<br>`m[0,0]` | `KC_1`<br>`m[0,1]` | `KC_2`<br>`m[0,2]` | `KC_3`<br>`m[0,3]` | `KC_4`<br>`m[0,4]` | `KC_5`<br>`m[0,5]` | `KC_6`<br>`m[0,6]` |  | `KC_EQL`<br>`m[5,6]` | `KC_7`<br>`m[5,5]` | `KC_8`<br>`m[5,4]` | `KC_9`<br>`m[5,3]` | `KC_0`<br>`m[5,2]` | `KC_MINS`<br>`m[5,1]` | `KC_BSLS`<br>`m[5,0]` |
| 1 | `KC_TAB`<br>`m[1,0]` | `KC_Q`<br>`m[1,1]` | `KC_W`<br>`m[1,2]` | `KC_E`<br>`m[1,3]` | `KC_R`<br>`m[1,4]` | `KC_T`<br>`m[1,5]` | `KC_GRV`<br>`m[1,6]` |  | `KC_QUOT`<br>`m[6,6]` | `KC_Y`<br>`m[6,5]` | `KC_U`<br>`m[6,4]` | `KC_I`<br>`m[6,3]` | `KC_O`<br>`m[6,2]` | `KC_P`<br>`m[6,1]` | `KC_LBRC`<br>`m[6,0]` |
| 2 | `KC_LGUI`<br>`m[2,0]` | `KC_A`<br>`m[2,1]` | `KC_S`<br>`m[2,2]` | `KC_D`<br>`m[2,3]` | `KC_F`<br>`m[2,4]` | `KC_G`<br>`m[2,5]` | `KC_ESC`<br>`m[2,6]` |  | `KC_ASTR`<br>`m[7,6]` | `KC_H`<br>`m[7,5]` | `KC_J`<br>`m[7,4]` | `KC_K`<br>`m[7,3]` | `KC_L`<br>`m[7,2]` | `KC_SCLN`<br>`m[7,1]` | `KC_RBRC`<br>`m[7,0]` |
| 3 | `KC_RCBR`<br>`m[3,0]` | `KC_LSFT`<br>`m[3,1]` | `KC_Z`<br>`m[3,2]` | `KC_X`<br>`m[3,3]` | `KC_C`<br>`m[3,4]` | `KC_V`<br>`m[3,5]` | `KC_B`<br>`m[3,6]` |  | `KC_PERC`<br>`m[8,6]` | `KC_N`<br>`m[8,5]` | `KC_M`<br>`m[8,4]` | `KC_COMM`<br>`m[8,3]` | `KC_DOT`<br>`m[8,2]` | `KC_SLSH`<br>`m[8,1]` | `KC_UP`<br>`m[8,0]` |
| 4 | `KC_ENT`<br>`m[4,0]` | `KC_BSPC`<br>`m[4,1]` | `KC_DEL`<br>`m[4,2]` | `KC_LALT`<br>`m[4,3]` | `KC_LSFT`<br>`m[4,4]` | `KC_LCTL`<br>`m[4,5]` | `KC_SPC`<br>`m[4,6]` |  | `KC_SPC`<br>`m[9,4]` | `KC_LSFT`<br>`m[9,5]` | `KC_LALT`<br>`m[9,6]` | `KC_LCTL`<br>`m[9,3]` | `KC_LEFT`<br>`m[9,2]` | `KC_DOWN`<br>`m[9,1]` | `KC_RGHT`<br>`m[9,0]` |
| 5 |  |  |  |  | `LOWER`<br>`m[4,4]` | `KC_SPC`<br>`m[4,5]` |  |  |  | `KC_SPC`<br>`m[9,4]` | `KC_LSFT`<br>`m[9,5]` |  |  |  |  |

## Thumb-Only Diff

| position | Ergo68 | ErgoDash |
|---|---|---|
| left thumb upper-1 | none | `KC_LSFT`<br>`m[4,4]` |
| left thumb upper-2 | none | `KC_LCTL`<br>`m[4,5]` |
| right thumb upper-1 | none | `KC_SPC`<br>`m[9,4]` |
| right thumb upper-2 | none | `KC_LSFT`<br>`m[9,5]` |

注記:

- 以前の 1 マスに `KC_SPC m[4,4] / m[4,5] / m[4,6]` をまとめた書き方は誤り
- これはレイヤーではなく、複数の物理キーを 1 セルに詰めてしまっていた
- このファイルでは `top layer` のみを、`1セル = 1物理キー` で書いている
