---
title: Server2003Api.JetUpdate2 method  (Microsoft.Isam.Esent.Interop.Server2003)
TOCTitle: 'JetUpdate2 method '
ms:assetid: M:Microsoft.Isam.Esent.Interop.Server2003.Server2003Api.JetUpdate2(Microsoft.Isam.Esent.Interop.JET_SESID,Microsoft.Isam.Esent.Interop.JET_TABLEID,System.Byte[],System.Int32,System.Int32@,Microsoft.Isam.Esent.Interop.Server2003.UpdateGrbit)
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/microsoft.isam.esent.interop.server2003.server2003api.jetupdate2(v=EXCHG.10)
ms:contentKeyID: 55104110
ms.date: 07/30/2014
ms.topic: reference
f1_keywords:
- Microsoft.Isam.Esent.Interop.Server2003.Server2003Api.JetUpdate2
dev_langs:
- CSharp
- JScript
- VB
- other
api_name: 
- Microsoft.Isam.Esent.Interop.Server2003.Server2003Api.JetUpdate2
topic_type: 
- kbSyntax
- apiref
api_type: 
- Managed
api_location: 
- Microsoft.Isam.Esent.Interop.dll
ROBOTS: INDEX,FOLLOW

---

# Server2003Api.JetUpdate2 method

The JetUpdate function performs an update operation including inserting a new row into a table or updating an existing row. Deleting a table row is performed by calling [JetDelete(JET_SESID, JET_TABLEID)](dn292131\(v=exchg.10\).md).

**Namespace:**  [Microsoft.Isam.Esent.Interop.Server2003](hh557147\(v=exchg.10\).md)  
**Assembly:**  Microsoft.Isam.Esent.Interop (in Microsoft.Isam.Esent.Interop.dll)

## Syntax

``` vb
'Declaration
Public Shared Sub JetUpdate2 ( _
    sesid As JET_SESID, _
    tableid As JET_TABLEID, _
    bookmark As Byte(), _
    bookmarkSize As Integer, _
    <OutAttribute> ByRef actualBookmarkSize As Integer, _
    grbit As UpdateGrbit _
)
'Usage
Dim sesid As JET_SESID
Dim tableid As JET_TABLEID
Dim bookmark As Byte()
Dim bookmarkSize As Integer
Dim actualBookmarkSize As Integer
Dim grbit As UpdateGrbitServer2003Api.JetUpdate2(sesid, tableid, bookmark, _
    bookmarkSize, actualBookmarkSize, _
    grbit)
```

``` csharp
public static void JetUpdate2(
    JET_SESID sesid,
    JET_TABLEID tableid,
    byte[] bookmark,
    int bookmarkSize,
    out int actualBookmarkSize,
    UpdateGrbit grbit
)
```

#### Parameters

  - sesid  
    Type: [Microsoft.Isam.Esent.Interop.JET_SESID](hh596745\(v=exchg.10\).md)  
    
    The session which started the update.

<!-- end list -->

  - tableid  
    Type: [Microsoft.Isam.Esent.Interop.JET_TABLEID](hh566310\(v=exchg.10\).md)  
    
    The cursor to update. An update should be prepared.

<!-- end list -->

  - bookmark  
    Type: \[\]  
    
    Returns the bookmark of the updated record. This can be null.

<!-- end list -->

  - bookmarkSize  
    Type: [System.Int32](https://docs.microsoft.com/dotnet/api/system.int32?redirectedfrom=MSDN)  
    
    The size of the bookmark buffer.

<!-- end list -->

  - actualBookmarkSize  
    Type: [System.Int32](https://docs.microsoft.com/dotnet/api/system.int32?redirectedfrom=MSDN)  
    
    Returns the actual size of the bookmark.

<!-- end list -->

  - grbit  
    Type: [Microsoft.Isam.Esent.Interop.Server2003.UpdateGrbit](hh558389\(v=exchg.10\).md)  
    
    Update options.

## Remarks

JetUpdate is the final step in performing an insert or an update. The update is begun by calling [JetPrepareUpdate(JET_SESID, JET_TABLEID, JET_prep)](dn332988\(v=exchg.10\).md) and then by calling [JetSetColumn(JET_SESID, JET_TABLEID, JET_COLUMNID, \[\], Int32, SetColumnGrbit, JET_SETINFO)](dn334009\(v=exchg.10\).md) one or more times to set the record state. Finally, JetUpdate2(JET_SESID, JET_TABLEID, \[\], Int32, Int32, UpdateGrbit) is called to complete the update operation. Indexes are updated only by JetUpdate or and not during JetSetColumn.

## See also

#### Reference

[Server2003Api class](dn351277\(v=exchg.10\).md)

[Server2003Api members](dn351196\(v=exchg.10\).md)

[Microsoft.Isam.Esent.Interop.Server2003 namespace](hh557147\(v=exchg.10\).md)

