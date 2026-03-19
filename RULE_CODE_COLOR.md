# VS Code Theme - Complete Color Attributes Reference

> _Checklist + danh mục “attributes/keys” chuẩn để thiết kế theme VS Code ( đầy đủ workbench colors, token colors, semantic tokens).

---

## Mục lục Checklist

1. [Semantic Token Colors](#1-semantic-token-colors)
2. [Colors (UI Colors)](#2-colors-ui-colors)
   - [2.1 Editor - Background & Foreground](#21-editor---background--foreground)
   - [2.2 Editor - Bracket Pair Colorization](#22-editor---bracket-pair-colorization)
   - [2.3 Editor - Gutter](#23-editor---gutter)
   - [2.4 Editor - Overview Ruler](#24-editor---overview-ruler)
   - [2.5 Editor - Errors & Warnings](#25-editor---errors--warnings)
   - [2.5 Editor - Diff Editor](#25-editor---diff-editor)
   - [2.6 Editor - Minimap & Scrollbar](#26-editor---minimap--scrollbar)
   - [2.7 Editor - Widgets](#27-editor---widgets)
   - [2.8 Workbench - Title Bar](#28-workbench---title-bar)
   - [2.9 Workbench - Peek View](#29-workbench---peek-view)
   - [2.10 Workbench - Activity Bar](#210-workbench---activity-bar)
   - [2.11 Workbench - Side Bar](#211-workbench---side-bar)
   - [2.12 Workbench - List & Trees](#212-workbench---list--trees)
   - [2.13 Workbench - Tabs](#213-workbench---tabs)
   - [2.15 Workbench - Breadcrumb](#215-workbench---breadcrumb)
   - [2.16 Workbench - Status Bar](#216-workbench---status-bar)
   - [2.17 Workbench - Panel](#217-workbench---panel)
   - [2.17 Terminal](#217-terminal)
   - [2.18 Input & Dropdown](#218-input--dropdown)
   - [2.19 Button & Badge](#219-button--badge)
   - [2.20 Git Decorations](#220-git-decorations)
   - [2.21 Debug](#221-debug)
   - [2.22 Testing](#222-testing)
   - [2.23 Command Center & Quick Input](#223-command-center--quick-input)
   - [2.24 Check Box & Progress Bar & Ports](#224-check-box--progress-bar--ports)
   - [2.25 Notification](#225-notification)
   - [2.26 Merge Conflicts](#226-merge-conflicts)
   - [2.27 Welcome Page](#227-welcome-page)
   - [2.28 Setting](#228-setting)
   - [2.29 Extension](#229-extension)
   - [2.30 Symbol Icons](#230-symbol-icons)
   - [2.31 Charts & Misc](#231-charts--misc)
3. [Token Colors (Syntax Highlighting)](#3-token-colors-syntax-highlighting)
   - [3.1 Comments](#31-comments)
   - [3.2 Keywords & Tags](#32-keywords--tags)
   - [3.3 Numbers & Booleans](#33-numbers--booleans)
   - [3.4 Function Parameters](#34-function-parameters)
   - [3.5 Strings](#35-strings)
   - [3.6 Functions](#36-functions)
   - [3.7 Regex & Language Functions](#37-regex--language-functions)
   - [3.8 Object](#38-object)
   - [3.9 Function & Css Names](#39-function--css-names)
   - [3.10 Control Keywords & Storage](#310-control-keywords--storage)
   - [3.11 Variables & Classes](#311-variables--classes)
   - [3.12 Editor](#312-editor)
   - [3.13 Markdown Text & OPERATORS & PUNCTUATION](#313-markdown-text--operators--punctuation)
   - [3.14 SPECIAL MARKDOWN](#314-special-markdown)
   - [3.15 Language-Specific](#315-language-specific)

**TOTAL**: ~220+ workbench colors + 100+ token scopes

---

## 1. Semantic Token Colors

```json
"semanticTokenColors": {
	"parameter": "#COLOR",
	"parameter.declaration": "#COLOR",
	"variable": "#COLOR",
	"variable.readonly": "#COLOR",
	"variable.defaultLibrary": "#COLOR",
	"variable.declaration": "#COLOR",
	"property": "#COLOR",
	"property.readonly": "#COLOR",
	"property.declaration": "#COLOR",
	"property.defaultLibrary": "#COLOR",
	"function": "#COLOR",
	"method": "#COLOR",
	"class": "#COLOR",
	"interface": "#COLOR",
	"type": "#COLOR",
	"enum": "#COLOR",
	"enumMember": "#COLOR",
	"namespace": "#COLOR",
}
```

**Hỗ trợ LSP semantic tokens để tô màu chính xác hơn theo ngữ cảnh.**

---

## 2. Colors (UI Colors)

### 2.1 Editor - Background & Foreground

```json
	"editor.background": "#COLOR",
	"editor.foreground": "#COLOR",
	"editor.selectionBackground": "#COLOR",
	"editor.selectionHighlightBackground": "#COLOR",
	"editor.inactiveSelectionBackground": "#COLOR",
	"editor.wordHighlightBackground": "#COLOR",
	"editor.wordHighlightStrongBackground": "#COLOR",
	"editor.findMatchBackground": "#COLOR",
	"editor.findMatchHighlightBackground": "#COLOR",
	"editor.hoverHighlightBackground": "#COLOR",
	"editor.lineHighlightBackground": "#COLOR"
	"editor.lineHighlightBorder": "#COLOR",
	"editor.rangeHighlightBackground": "#COLOR",
	"editorLineNumber.foreground": "#COLOR",
	"editorLineNumber.activeForeground": "#COLOR",
	"editorCursor.foreground": "#COLOR",
	"editorWhitespace.foreground": "#COLOR",
	"editorIndentGuide.background": "#COLOR",
	"editorIndentGuide.activeBackground": "#COLOR",
	"editorRuler.foreground": "#COLOR",
	"editorBracketMatch.background": "#COLOR",
	"editorBracketMatch.border": "#COLOR",
```

**Nền tối với độ tương phản vừa phải, giảm mỏi mắt khi code lâu.**

### 2.2 Editor - Bracket Pair Colorization

```json
	"editorBracketHighlight.foreground1": "#COLOR",
	"editorBracketHighlight.foreground2": "#COLOR",
	"editorBracketHighlight.foreground3": "#COLOR",
	"editorBracketHighlight.foreground4": "#COLOR",
	"editorBracketHighlight.foreground5": "#COLOR",
	"editorBracketHighlight.foreground6": "#COLOR",
	"editorBracketHighlight.unexpectedBracket.foreground": "#COLOR",
```

**6 màu cho 6 cấp độ ngoặc lồng nhau, giúp dễ dàng phân biệt cặp ngoặc.**

### 2.3 Editor - Gutter

```json
	"editorGutter.background": "#COLOR",
	"editorGutter.modifiedBackground": "#COLOR",
	"editorGutter.addedBackground": "#COLOR",
	"editorGutter.deletedBackground": "#COLOR",
	"editorGutter.commentRangeForeground": "#COLOR",
	"editorGutter.foldingControlForeground": "#COLOR",
```

**Hiển thị trạng thái Git diff ở bên trái editor.**

### 2.4 Editor - Overview Ruler

```json
	"editorOverviewRuler.border": "#COLOR",
	"editorOverviewRuler.findMatchForeground": "#COLOR",
	"editorOverviewRuler.rangeHighlightForeground": "#COLOR",
	"editorOverviewRuler.selectionHighlightForeground": "#COLOR",
	"editorOverviewRuler.wordHighlightForeground": "#COLOR",
	"editorOverviewRuler.wordHighlightStrongForeground": "#COLOR",
	"editorOverviewRuler.modifiedForeground": "#COLOR",
	"editorOverviewRuler.addedForeground": "#COLOR",
	"editorOverviewRuler.deletedForeground": "#COLOR",
	"editorOverviewRuler.errorForeground": "#COLOR",
	"editorOverviewRuler.warningForeground": "#COLOR",
	"editorOverviewRuler.infoForeground": "#COLOR",
```

### 2.5 Editor - Errors & Warnings

```json
	"editorError.foreground": "#COLOR",
	"editorWarning.foreground": "#COLOR",
	"editorInfo.foreground": "#COLOR",
	"editorHint.foreground": "#COLOR",
	"problemsErrorIcon.foreground": "#COLOR",
	"problemsWarningIcon.foreground": "#COLOR",
	"problemsInfoIcon.foreground": "#COLOR",
```

### 2.5 Editor - Diff Editor

```json
	"diffEditor.insertedTextBackground": "#COLOR",
	"diffEditor.insertedLineBackground": "#COLOR",
	"diffEditor.removedTextBackground": "#COLOR",
	"diffEditor.removedLineBackground": "#COLOR",
	"diffEditor.border": "#COLOR",
	"diffEditor.diagonalFill": "#COLOR",
	"diffEditorGutter.insertedLineBackground": "#COLOR",
	"diffEditorGutter.removedLineBackground": "#COLOR",
```

**Độ trong suốt 20% để không quá nổi bật khi xem diff.**

### 2.6 Editor - Minimap & Scrollbar

```json
	"minimap.findMatchHighlight": "#COLOR",
	"minimap.selectionHighlight": "#COLOR",
	"minimap.errorHighlight": "#COLOR",
	"minimap.warningHighlight": "#COLOR",
	"minimap.background": "#COLOR",
	"minimap.hoverBackground": "#COLOR",
	"minimap.activeBackground": "#COLOR",
	"minimap.addedBackground": "#COLOR",
	"minimap.modifiedBackground": "#COLOR",
	"minimap.deletedBackground": "#COLOR",
	"scrollbar.shadow": "#COLOR",
	"scrollbarSlider.background": "#COLOR",
	"scrollbarSlider.hoverBackground": "#COLOR",
	"scrollbarSlider.activeBackground": "#COLOR",
```

**Minimap background: cùng màu editor; Scrollbar: với độ trong suốt khác nhau cho các trạng thái**

### 2.7 Editor - Widgets

```json
	"editorWidget.background": "#COLOR",
	"editorWidget.foreground": "#COLOR",
	"editorWidget.border": "#COLOR",
	"editorWidget.resizeBorder": "#COLOR",
	"editorSuggestWidget.background": "#COLOR",
	"editorSuggestWidget.border": "#COLOR",
	"editorSuggestWidget.foreground": "#COLOR",
	"editorSuggestWidget.highlightForeground": "#COLOR",
	"editorSuggestWidget.selectedBackground": "#COLOR",
	"editorSuggestWidget.focusHighlightForeground": "#COLOR",
	"editorSuggestWidget.selectedForeground": "#COLOR",
	"editorSuggestWidget.selectedIconForeground": "#COLOR",
	"editorHoverWidget.background": "#COLOR",
	"editorHoverWidget.border": "#COLOR",
	"editorHoverWidget.foreground": "#COLOR",
	"editorHoverWidget.highlightForeground": "#COLOR",
	"editorHoverWidget.statusBarBackground": "#COLOR",
```

**Các popup như autocomplete**

### 2.8 Workbench - Title Bar

```json
	"titleBar.activeBackground": "#COLOR",
	"titleBar.activeForeground": "#COLOR",
	"titleBar.inactiveBackground": "#COLOR",
	"titleBar.inactiveForeground": "#COLOR",
	"titleBar.border": "#COLOR",
```

### 2.9 Workbench - Peek View

```json
	"peekView.border": "#COLOR",
	"peekViewEditor.background": "#COLOR",
	"peekViewEditor.matchHighlightBackground": "#COLOR",
	"peekViewEditor.matchHighlightBorder": "#COLOR",
	"peekViewEditorGutter.background": "#COLOR",
	"peekViewResult.background": "#COLOR",
	"peekViewResult.fileForeground": "#COLOR",
	"peekViewResult.lineForeground": "#COLOR",
	"peekViewResult.matchHighlightBackground": "#COLOR",
	"peekViewResult.selectionBackground": "#COLOR",
	"peekViewResult.selectionForeground": "#COLOR",
	"peekViewTitle.background": "#COLOR",
	"peekViewTitleDescription.foreground": "#COLOR",
	"peekViewTitleLabel.foreground": "#COLOR",
```

### 2.10 Workbench - Activity Bar

```json
	"activityBar.background": "#COLOR",
	"activityBar.foreground": "#COLOR",
	"activityBar.inactiveForeground": "#COLOR",
	"activityBar.border": "#COLOR",
	"activityBar.activeBorder": "#COLOR",
	"activityBar.activeBackground": "#COLOR",
	"activityBarBadge.background": "#COLOR",
	"activityBarBadge.foreground": "#COLOR",
```

### 2.11 Workbench - Side Bar

```json
	"sideBar.background": "#COLOR",
	"sideBar.foreground": "#COLOR",
	"sideBar.border": "#COLOR",
	"sideBar.dropBackground": "#COLOR",
	"sideBarTitle.foreground": "#COLOR",
	"sideBarSectionHeader.background": "#COLOR",
	"sideBarSectionHeader.foreground": "#COLOR",
	"sideBarSectionHeader.border": "#COLOR",
```

### 2.12 Workbench - List & Trees

```json
	"list.activeSelectionBackground": "#COLOR",
	"list.activeSelectionForeground": "#COLOR",
	"list.activeSelectionIconForeground": "#COLOR",
	"list.inactiveSelectionBackground": "#COLOR",
	"list.inactiveSelectionForeground": "#COLOR",
	"list.inactiveSelectionIconForeground": "#COLOR",
	"list.hoverBackground": "#COLOR",
	"list.hoverForeground": "#COLOR",
	"list.focusBackground": "#COLOR",
	"list.focusForeground": "#COLOR",
	"list.focusOutline": "#COLOR",
	"list.focusAndSelectionOutline": "#COLOR",
	"list.dropBackground": "#COLOR",
	"list.highlightForeground": "#COLOR",
	"list.errorForeground": "#COLOR",
	"list.warningForeground": "#COLOR",
	"list.invalidItemForeground": "#COLOR",
	"list.deemphasizedForeground": "#COLOR",
	"listFilterWidget.background": "#COLOR",
	"listFilterWidget.outline": "#COLOR",
	"listFilterWidget.noMatchesOutline": "#COLOR",
	"tree.indentGuidesStroke": "#COLOR",
	"tree.tableColumnsBorder": "#COLOR",
```

### 2.13 Workbench - Tabs

```json
	"editorGroupHeader.tabsBackground": "#COLOR",
	"editorGroupHeader.tabsBorder": "#COLOR",
	"editorGroupHeader.noTabsBackground": "#COLOR",
	"editorGroupHeader.border": "#COLOR",
	"editorGroup.border": "#COLOR",
	"editorGroup.dropBackground": "#COLOR",
	"editorGroup.emptyBackground": "#COLOR",
	"editorGroup.focusedEmptyBorder": "#COLOR",
	"tab.activeBackground": "#COLOR",
	"tab.activeForeground": "#COLOR",
	"tab.activeBorder": "#COLOR",
	"tab.activeBorderTop": "#COLOR",
	"tab.inactiveBackground": "#COLOR",
	"tab.inactiveForeground": "#COLOR",
	"tab.unfocusedActiveBackground": "#COLOR",
	"tab.unfocusedActiveForeground": "#COLOR",
	"tab.unfocusedActiveBorderTop": "#COLOR",
	"tab.unfocusedInactiveBackground": "#COLOR",
	"tab.unfocusedInactiveForeground": "#COLOR",
	"tab.hoverBackground": "#COLOR",
	"tab.hoverForeground": "#COLOR",
	"tab.border": "#COLOR",
	"tab.lastPinnedBorder": "#COLOR",
	"tab.unfocusedHoverBackground": "#COLOR",
```

**Tab active có border top để dễ nhận biết**

### 2.15 Workbench - Breadcrumb

```json
	"breadcrumb.background": "#COLOR",
	"breadcrumb.foreground": "#COLOR",
	"breadcrumb.focusForeground": "#COLOR",
	"breadcrumb.activeSelectionForeground": "#COLOR",
	"breadcrumbPicker.background": "#COLOR",
```

### 2.16 Workbench - Status Bar

```json
	"statusBar.background": "#COLOR",
	"statusBar.foreground": "#COLOR",
	"statusBar.border": "#COLOR",
	"statusBar.debuggingBackground": "#COLOR",
	"statusBar.debuggingForeground": "#COLOR",
	"statusBar.debuggingBorder": "#COLOR",
	"statusBar.noFolderBackground": "#COLOR",
	"statusBar.noFolderForeground": "#COLOR",
	"statusBar.noFolderBorder": "#COLOR",
	"statusBarItem.activeBackground": "#COLOR",
	"statusBarItem.hoverBackground": "#COLOR",
	"statusBarItem.prominentBackground": "#COLOR",
	"statusBarItem.prominentForeground": "#COLOR",
	"statusBarItem.prominentHoverBackground": "#COLOR",
	"statusBarItem.remoteBackground": "#COLOR",
	"statusBarItem.remoteForeground": "#COLOR",
	"statusBarItem.errorBackground": "#COLOR",
	"statusBarItem.errorForeground": "#COLOR",
	"statusBarItem.warningBackground": "#COLOR",
	"statusBarItem.warningForeground": "#COLOR",
```

### 2.17 Workbench - Panel

```json
	"panel.background": "#COLOR",
	"panel.border": "#COLOR",
	"panel.dropBorder": "#COLOR",
	"panelTitle.activeBorder": "#COLOR",
	"panelTitle.activeForeground": "#COLOR",
	"panelTitle.inactiveForeground": "#COLOR",
	"panelInput.border": "#COLOR",
	"panelSection.border": "#COLOR",
	"panelSection.dropBackground": "#COLOR",
	"panelSectionHeader.background": "#COLOR",
	"panelSectionHeader.foreground": "#COLOR",
	"panelSectionHeader.border": "#COLOR",
```

### 2.17 Terminal

```json
	"terminal.background": "#COLOR",
	"terminal.foreground": "#COLOR",
	"terminal.border": "#COLOR",
	"terminal.selectionBackground": "#COLOR",
	"terminal.inactiveSelectionBackground": "#COLOR",
	"terminalCursor.background": "#COLOR",
	"terminalCursor.foreground": "#COLOR",
	"terminal.ansiBlack": "#COLOR",
	"terminal.ansiRed": "#COLOR",
	"terminal.ansiGreen": "#COLOR",
	"terminal.ansiYellow": "#COLOR",
	"terminal.ansiBlue": "#COLOR",
	"terminal.ansiMagenta": "#COLOR",
	"terminal.ansiCyan": "#COLOR",
	"terminal.ansiWhite": "#COLOR",
	"terminal.ansiBrightBlack": "#COLOR",
	"terminal.ansiBrightRed": "#COLOR",
	"terminal.ansiBrightGreen": "#COLOR",
	"terminal.ansiBrightYellow": "#COLOR",
	"terminal.ansiBrightBlue": "#COLOR",
	"terminal.ansiBrightMagenta": "#COLOR",
	"terminal.ansiBrightCyan": "#COLOR",
	"terminal.ansiBrightWhite": "#COLOR",
	"terminal.findMatchBackground": "#COLOR",
	"terminal.findMatchBorder": "#COLOR",
	"terminal.findMatchHighlightBackground": "#COLOR",
	"terminal.findMatchHighlightBorder": "#COLOR",
	"terminalCommandDecoration.defaultBackground": "#COLOR",
	"terminalCommandDecoration.successBackground": "#COLOR",
	"terminalCommandDecoration.errorBackground": "#COLOR",
	"terminalOverviewRuler.cursorForeground": "#COLOR",
	"terminalOverviewRuler.findMatchForeground": "#COLOR",
```

**Bảng màu terminal đồng nhất với theme, hỗ trợ 16 màu ANSI chuẩn.**

### 2.18 Input & Dropdown

```json
	"input.background": "#COLOR",
	"input.foreground": "#COLOR",
	"input.border": "#COLOR",
	"input.placeholderForeground": "#COLOR",
	"inputOption.activeBackground": "#COLOR",
	"inputOption.activeBorder": "#COLOR",
	"inputOption.activeForeground": "#COLOR",
	"inputOption.hoverBackground": "#COLOR",
	"inputValidation.errorBackground": "#COLOR",
	"inputValidation.errorBorder": "#COLOR",
	"inputValidation.errorForeground": "#COLOR",
	"inputValidation.infoBackground": "#COLOR",
	"inputValidation.infoBorder": "#COLOR",
	"inputValidation.infoForeground": "#COLOR",
	"inputValidation.warningBackground": "#COLOR",
	"inputValidation.warningBorder": "#COLOR",
	"inputValidation.warningForeground": "#COLOR",
	"dropdown.background": "#COLOR",
	"dropdown.foreground": "#COLOR",
	"dropdown.border": "#COLOR",
	"dropdown.listBackground": "#COLOR",
```

### 2.19 Button & Badge

```json
	"button.background": "#COLOR",
	"button.foreground": "#COLOR",
	"button.hoverBackground": "#COLOR",
	"button.secondaryBackground": "#COLOR",
	"button.secondaryForeground": "#COLOR",
	"button.secondaryHoverBackground": "#COLOR",
	"button.border": "#COLOR",
	"badge.background": "#COLOR",
	"badge.foreground": "#COLOR",
```

### 2.20 Git Decorations

```json
	"gitDecoration.addedResourceForeground": "#COLOR",
	"gitDecoration.modifiedResourceForeground": "#COLOR",
	"gitDecoration.deletedResourceForeground": "#COLOR",
	"gitDecoration.renamedResourceForeground": "#COLOR",
	"gitDecoration.stageModifiedResourceForeground": "#COLOR",
	"gitDecoration.stageDeletedResourceForeground": "#COLOR",
	"gitDecoration.untrackedResourceForeground": "#COLOR",
	"gitDecoration.ignoredResourceForeground": "#COLOR",
	"gitDecoration.conflictingResourceForeground": "#COLOR",
	"gitDecoration.submoduleResourceForeground": "#COLOR",
```

### 2.21 Debug

```json
	"debugToolBar.background": "#COLOR",
	"debugToolBar.border": "#COLOR",
	"debugIcon.breakpointForeground": "#COLOR",
	"debugIcon.breakpointDisabledForeground": "#COLOR",
	"debugIcon.breakpointUnverifiedForeground": "#COLOR",
	"debugIcon.breakpointCurrentStackframeForeground": "#COLOR",
	"debugIcon.breakpointStackframeForeground": "#COLOR",
	"debugIcon.startForeground": "#COLOR",
	"debugIcon.pauseForeground": "#COLOR",
	"debugIcon.stopForeground": "#COLOR",
	"debugIcon.disconnectForeground": "#COLOR",
	"debugIcon.restartForeground": "#COLOR",
	"debugIcon.stepOverForeground": "#COLOR",
	"debugIcon.stepIntoForeground": "#COLOR",
	"debugIcon.stepOutForeground": "#COLOR",
	"debugIcon.continueForeground": "#COLOR",
	"debugIcon.stepBackForeground": "#COLOR",
	"debugConsole.infoForeground": "#COLOR",
	"debugConsole.warningForeground": "#COLOR",
	"debugConsole.errorForeground": "#COLOR",
	"debugConsole.sourceForeground": "#COLOR",
	"debugConsoleInputIcon.foreground": "#COLOR",
	"debugTokenExpression.name": "#COLOR",
	"debugTokenExpression.value": "#COLOR",
	"debugTokenExpression.string": "#COLOR",
	"debugTokenExpression.boolean": "#COLOR",
	"debugTokenExpression.number": "#COLOR",
	"debugTokenExpression.error": "#COLOR",
```

### 2.22 Testing

```json
	"testing.iconFailed": "#COLOR",
	"testing.iconErrored": "#COLOR",
	"testing.iconPassed": "#COLOR",
	"testing.iconQueued": "#COLOR",
	"testing.iconUnset": "#COLOR",
	"testing.iconSkipped": "#COLOR",
	"testing.runAction": "#COLOR",
	"testing.peekBorder": "#COLOR",
	"testing.peekHeaderBackground": "#COLOR",
	"testing.message.error.decorationForeground": "#COLOR",
	"testing.message.error.lineBackground": "#COLOR",
	"testing.message.info.decorationForeground": "#COLOR",
```

### 2.23 Command Center & Quick Input

```json
	"commandCenter.foreground": "#COLOR",
	"commandCenter.activeForeground": "#COLOR",
	"commandCenter.background": "#COLOR",
	"commandCenter.activeBackground": "#COLOR",
	"commandCenter.border": "#COLOR",
	"commandCenter.inactiveForeground": "#COLOR",
	"commandCenter.inactiveBorder": "#COLOR",
	"commandCenter.activeBorder": "#COLOR",
	"quickInput.background": "#COLOR",
	"quickInput.foreground": "#COLOR",
	"quickInputList.focusBackground": "#COLOR",
	"quickInputList.focusForeground": "#COLOR",
	"quickInputList.focusIconForeground": "#COLOR",
	"quickInputTitle.background": "#COLOR",
	"pickerGroup.border": "#COLOR",
	"pickerGroup.foreground": "#COLOR",
	"keybindingLabel.background": "#COLOR",
	"keybindingLabel.foreground": "#COLOR",
	"keybindingLabel.border": "#COLOR",
	"keybindingLabel.bottomBorder": "#COLOR",
```

### 2.24 Check Box & Progress Bar & Ports

```json
	"checkbox.background": "#1a1b26",
	"checkbox.foreground": "#7aa2f7",
	"checkbox.border": "#3b4261",
	"progressBar.background": "#7aa2f7",
	"ports.iconRunningProcessForeground": "#9ece6a",
```

### 2.25 Notification

```json
	"notifications.background": "#COLOR",
	"notifications.foreground": "#COLOR",
	"notifications.border": "#COLOR",
	"notificationCenter.border": "#COLOR",
	"notificationCenterHeader.background": "#COLOR",
	"notificationCenterHeader.foreground": "#COLOR",
	"notificationToast.border": "#COLOR",
	"notificationsErrorIcon.foreground": "#COLOR",
	"notificationsWarningIcon.foreground": "#COLOR",
	"notificationsInfoIcon.foreground": "#COLOR",
	"notificationLink.foreground": "#COLOR",
```

### 2.26 Merge Conflicts

```json
	"merge.currentHeaderBackground": "#COLOR",
	"merge.currentContentBackground": "#COLOR",
	"merge.incomingHeaderBackground": "#COLOR",
	"merge.incomingContentBackground": "#COLOR",
	"merge.border": "#COLOR",
	"merge.commonHeaderBackground": "#COLOR",
	"merge.commonContentBackground": "#COLOR",
	"editorOverviewRuler.currentContentForeground": "#COLOR",
	"editorOverviewRuler.incomingContentForeground": "#COLOR",
	"editorOverviewRuler.commonContentForeground": "#COLOR",
	"mergeEditor.change.background": "#COLOR",
	"mergeEditor.change.word.background": "#COLOR",
	"mergeEditor.conflict.unhandledUnfocused.border": "#COLOR",
	"mergeEditor.conflict.unhandledFocused.border": "#COLOR",
	"mergeEditor.conflict.handledUnfocused.border": "#COLOR",
	"mergeEditor.conflict.handledFocused.border": "#COLOR",
	"mergeEditor.conflict.handled.minimapOverViewRuler": "#COLOR",
	"mergeEditor.conflict.unhandled.minimapOverViewRuler": "#COLOR",
```

### 2.27 Welcome Page

```json
	"welcomePage.background": "#COLOR",
	"welcomePage.tileBackground": "#COLOR",
	"welcomePage.tileHoverBackground": "#COLOR",
	"welcomePage.tileBorder": "#COLOR",
	"welcomePage.progress.background": "#COLOR",
	"welcomePage.progress.foreground": "#COLOR",
	"walkThrough.embeddedEditorBackground": "#COLOR",
	"walkthrough.stepTitle.foreground": "#COLOR",
```

### 2.28 Setting

```json
	"settings.headerForeground": "#COLOR",
	"settings.modifiedItemIndicator": "#COLOR",
	"settings.dropdownBackground": "#COLOR",
	"settings.dropdownForeground": "#COLOR",
	"settings.dropdownBorder": "#COLOR",
	"settings.dropdownListBorder": "#COLOR",
	"settings.checkboxBackground": "#COLOR",
	"settings.checkboxForeground": "#COLOR",
	"settings.checkboxBorder": "#COLOR",
	"settings.textInputBackground": "#COLOR",
	"settings.textInputForeground": "#COLOR",
	"settings.textInputBorder": "#COLOR",
	"settings.numberInputBackground": "#COLOR",
	"settings.numberInputForeground": "#COLOR",
	"settings.numberInputBorder": "#COLOR",
	"settings.rowHoverBackground": "#COLOR",
	"settings.focusedRowBackground": "#COLOR",
	"settings.focusedRowBorder": "#COLOR",
	"settings.sashBorder": "#COLOR",
```

### 2.29 Extension

```json
	"extensionButton.prominentBackground": "#COLOR",
	"extensionButton.prominentForeground": "#COLOR",
	"extensionButton.prominentHoverBackground": "#COLOR",
	"extensionBadge.remoteBackground": "#COLOR",
	"extensionBadge.remoteForeground": "#COLOR",
	"extensionIcon.starForeground": "#COLOR",
	"extensionIcon.verifiedForeground": "#COLOR",
	"extensionIcon.preReleaseForeground": "#COLOR",
	"extensionIcon.sponsorForeground": "#COLOR",
```

### 2.30 Symbol Icons

```json
	"symbolIcon.arrayForeground": "#COLOR",
	"symbolIcon.booleanForeground": "#COLOR",
	"symbolIcon.classForeground": "#COLOR",
	"symbolIcon.colorForeground": "#COLOR",
	"symbolIcon.constantForeground": "#COLOR",
	"symbolIcon.constructorForeground": "#COLOR",
	"symbolIcon.enumeratorForeground": "#COLOR",
	"symbolIcon.enumeratorMemberForeground": "#COLOR",
	"symbolIcon.eventForeground": "#COLOR",
	"symbolIcon.fieldForeground": "#COLOR",
	"symbolIcon.fileForeground": "#COLOR",
	"symbolIcon.folderForeground": "#COLOR",
	"symbolIcon.functionForeground": "#COLOR",
	"symbolIcon.interfaceForeground": "#COLOR",
	"symbolIcon.keyForeground": "#COLOR",
	"symbolIcon.keywordForeground": "#COLOR",
	"symbolIcon.methodForeground": "#COLOR",
	"symbolIcon.moduleForeground": "#COLOR",
	"symbolIcon.namespaceForeground": "#COLOR",
	"symbolIcon.nullForeground": "#COLOR",
	"symbolIcon.numberForeground": "#COLOR",
	"symbolIcon.objectForeground": "#COLOR",
	"symbolIcon.operatorForeground": "#COLOR",
	"symbolIcon.packageForeground": "#COLOR",
	"symbolIcon.propertyForeground": "#COLOR",
	"symbolIcon.referenceForeground": "#COLOR",
	"symbolIcon.snippetForeground": "#COLOR",
	"symbolIcon.stringForeground": "#COLOR",
	"symbolIcon.structForeground": "#COLOR",
	"symbolIcon.textForeground": "#COLOR",
	"symbolIcon.typeParameterForeground": "#COLOR",
	"symbolIcon.unitForeground": "#COLOR",
	"symbolIcon.variableForeground": "#COLOR",
```

### 2.31 Charts & Misc

```json
	"charts.foreground": "#COLOR",
	"charts.lines": "#COLOR",
	"charts.red": "#COLOR",
	"charts.blue": "#COLOR",
	"charts.yellow": "#COLOR",
	"charts.orange": "#COLOR",
	"charts.green": "#COLOR",
	"charts.purple": "#COLOR",
	"focusBorder": "#COLOR",
	"foreground": "#COLOR",
	"disabledForeground": "#COLOR",
	"widget.shadow": "#COLOR",
	"selection.background": "#COLOR",
	"descriptionForeground": "#COLOR",
	"errorForeground": "#COLOR",
	"icon.foreground": "#COLOR",
	"sash.hoverBorder": "#COLOR"
```

---

## 3. Token Colors (Syntax Highlighting)

### 3.1 Comments

```json
	{
		"name": "Comments",
		"scope": ["comment", "punctuation.definition.comment", "comment.block", "comment.line", "comment.block.documentation"],
		"settings": {
			"foreground": "#565f89",
			"fontStyle": "italic"
		}
	},
```

**Comment màu xám, in nghiêng để phân biệt.**

### 3.2 Keywords & Tags

```json
	{
		"name": "This Keyword",
		"scope": ["variable.language.this", "variable.language.self", "variable.language.super"],
		"settings": {
			"foreground": "#COLOR",
			"fontStyle": "italic"
		}
	},
	{
		"name": "HTML Tags",
		"scope": ["entity.name.tag", "punctuation.definition.tag"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "Regex Group Symbol",
		"scope": ["punctuation.definition.group.regexp", "punctuation.definition.group.assertion.regexp"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "CSS Units",
		"scope": ["keyword.other.unit", "keyword.other.unit.css", "keyword.other.unit.scss", "keyword.other.unit.less"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
```

**Các từ khóa đặc biệt và HTML tags màu đỏ.**

### 3.3 Numbers & Booleans

```json
	{
		"name": "Numbers and Boolean Constants",
		"scope": ["constant.numeric", "constant.language.boolean", "constant.language.true", "constant.language.false", "constant.language.null", "constant.language.undefined", "constant.language.nan"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "Language Support Constants",
		"scope": ["support.constant", "constant.language", "constant.other", "constant.character", "constant.character.escape"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
```

### 3.4 Function Parameters

```json
	{
		"name": "Function Parameters",
		"scope": ["variable.parameter", "meta.function.parameters variable", "meta.parameters variable"],
		"settings": {
			"foreground": "#COLOR",
			"fontStyle": "italic"
		}
	},
	{
		"name": "Regex Character Sets",
		"scope": ["constant.other.character-class.regexp", "constant.character.character-class.regexp", "constant.other.character-class.set.regexp", "punctuation.definition.character-class.regexp"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
```

### 3.5 Strings

```json
	{
		"name": "Strings",
		"scope": ["string", "string.quoted", "string.quoted.single", "string.quoted.double", "string.template", "punctuation.definition.string"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "CSS Class Names",
		"scope": ["entity.other.attribute-name.class", "entity.other.attribute-name.class.css", "entity.other.attribute-name.class.scss"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
```

### 3.6 Functions

```json
	{
		"name": "Object Literal Keys",
		"scope": ["meta.object-literal.key", "support.type.property-name.json", "string.json support.type.property-name"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "Markdown Links",
		"scope": ["markup.underline.link", "markup.underline.link.markdown", "string.other.link.title.markdown", "string.other.link.description.markdown"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
```

### 3.7 Regex & Language Functions

```json
	{
		"name": "Regex Literal Strings",
		"scope": ["string.regexp", "constant.other.character-class.regexp"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "Language Support Functions",
		"scope": ["support.function", "support.function.builtin", "support.function.misc"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "CSS HTML Element Selectors",
		"scope": ["entity.name.tag.css", "entity.name.tag.scss", "entity.name.tag.less", "source.css entity.name.tag", "source.scss entity.name.tag"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
```

### 3.8 Object

```json
	{
		"name": "Object Properties",
		"scope": ["variable.other.property", "variable.other.object.property", "support.variable.property", "meta.property.object"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "Regex Quantifiers and Flags",
		"scope": ["keyword.operator.quantifier.regexp", "string.regexp keyword.other", "keyword.other.flag.regexp"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "Markdown Headings",
		"scope": ["markup.heading", "markup.heading.markdown", "entity.name.section.markdown", "punctuation.definition.heading.markdown"],
		"settings": {
			"foreground": "#COLOR",
			"fontStyle": "bold"
		}
	},
	{
		"name": "Markdown Code",
		"scope": ["markup.inline.raw", "markup.raw.inline.markdown", "markup.fenced_code", "markup.raw.block.markdown"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "Import/Export Keywords",
		"scope": ["keyword.control.import", "keyword.control.export", "keyword.control.from", "keyword.control.as", "keyword.control.default"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
```

### 3.9 Function & Css Names

```json
	{
		"name": "Function Names",
		"scope": ["entity.name.function", "support.function", "meta.function-call entity.name.function", "meta.function entity.name.function"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "CSS Property Names",
		"scope": ["support.type.property-name", "support.type.property-name.css", "support.type.property-name.scss", "meta.property-name.css", "meta.property-name.scss"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "Method Calls",
		"scope": ["meta.method-call entity.name.function", "entity.name.method"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
```

### 3.10 Control Keywords & Storage

```json
	{
		"name": "Control Keywords",
		"scope": ["keyword.control", "keyword.control.conditional", "keyword.control.loop", "keyword.control.flow", "keyword.control.return", "keyword.control.break", "keyword.control.continue", "keyword.control.switch", "keyword.control.case", "keyword.control.try", "keyword.control.catch", "keyword.control.finally", "keyword.control.throw"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "Storage Types",
		"scope": ["storage", "storage.type", "storage.modifier", "keyword.var", "keyword.let", "keyword.const", "keyword.function", "keyword.class", "keyword.interface", "keyword.type", "keyword.async", "keyword.await"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "Regex Symbols and Operators",
		"scope": ["keyword.operator.or.regexp", "keyword.operator.negation.regexp", "punctuation.definition.group.regexp", "constant.other.assertion.regexp"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "HTML Attributes",
		"scope": ["entity.other.attribute-name", "entity.other.attribute-name.html"],
		"settings": {
			"foreground": "#COLOR",
			"fontStyle": "italic"
		}
	},
```

### 3.11 Variables & Classes

```json
	{
		"name": "Variables",
		"scope": ["variable", "variable.other", "variable.other.readwrite", "variable.other.local"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "Class Names",
		"scope": ["entity.name.class", "entity.name.type.class", "support.class", "entity.other.inherited-class"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "Type Names",
		"scope": ["entity.name.type", "support.type", "support.type.primitive"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
```

### 3.12 Editor

```json
	{
		"name": "Editor Foreground",
		"scope": ["source", "text"],
		"settings": {
			"foreground": "#c0caf5"
		}
	},
```

### 3.13 Markdown Text & OPERATORS & PUNCTUATION

```json
	{
		"name": "Markdown Text",
		"scope": ["text.html.markdown", "meta.paragraph.markdown"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "HTML Text",
		"scope": ["text.html", "text.xml"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "Operators",
		"scope": ["keyword.operator", "keyword.operator.arithmetic", "keyword.operator.comparison", "keyword.operator.assignment", "keyword.operator.logical"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "Punctuation",
		"scope": ["punctuation", "punctuation.separator", "punctuation.terminator", "punctuation.accessor", "meta.brace"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
```

### 3.14 SPECIAL MARKDOWN

```json
	{
		"name": "Markdown Bold",
		"scope": ["markup.bold", "punctuation.definition.bold.markdown"],
		"settings": {
			"foreground": "#COLOR",
			"fontStyle": "bold"
		}
	},
	{
		"name": "Markdown Italic",
		"scope": ["markup.italic", "punctuation.definition.italic.markdown"],
		"settings": {
			"foreground": "#COLOR",
			"fontStyle": "italic"
		}
	},
	{
		"name": "Markdown Quote",
		"scope": ["markup.quote", "punctuation.definition.quote.begin.markdown"],
		"settings": {
			"foreground": "#COLOR",
			"fontStyle": "italic"
		}
	},
	{
		"name": "Markdown List",
		"scope": ["markup.list", "punctuation.definition.list.begin.markdown"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
```

### 3.15 Language-Specific

```json
	{
		"name": "CSS ID Selector",
		"scope": ["entity.other.attribute-name.id", "entity.other.attribute-name.id.css"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "CSS Pseudo Classes",
		"scope": ["entity.other.attribute-name.pseudo-class", "entity.other.attribute-name.pseudo-element"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "CSS Property Values",
		"scope": ["support.constant.property-value.css", "support.constant.color.css", "constant.other.color.rgb-value.css", "constant.other.rgb-value.css"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "CSS Variables",
		"scope": ["variable.css", "variable.argument.css", "variable.scss"],
		"settings": {
			"foreground": "#COLOR"
		}
	},

	{
		"name": "TypeScript Types",
		"scope": ["entity.name.type.ts", "entity.name.type.tsx", "support.type.builtin.ts", "support.type.primitive.ts"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "TypeScript Interfaces",
		"scope": ["entity.name.type.interface.ts", "entity.name.type.interface.tsx"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "TypeScript Enums",
		"scope": ["entity.name.type.enum.ts", "entity.name.type.enum.tsx"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "TypeScript Decorators",
		"scope": ["meta.decorator", "punctuation.decorator"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "JSX/TSX Tags",
		"scope": ["support.class.component.tsx", "support.class.component.jsx"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "Python Function Decorators",
		"scope": ["entity.name.function.decorator.python", "meta.function.decorator.python"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "Python Magic Methods",
		"scope": ["support.function.magic.python"],
		"settings": {
			"foreground": "#COLOR",
			"fontStyle": "italic"
		}
	},
	{
		"name": "Rust Lifetimes",
		"scope": ["storage.modifier.lifetime.rust", "entity.name.type.lifetime.rust"],
		"settings": {
			"foreground": "#COLOR",
			"fontStyle": "italic"
		}
	},
	{
		"name": "Rust Macros",
		"scope": ["entity.name.function.macro.rust", "support.macro.rust"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "Go Package Names",
		"scope": ["entity.name.package.go"],
		"settings": {
			"foreground": "#COLOR"
		}
	},
	{
		"name": "Invalid",
		"scope": ["invalid.illegal"],
		"settings": {
			"foreground": "#COLOR",
			"fontStyle": "strikethrough"
		}
	},
	{
		"name": "Deprecated",
		"scope": ["invalid.deprecated"],
		"settings": {
			"foreground": "#COLOR",
			"fontStyle": "strikethrough"
		}
	}
```

---

## Usage Example

```json
{
	"name": "My Custom Theme",
	"type": "dark",
	"semanticTokenColors": {
		"variable": "#COLOR"
	}
	"colors": {
		"editor.background": "#COLOR",
		"editor.foreground": "#COLOR"
	},
	"tokenColors": [
		{
			"scope": ["comment"],
			"settings": {
				"foreground": "#COLOR",
				"fontStyle": "italic"
			}
		}
	],
	
}
```