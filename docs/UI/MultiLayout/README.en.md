# Multi Layout

🌏 [한국어](README.md)

## Overview

The multi-layout component configures RectTransform data of UI component into many layouts so as to deal with resolution or orientation.

## 🔨 API

### SelectLayout

Select one of the configured layouts.

#### API

```cs
public void SelectLayout(int layoutIndex)
```

#### Example

```cs
public void SetOrientation(ScreenOrientation orientataion)
{
    if (orientataion == ScreenOrientation.Portrait)
    {
        multiLayout.SelectLayout(1);
    }
    else
    {
        multiLayout.SelectLayout(0);
    }
}
```

## 🐾 Example

Assets/TOAST/Kit/UI/MultiLayout/Sample

### Editor

![multilayout_editor](images/multilayout_editor.gif)

### Runtime

![multilayout_runtime](images/multilayout_runtime.gif)