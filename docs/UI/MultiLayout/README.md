# Multi Layout

🌏 [English](README.en.md)

## 개요

MultiLayout Component는 UI Component의 RectTransform 정보를 여러 개의 layout으로 설정하여 Resolution, Orientation 등에 대응할 수 있도록 도와줍니다.

## 🔨 API

### SelectLayout

설정되어 있는 layout 중 하나를 선택합니다.

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