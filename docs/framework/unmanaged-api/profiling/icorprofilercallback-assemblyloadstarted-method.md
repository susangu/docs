---
title: "ICorProfilerCallback::AssemblyLoadStarted Method | Microsoft Docs"
ms.custom: ""
ms.date: "03/30/2017"
ms.prod: ".net-framework-4.6"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "dotnet-clr"
ms.tgt_pltfrm: ""
ms.topic: "reference"
apiname: 
  - "ICorProfilerCallback.AssemblyLoadStarted"
apilocation: 
  - "mscorwks.dll"
apitype: "COM"
f1_keywords: 
  - "ICorProfilerCallback::AssemblyLoadStarted"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "ICorProfilerCallback::AssemblyLoadStarted method [.NET Framework profiling]"
  - "AssemblyLoadStarted method [.NET Framework profiling]"
ms.assetid: 67e8209d-a0ca-4118-a6e6-c1ee0abc2221
caps.latest.revision: 13
author: "mairaw"
ms.author: "mairaw"
manager: "wpickett"
---
# ICorProfilerCallback::AssemblyLoadStarted Method
Notifies the profiler that an assembly is being loaded.  
  
## Syntax  
  
```  
HRESULT AssemblyLoadStarted(  
    [in] AssemblyID assemblyId);  
```  
  
#### Parameters  
 `assemblyId`  
 [in] Identifies the assembly that is being loaded.  
  
## Remarks  
 The value of `assemblyId` is not valid for an information request until the [ICorProfilerCallback::AssemblyLoadFinished](../../../../docs/framework/unmanaged-api/profiling/icorprofilercallback-assemblyloadfinished-method.md) method is called.  
  
## Requirements  
 **Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).  
  
 **Header:** CorProf.idl, CorProf.h  
  
 **Library:** CorGuids.lib  
  
 **.NET Framework Versions:** [!INCLUDE[net_current_v20plus](../../../../includes/net-current-v20plus-md.md)]  
  
## See Also  
 [ICorProfilerCallback Interface](../../../../docs/framework/unmanaged-api/profiling/icorprofilercallback-interface.md)