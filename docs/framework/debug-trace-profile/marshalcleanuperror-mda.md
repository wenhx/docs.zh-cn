---
title: marshalCleanupError MDA
description: 查看 marshalCleanupError 托管调试助手（MDA），因为在清理临时结构时出现意外错误。
ms.date: 03/30/2017
helpviewer_keywords:
- cleanup operations
- marshaling, run-time errors
- managed debugging assistants (MDAs), marshaling
- MDAs (managed debugging assistants), marshaling
- marshaling cleanup error
- MarshalCleanupError MDA
- memory, cleanup errors
ms.assetid: 2f5d9e7c-ae51-4155-a435-54347aa1f091
ms.openlocfilehash: 3c7498d6f51484de3a2e84d611a2634f53724ab6
ms.sourcegitcommit: 0edbeb66d71b8df10fcb374cfca4d731b58ccdb2
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2020
ms.locfileid: "86051605"
---
# <a name="marshalcleanuperror-mda"></a>marshalCleanupError MDA
如果公共语言运行时 (CLR) 在尝试清理那些用于封送本机代码和托管代码边界之间的数据类型的临时结构和内存时遇到错误，则将激活 `marshalCleanupError` 托管调试助手 (MDA)。  
  
## <a name="symptoms"></a>症状  
 进行本机代码和托管代码转换时发生内存泄漏，线程区域性等运行时状态无法还原，或 <xref:System.Runtime.InteropServices.SafeHandle> 清理中发生错误。  
  
## <a name="cause"></a>原因  
 清理临时结构时发生意外错误。  
  
## <a name="resolution"></a>解决方法  
 检查所有 <xref:System.Runtime.InteropServices.SafeHandle> 析构函数、终结器和自定义封送拆收器实现中是否存在错误。  
  
## <a name="effect-on-the-runtime"></a>对运行时的影响  
 此 MDA 对 CLR 无任何影响。  
  
## <a name="output"></a>输出  
 报告在清理期间失败的操作的消息。  
  
## <a name="configuration"></a>配置  
  
```xml  
<mdaConfig>  
  <assistants>  
    <marshalCleanupError />  
  </assistants>  
</mdaConfig>  
```  
  
## <a name="see-also"></a>请参阅

- <xref:System.Runtime.InteropServices.MarshalAsAttribute>
- [使用托管调试助手诊断错误](diagnosing-errors-with-managed-debugging-assistants.md)
- [互操作封送处理](../interop/interop-marshaling.md)
