# ke_complex-rules

This repo includes custom complex modification rules for [karabiner-elements](https://karabiner-elements.pqrs.org/) to customize key strokes.

The CapsLock key is modified to be used as a virtual modifier. To use the virtual modifier, make sure to enable the mandatory rules.

The following keys are used as virtual modifiers:

- CapsLock
- Right Command

While holding down the CapsLock key, you can activate the following modes by pressing additional dedicated keys:

- Launcher mode: Enter
- Window control mode: Right Command
- Mouse key mode: Right Shift

## Importing Rules

The detailed instructions can be found in [karabiner-elements](https://github.com/pqrs-org/KE-complex_modifications#import-file-from-another-site).

In order to import the rules, fill `<Rule URL>` and open the link in a web browser.
> karabiner://karabiner/assets/complex_modifications/import?url=`<Rule URL>`

Or

The ruleset files can directly be copied under
> $HOME/.config/karabiner/assets/complex_modifications/

Rule URLs can be copied from the following list.

| URL | Description |
|-----------------------------------|---------------------------------------|
| [CustomCapslock_Base](https://raw.githubusercontent.com/seungbemi/ke_complex-rules/master/CustomCapslock_Base.json) | Ruleset for basic custom capslock |
| [CustomCapslock_iTerm2](https://raw.githubusercontent.com/seungbemi/ke_complex-rules/master/CustomCapslock_iTerm2.json) | Ruleset for iTerms2 |
| [CustomCapslock_VSCode](https://raw.githubusercontent.com/seungbemi/ke_complex-rules/master/CustomCapslock_VSCode.json) | Ruleset for VSCode |
| [CustomCapslock_LauncherMode](https://raw.githubusercontent.com/seungbemi/ke_complex-rules/master/CustomCapslock_LauncherMode.json)| Ruleset to launch applications |
| [CustomCapslock_WindowCtrlMode](https://raw.githubusercontent.com/seungbemi/ke_complex-rules/master/CustomCapslock_WindowCtrlMode.json) | Ruleset to control activated window |
| [CustomCapslock_MouseKeyMode](https://raw.githubusercontent.com/seungbemi/ke_complex-rules/master/CustomCapslock_MouseKeyMode.json) | Ruleset to use mouse using keyboard |
| [CustomSpacebar_Base](https://raw.githubusercontent.com/seungbemi/ke_complex-rules/master/CustomSpacebar_Base.json) | Ruleset using spacebar as a modifier |

## CustomCapslock Basic

The following keys are modified while the Capslock key is being pressed to provide additional functionalities.

e.g. CAPSLOCK(pressed) + i -> Arrow Up

### Virtual Modifier

| FROM | TO |
| - | - |
| CapsLock | Virtual Modifier |
| 5 | CapsLock |

### Home Row Modifier

| FROM | TO |
| - | - |
| a + other keys | CTRL |
| s + other keys | SHIFT |
| d + other keys | OPTION |
| f + other keys | CMD |

### Diamond cursor

| FROM | TO |
| - | - |
| i | Arrow up |
| j | Arrow left |
| k | Arrow down |
| l | Arrow right|

### Home/End

| FROM | TO |
| - | - |
| h | Home |
| semicolon(;) | End |

### Delete keys

| FROM | TO |
| - | - |
| u | Delete |
| o | Delete foward |

### Page Up/Down

| FROM | TO |
| - | - |
| p | Page up |
| quote(') | Page down |

### Tab Mover

| FROM | TO |
| - | - |
| 7 | Move left tab (CMD+SHIFT+[) |
| 8 | Move right tab (CMD+SHIFT+]) |
| Open bracket([) | Move left tab (CMD+SHIFT+[) |
| Close bracket(]) | Move right tab (CMD+SHIFT+]) |

### Windowslike redo

| FROM | TO |
| - | - |
| y | Redo (CMD+SHIFT+z) |

### Enter

| FROM | TO |
| - | - |
| Space | Enter |

### Escape

| FROM | TO |
| - | - |
| e | Escape |

### Replace Command key

| FROM | TO |
| - | - |
| q | CMD + q |
| CMD + w  | CMD + SHIFT + w |
| w | CMD + w |
| CMD + r | CMD + SHIFT + r |
| r | CMD + r |
| CMD + t | CMD + SHIFT + t |
| t | CMD + t |
| a | CMD + a |
| s | CMD + s |
| f | CMD + f |
| z | CMD + z |
| x | CMD + x |
| c | CMD + c |
| v | CMD + v |
| 0 | CMD + 0 |
| hypen(-) | CMD + - |
| equal(=) | CMD + = |

### Extra

| FROM | TO |
| - | - |
| 9 | Next window |
| g | Select a word |
| Tab | SHIFT+Tab |
| d | [DeepL](https://www.deepl.com/pro?cta=header-pro) app |
| Right CMD(without capslock) | Switch Input language |

### VSCode

The following bindings are only enabled in VSCode application.

| FROM | TO |
| - | - |
| b | Go Back (CTRL + hypen) |
| n | Go Foward (CTRL + SHIFT + hypen) |
| m | Go to Definition (f12) |
| CMD + m | Go to References (SHIFT + f12) |
| OPTION + m | Go to Implementation (CMD + f12) |
| comma(,) | Next Problem (f8) |
| period(.)| Expand Selection |
| CMD + period | Shrink Selection |
| Slash(/) | Toggle line comment |

### iTerm

The following bindings are only enabled in iTerm application.
| FROM | TO |
| - | - |
| r | CTRL + r |

## Launcher Mode

The launcher mode can be initiated by pressing the Enter key while the Caps Lock key is being held down. This mode allows you to quickly open applications by combining the Caps Lock key with other keys.

e.g. `CAPSLOCK(pressed) + ENTER(down/up) + c -> open Chrome`

| FROM | Application |
| - | - |
| b | Brave Browser |
| c | Chrome Browser |
| d | Dock (CTRL + f3) |
| f | Forklift |
| g | Micorsoft Edge |
| i | Safari |
| j | Menu (CTRL + f2)|
| k | KakaoTalk |
| m | Messages |
| p | Spark |
| s | Slack |
| t | iTerm2 |
| v | VSCode |
| w | WhatsApp |

## Window Control Mode

This Window Control Mode requires the use of [Better Touch Tool](https://folivora.ai/) to be properly configured.

To activate this mode, press the right command key while holding down the Caps Lock key.

e.g. `CAPSLOCK(pressed) + R_COMMAND(down/up) + m -> maximize window`

### Mission control

| FROM | TO |
| - | - |
| i | Mission control  |
| j | Move left a sapce |
| k | Application Window |
| l | Move right a space |
| d | Show desktop |

### Switch desktop

| FROM | TO |
| - | - |
| 1 | Move to Desktop 1 |
| 2 | Move to Desktop 2 |
| 3 | Move to Desktop 3 |
| 4 | Move to Desktop 4 |

### Move activated window

| FROM | TO |
| - | - |
| CMD + j | Move activated window to a left space |
| CMD + l | Move activated window to a right space |
| n | Move activated window to a next monitor |

### Window snapping

| FROM | TO |
| - | - |
| h | Resize window to left Half |
| semicolon(;) | Resize window to right half |
| t | Resize window to top half |
| b | Resize window to bottom half |
| u | Resizee window to left two thirds |
| o | Resize window to right two thirds |
| m | Resize window to max |
| f | Resize window to middle |
| r | Revert window size |

## Mouse Key Mode

The Mouse Key Mode can be initiated by striking right shift key while the capslock key is being pressed.

### Move Cursor

| FROM | TO |
| - | - |
| i | Move cursor up  |
| j | Move cursor left |
| k | Move cursor down |
| l | Move cursor right |

### Scroll

| FROM | TO |
| - | - |
| u | Scroll left |
| o | Scroll right |
| p | Scroll up |
| quote(') | Scroll down |
| y | Scroll up |
| n | Scroll down |

### Click

| FROM | TO |
| - | - |
| v | Left click |
| g | CMD + Left click |
| b | Right click |

### Speed control

The speed will change while pressing the following keys.

| FROM | TO |
| - | - |
| s | Slower cursor speed |
| d | Faster cursor speed |
| f | Even Faster cursor speed |

### Page Navigation

| FROM | TO |
| - | - |
| h | Prev Page |
| semicolon(;) | Next Page |

### Tab Navigation

| FROM | TO |
| - | - |
| m | Move left tab (CMD+SHIFT+[) |
| comma(,) | Move right tab (CMD+SHIFT+]) |

### Common keys

| FROM | TO |
| - | - |
| e | Escape |
| r | Refresh (CMD + R)  |

## Custom Right Command Basic

The following keys are modified while the Right Command key is being pressed to be able to have a layer with fullset of symbols without using the shift key.

e.g. right command(alone) -> right command, right command + q -> !, right command + w -> @

### Symbol Mapping

- Top Row

| FROM | TO |
| - | - |
| q | ` |
| w | @ |
| e | # |
| r | $ |
| t | % |
| y | ^ |
| u | & |
| i | * |
| o | \ |
| p | \| |
| \[ | " |

- Home Row

| FROM | TO |
| - | - |
| a | [ |
| s | ] |
| d | ( |
| f | ) |
| g | ? |
| h | _ |
| j | - |
| k | = |
| l | : |
| ; | ; |
| ' | ' |

- Bottom Row

| FROM | TO |
| - | - |
| z | < |
| x | > |
| c | { |
| v | } |
| b | ! |
| n | ~ |
| m | + |
| , | , |
| . | . |
| / | / |

## Base Key Mapping

These are the base key mappings that are used without any virtual modifiers.

| FROM | TO |
| - | - |
| keyboard layout | [colemak-dh matrix layout](https://colemakmods.github.io/mod-dh/keyboards.html#matrix-keyboards) |
| home | CMD + left |
| end | CMD + right |
| left command + delete_forward | delete all left of cursor |
| right option | fn key |
| left command + e | open PastePal (CMD + SHIFT + v) |
