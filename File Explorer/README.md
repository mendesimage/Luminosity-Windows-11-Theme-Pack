# Luminosity theme for Windows 11 File Explorer Styler

**Author**: [mendes.image](https://github.com/mendesimage)

![Demonstration](nc.png)

## Intro
**Luminosity** is based on native Acrylic, using the maximum **TintLuminosityOpacity** value as its backdrop.

It's meant to be used with **Mica** or **MicaAlt** backdrops, with or without the **Translucent Windows** mod.

---

![MediaControlCenter](mediacontrolcenter.png)

---

## General Information

The theme changes the following elements:

- Rounded tabs
- Transparent Command bars
- Transparent Address Bar and Search Box (Unless if in focus)
- Centralized Lower Command bar
- Transparent separator below lower Command bar
- Removed dropshadows
- Matching border brush on some UWP context menus
- Matching border brush and radius on some UWM tool tips

---

## Known Issues

I didn't know how to fix these. I couldn't find the correct target names, or I'm not sure if they can even be changed.

- Tooltips have no Acrylic
- Context menus doesn't have matching border radius
- Some Context menus doesn't have matching border brushes
- Context menus doesn't have matching backdrop
- Context menus inside context menus doesn't match anything

---

## Full Luminosity Theme

For that, download the listed mods and select "**Luminosity**" on each.
- Windows 11 Taskbar Styler
- Windows 11 Start Menu Styler
- Windows 11 Notification Center Styler
- Windows 11 File Explorer Styler

I also highly recommend **Translucent Windows** with **Mica** or **MicaAlt** selected as backdrop.

---

## Theme selection

The theme is integrated into the mod and can simply be selected from the mod's
settings:

* Open the Windows 11 Taskbar Styler mod in Windhawk.
* Go to the "Settings" tab.
* Select the theme and save the settings.

## Manual installation

The theme styles can also be imported manually. To do that, follow these steps:

* Open the Windows 11 Taskbar Styler mod in Windhawk.
* Go to the "Advanced" tab.
* Copy the content below to the text box under "Mod settings" and click "Save".

<details>
<summary>Content to import (click to expand)</summary>

```json
 {
  "controlStyles[0].target": "TabViewItem > Grid#LayoutRoot",
  "controlStyles[0].styles[0]": "CornerRadius=10",
  "controlStyles[1].target": "Button#AddButton",
  "controlStyles[1].styles[0]": "RenderTransform:=<TranslateTransform X=\"0\" Y=\"-1\" />",
  "controlStyles[2].target": "Microsoft.UI.Xaml.Controls.Border#BottomBorderLine",
  "controlStyles[2].styles[0]": "Visibility=Collapsed",
  "controlStyles[3].target": "Grid#TabContainerGrid > Border#LeftBottomBorderLine",
  "controlStyles[3].styles[0]": "Visibility=Collapsed",
  "controlStyles[4].target": "Grid#TabContainerGrid > Border#RightBottomBorderLine",
  "controlStyles[4].styles[0]": "Visibility=Collapsed",
  "controlStyles[5].target": "Microsoft.UI.Xaml.Controls.Grid#NavigationBarControlGrid",
  "controlStyles[5].styles[0]": "Background:=$t",
  "controlStyles[6].target": "Microsoft.UI.Xaml.Controls.Grid#PART_LayoutRoot",
  "controlStyles[7].target": "Microsoft.UI.Xaml.Controls.AutoSuggestBox#FileExplorerSearchBox > Microsoft.UI.Xaml.Controls.Grid#LayoutRoot > Microsoft.UI.Xaml.Controls.TextBox#TextBox",
  "controlStyles[8].target": "Microsoft.UI.Xaml.Controls.Grid#CommandBarControlRootGrid",
  "controlStyles[8].styles[0]": "Background:=$t",
  "controlStyles[8].styles[1]": "BorderBrush:=$t",
  "controlStyles[9].target": "Microsoft.UI.Xaml.Controls.CommandBar#FileExplorerCommandBar",
  "controlStyles[9].styles[0]": "Background:=$t",
  "controlStyles[9].styles[1]": "RenderTransform:=<TranslateTransform X=\"0\" Y=\"-10\" />",
  "controlStyles[9].styles[2]": "HorizontalAlignment=Center",
  "controlStyles[10].target": "Microsoft.UI.Xaml.Controls.CommandBar#FileExplorerSecondaryCommandBar > Microsoft.UI.Xaml.Controls.Grid#LayoutRoot > Microsoft.UI.Xaml.Controls.Grid#ContentRoot",
  "controlStyles[10].styles[0]": "Visibility=Collapsed",
  "controlStyles[11].target": "Microsoft.UI.Xaml.Controls.Grid#HomeViewRootGrid",
  "controlStyles[11].styles[0]": "Background:=$t",
  "controlStyles[12].target": "FileExplorerExtensions.GalleryViewControl - GalleryViewControl",
  "controlStyles[12].styles[0]": "Visibility=Collapsed",
  "controlStyles[13].target": "FileExplorerExtensions.GalleryViewControl#GalleryViewControl > Grid",
  "controlStyles[13].styles[0]": "Background:=$t",
  "styleConstants[0]": "mbg=<AcrylicBrush TintColor=\"{ThemeResource CardStrokeColorDefaultSolid}\" FallbackColor=\"{ThemeResource CardStrokeColorDefaultSolid}\" TintOpacity=\"0.0\" TintLuminosityOpacity=\"1.0\" Opacity=\"1\"/>",
  "styleConstants[1]": "bcr=10",
  "styleConstants[2]": "bbb=#13FFFFFF",
  "styleConstants[3]": "wcr=20",
  "styleConstants[4]": "mcr=15",
  "styleConstants[5]": "t=Transparent",
  "styleConstants[6]": "bb=#20FFFFFF",
  "styleConstants[7]": "bt=1",
  "styleConstants[8]": "mbt=#10FFFFFF",
  "styleConstants[9]": "mbth=#15FFFFFF",
  "styleConstants[10]": "mbtp=#15FFFFFF",
  "controlStyles[14].target": "TabViewItem > Grid#LayoutRoot",
  "controlStyles[14].styles[0]": "CornerRadius=$mcr",
  "controlStyles[14].styles[1]": "BorderThickness=0",
  "controlStyles[14].styles[2]": "BorderBrush=$t",
  "controlStyles[15].target": "Button#CloseButton",
  "controlStyles[15].styles[0]": "CornerRadius=$bcr",
  "controlStyles[16].target": "Button#AddButton",
  "controlStyles[16].styles[0]": "CornerRadius=$bcr",
  "controlStyles[17].target": "TabViewItem > Grid#LayoutRoot@CommonStates",
  "controlStyles[17].styles[0]": "Background@Normal:=$t",
  "controlStyles[17].styles[1]": "Background@PointerOver:=#02FFFFFF",
  "controlStyles[17].styles[2]": "Background@Selected:=#05FFFFFF",
  "controlStyles[17].styles[3]": "Background@PointerOverSelected:=$mbth",
  "controlStyles[17].styles[4]": "Background@PressedSelected:=$mbth",
  "controlStyles[18].target": "Microsoft.UI.Xaml.Controls.Grid#PART_LayoutRoot",
  "controlStyles[18].styles[0]": "CornerRadius=14",
  "controlStyles[18].styles[1]": "BorderBrush:=$bbb",
  "controlStyles[19].target": "Microsoft.UI.Xaml.Controls.Primitives.ToggleButton#PART_RootChevronButton",
  "controlStyles[19].styles[0]": "CornerRadius=$bcr",
  "controlStyles[20].target": "Microsoft.UI.Xaml.Controls.TextBox - TextBox > Microsoft.UI.Xaml.Controls.Grid > Microsoft.UI.Xaml.Controls.Border#BorderElement > Microsoft.UI.Xaml.Controls.ScrollViewer#ContentElement > Microsoft.UI.Xaml.Controls.Border#Root > Microsoft.UI.Xaml.Controls.Grid > Microsoft.UI.Xaml.Controls.ScrollContentPresenter#ScrollContentPresenter > Microsoft.UI.Xaml.Internal.TextBoxView",
  "controlStyles[20].styles[0]": "RenderTransform:=<TranslateTransform X=\"0\" Y=\"1\" />",
  "controlStyles[21].target": "Microsoft.UI.Xaml.Controls.Primitives.ToggleButton#PART_RootChevronButton",
  "controlStyles[21].styles[0]": "CornerRadius=8",
  "controlStyles[22].target": "Microsoft.UI.Xaml.Controls.AutoSuggestBox#FileExplorerSearchBox > Microsoft.UI.Xaml.Controls.Grid#LayoutRoot > Microsoft.UI.Xaml.Controls.TextBox#TextBox",
  "controlStyles[22].styles[0]": "Background:=$mbt",
  "controlStyles[22].styles[1]": "CornerRadius=$mcr",
  "controlStyles[22].styles[2]": "BorderBrush:=$bbb",
  "controlStyles[22].styles[3]": "Margin=0,-0.3,0,-0.75",
  "controlStyles[23].target": "Microsoft.UI.Xaml.Controls.Button#MoreButton > Microsoft.UI.Xaml.Controls.Grid@CommonStates",
  "controlStyles[23].styles[0]": "CornerRadius@PointerOver:=$bcr",
  "controlStyles[23].styles[1]": "CornerRadius@Pressed:=$bcr",
  "controlStyles[24].target": "MenuFlyoutPresenter > Border",
  "controlStyles[24].styles[0]": "BorderThickness:=$bt",
  "controlStyles[24].styles[1]": "BorderBrush:=$bb",
  "controlStyles[24].styles[2]": "CornerRadius:=$mcr",
  "controlStyles[25].target": "MenuFlyoutPresenter",
  "controlStyles[25].styles[0]": "BorderThickness:=$bt",
  "controlStyles[25].styles[1]": "BorderBrush:=$bb",
  "controlStyles[25].styles[2]": "CornerRadius:=$mcr",
  "controlStyles[26].target": "Microsoft.UI.Xaml.Controls.Primitives.CommandBarFlyoutCommandBar",
  "controlStyles[26].styles[0]": "BorderThickness:=$bt",
  "controlStyles[26].styles[1]": "BorderBrush:=$bb",
  "controlStyles[26].styles[2]": "CornerRadius:=$mcr",
  "controlStyles[27].target": "Microsoft.UI.Xaml.Controls.RadioMenuFlyoutItem",
  "controlStyles[27].styles[0]": "CornerRadius=$bcr",
  "controlStyles[28].target": "Microsoft.UI.Xaml.Controls.Border#AppBarButtonInnerBorder",
  "controlStyles[28].styles[0]": "CornerRadius=$bcr",
  "controlStyles[29].target": "Microsoft.UI.Xaml.Controls.MenuFlyoutItem",
  "controlStyles[29].styles[0]": "CornerRadius=$bcr",
  "controlStyles[30].target": "Microsoft.UI.Xaml.Controls.MenuFlyoutSubItem",
  "controlStyles[30].styles[0]": "CornerRadius=$bcr",
  "controlStyles[31].target": "ToolTip",
  "controlStyles[31].styles[0]": "Background:=$mbg",
  "controlStyles[31].styles[1]": "CornerRadius:=$mcr",
  "controlStyles[31].styles[2]": "BorderThickness:=$bt",
  "controlStyles[31].styles[3]": "BorderBrush:=$bb",
  "controlStyles[32].target": "Microsoft.UI.Xaml.Controls.Primitives.CommandBarFlyoutCommandBar > Grid#LayoutRoot > Grid#OuterContentRoot > Grid#ContentRoot > Grid#PrimaryItemsRoot",
  "controlStyles[33].target": "ScrollViewer#MenuFlyoutPresenterScrollViewer > Border > Grid > ScrollContentPresenter > ItemsPresenter > StackPanel",
  "controlStyles[33].styles[0]": "ChildrenTransitions:=<TransitionCollection><EntranceThemeTransition IsStaggeringEnabled=\"True\" FromHorizontalOffset=\"0\" FromVerticalOffset=\"100\" /></TransitionCollection>",
  "controlStyles[34].target": "Grid#LayoutRoot",
  "controlStyles[34].styles[0]": "BackgroundTransition:=<BrushTransition Duration=\"0:0:0.100\" />",
  "controlStyles[35].target": "Border#BackgroundBorder",
  "controlStyles[35].styles[0]": "BackgroundTransition:=<BrushTransition Duration=\"0:0:0.100\" />"
}
```
</details>