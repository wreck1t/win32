---
title: VistaApi.JetOSSnapshotGetFreezeInfo method  (Microsoft.Isam.Esent.Interop.Vista)
TOCTitle: 'JetOSSnapshotGetFreezeInfo method '
ms:assetid: M:Microsoft.Isam.Esent.Interop.Vista.VistaApi.JetOSSnapshotGetFreezeInfo(Microsoft.Isam.Esent.Interop.JET_OSSNAPID,System.Int32@,Microsoft.Isam.Esent.Interop.JET_INSTANCE_INFO[]@,Microsoft.Isam.Esent.Interop.Vista.SnapshotGetFreezeInfoGrbit)
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/microsoft.isam.esent.interop.vista.vistaapi.jetossnapshotgetfreezeinfo(v=EXCHG.10)
ms:contentKeyID: 55104199
ms.date: 07/30/2014
ms.topic: reference
f1_keywords:
- Microsoft.Isam.Esent.Interop.Vista.VistaApi.JetOSSnapshotGetFreezeInfo
dev_langs:
- CSharp
- JScript
- VB
- other
api_name: 
- Microsoft.Isam.Esent.Interop.Vista.VistaApi.JetOSSnapshotGetFreezeInfo
topic_type: 
- apiref
- kbSyntax
api_type: 
- Managed
api_location: 
- Microsoft.Isam.Esent.Interop.dll
ROBOTS: INDEX,FOLLOW

---

# VistaApi.JetOSSnapshotGetFreezeInfo method

Retrieves the list of instances and databases that are part of the snapshot session at any given moment.

**Namespace:**  [Microsoft.Isam.Esent.Interop.Vista](hh558039\(v=exchg.10\).md)  
**Assembly:**  Microsoft.Isam.Esent.Interop (in Microsoft.Isam.Esent.Interop.dll)

## Syntax

``` vb
'Declaration
Public Shared Sub JetOSSnapshotGetFreezeInfo ( _
    snapshot As JET_OSSNAPID, _
    <OutAttribute> ByRef numInstances As Integer, _
    <OutAttribute> ByRef instances As JET_INSTANCE_INFO(), _
    grbit As SnapshotGetFreezeInfoGrbit _
)
'Usage
Dim snapshot As JET_OSSNAPID
Dim numInstances As Integer
Dim instances As JET_INSTANCE_INFO()
Dim grbit As SnapshotGetFreezeInfoGrbitVistaApi.JetOSSnapshotGetFreezeInfo(snapshot, _
    numInstances, instances, grbit)
```

``` csharp
public static void JetOSSnapshotGetFreezeInfo(
    JET_OSSNAPID snapshot,
    out int numInstances,
    out JET_INSTANCE_INFO[] instances,
    SnapshotGetFreezeInfoGrbit grbit
)
```

#### Parameters

  - snapshot  
    Type: [Microsoft.Isam.Esent.Interop.JET_OSSNAPID](hh558483\(v=exchg.10\).md)  
    
    The identifier of the snapshot session.

<!-- end list -->

  - numInstances  
    Type: [System.Int32](https://docs.microsoft.com/dotnet/api/system.int32?redirectedfrom=MSDN)  
    
    Returns the number of instances.

<!-- end list -->

  - instances  
    Type: \[\]  
    
    Returns information about the instances.

<!-- end list -->

  - grbit  
    Type: [Microsoft.Isam.Esent.Interop.Vista.SnapshotGetFreezeInfoGrbit](hh565195\(v=exchg.10\).md)  
    
    Options for this call.

## See also

#### Reference

[VistaApi class](dn335321\(v=exchg.10\).md)

[VistaApi members](dn335317\(v=exchg.10\).md)

[Microsoft.Isam.Esent.Interop.Vista namespace](hh558039\(v=exchg.10\).md)

