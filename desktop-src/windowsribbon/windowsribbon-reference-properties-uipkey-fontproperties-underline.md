---
title: UI\_PKEY\_FontProperties\_Underline
description: Identifies the UI\_PKEY\_FontProperties\_Underline property.
ms.assetid: '88492558-ab19-4606-8fe0-5f100677b88a'
---

# UI\_PKEY\_FontProperties\_Underline

Identifies the UI\_PKEY\_FontProperties\_Underline property.

```
propertyDescription
   name = UI_PKEY_FontProperties_Underline
   shellPKey = UI_PKEY_FontProperties_Underline
   formatID = 00000305-7363-696e-8441798acf5aebb7
   propID = 305
   typeInfo
      type = UI_FONTUNDERLINE
```

## Remarks

UI\_PKEY\_FontProperties\_Underline is used by an application to query the state of the **Underline** button.

The property value is from the [**UI\_FONTUNDERLINE**](https://msdn.microsoft.com/library/windows/desktop/dd371568) enumeration.

The default value is `UI_FONTUNDERLINE_NOTSET`.

The following screen shot shows the **Underline** button of the Ribbon [**FontControl**](windowsribbon-element-fontcontrol.md).

![screen shot of the fontcontrol element with the richfont attribute set to true.](images/markup/fontcontrol-underline.png)

The following table describes the properties and the UI result.



|                                 |                                                                          |
|---------------------------------|--------------------------------------------------------------------------|
| `UI_FONTUNDERLINE_NOTAVAILABLE` | **Underline** button is disabled and can only be set by the application. |
| `UI_FONTUNDERLINE_NOTSET`       | **Underline** button is not selected.                                    |
| `UI_FONTUNDERLINE_SET`          | **Underline** button is selected.                                        |



 

## Related topics

<dl> <dt>

[Font Control Properties](windowsribbon-reference-properties-fontcontrol.md)
</dt> <dt>

[**UI\_FONTUNDERLINE**](https://msdn.microsoft.com/library/windows/desktop/dd371568)
</dt> <dt>

[Font Control](windowsribbon-controls-fontcontrol.md)
</dt> </dl>

 

 



