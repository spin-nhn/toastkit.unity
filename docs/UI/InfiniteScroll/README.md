# Infinite Scroll

🌏 [English](README.en.md)

## 개요

Scroll Rect를 사용할 경우 Content 사이즈에 맞게 Item을 생성해서 재사용하도록 도와주는 Component입니다.

* InfiniteScroll은 사용자가 Insert 한 InfiniteScrollData(혹은 상속받은) 클래스를 가지고 Content의 Element를 생성합니다.
    * InfiniteScroll.InsertData()
* Content의 Element로 사용할 Prefab에서는 InfiniteScrollItem(혹은 상속받은) 클래스를 Attach 해서 사용하셔야 합니다.
    * InfiniteScrollItem.UpdateData()에서 Prefab 로직 구현

## 🔨 API

API 사용 방법은 Assets/TOAST/Kit/UI/InfiniteScroll/Sample/Scripts/InfiniteScrollSample.cs 를 참고하시기 바랍니다.

### InsertData

Content의 Element로 보여줄 Data를 추가합니다.

```cs
public void InsertData(InfiniteScrollData data)
```

### UpdateData

Insert한 Data를 업데이트합니다.

```cs
public void UpdateData(InfiniteScrollData data)
```

### UpdateAllData

모든 Data를 업데이트합니다.

```cs
public void UpdateAllData()
```

### RemoveData

Insert한 Data를 삭제합니다.

```cs
public void RemoveData(InfiniteScrollData data)
```

### Clear

모든 Data를 삭제합니다.

```cs
public void Clear()
```

### MoveToFirstData

첫 번째 Data로 Content를 이동합니다.

```cs
public void MoveToFirstData()
```

### MoveToLastData

마지막 Data로 Content를 이동합니다.

```cs
public void MoveToLastData()
```

### IsMoveToLastData

Content가 마지막 Data로 이동했는지 확인합니다.

```cs
public bool IsMoveToLastData()
```

### ResizeScrollView

ScrollView 사이즈가 변경되었을 때 Infinite Scroll에서 사이즈 변경에 대한 처리를 하기 위해 필요한 API입니다.

```cs
public void ResizeScrollView()
```

## 🐾 Example

Assets/TOAST/Kit/UI/InfiniteScroll/Sample

![infinitescroll_sample](images/infinitescroll_sample.gif)

