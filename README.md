# ke_complex-rules

This repo includes custom complex modification rules for [karabiner-elements](https://karabiner-elements.pqrs.org/) to customize key strokes.

The CapsLock key is modified to be used as a virtual modifier and in order to use the virtual modifier, the mandatory rules MUST be enabled.

The following keys are used as virtual modifiers.

- CapsLock
- Tab

The following modes can be enabled by hitting extra dedicated keys while CapsLock is pressed.

- Launcher mode : Enter
- Window control mode : Right command
- Mouse key mode : Right shift

## Import rules

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
| [CustomTab_Base](https://raw.githubusercontent.com/seungbemi/ke_complex-rules/master/CustomTab_Base.json) | Ruleset using tab as a modifier |

## CustomCapslock Basic

The following keys are modified while the Capslock key is being pressed.

e.g. CAPSLOCK(pressed) + i -> Arrow Up

### Virtual Modifier

| FROM | TO |
| - | - |
| CapsLock | Virtual Modifier |
| 5 | CapsLock |

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
| Right Option(without capslock) | fn key |

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

The launcher mode can be initiated by striking enter while the capslock key is being pressed.

e.g. `CAPSLOCK(pressed) + ENTER(down/up) + c -> open Chrome`

| FROM | Application |
| - | - |
| b | Brave Browser |
| c | Chrome Browser |
| d | Dock (CTRL + f3) |
| f | Forklift |
| g | Micorsoft Edge |
| i | Safari |
| j | Menu (CTRL + f2)
| k | KakaoTalk |
| m | Messages |
| p | Spark |
| s | Slack |
| t | iTerm2 |
| v | VSCode |
| w | WhatsApp |

## Window Control Mode

This Window Control Mode requires a tool called [Better Touch Tool](https://folivora.ai/). And it is desired to be configured to work properly.

The mode can be initiated by striking right command key while the capslock key is being pressed.

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

### Click

| FROM | TO |
| - | - |
| v | Left click |
| c | CMD + Left click |
| b | Right click |

### Speed control

The speed will change while pressing the following keys.

| FROM | TO |
| - | - |
| s | Slower cursor speed |
| d | Faster cursor speed |
| f | Even Faster cursor speed |

### Common keys

| FROM | TO |
| - | - |
| h | Prev Page |
| semicolon(;) | Next Page |
| e | Escape |

## Custom Tab Basic

The tab key is pressed solo, it's used as the tab. But it's going to be used as a virtual key when it's pressed with the following keys.

e.g. tab(alone) -> tab, tab + q -> previous application

### Switch application

| FROM | TO |
| - | - |
| q | Prev application |
| w | Next application |

### Number pad

| FROM | TO |
| - | - |
| o | 9 |
| i | 8 |
| u | 7 |
| l | 6 |
| k | 5 |
| j | 4 |
| comma(,) | 3 |
| o | 2 |
| i | 1 |
| Space | 0 |
