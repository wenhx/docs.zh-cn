---
title: StrongNameSignatureVerificationFromImage 函数
ms.date: 03/30/2017
api_name:
- StrongNameSignatureVerificationFromImage
api_location:
- mscoree.dll
api_type:
- DLLExport
f1_keywords:
- StrongNameSignatureVerificationFromImage
helpviewer_keywords:
- StrongnameSignatureVerificationFromImage function [.NET Framework strong naming]
ms.assetid: 9fb144d2-07e0-4a0e-8e05-907bbb6c9e03
topic_type:
- apiref
ms.openlocfilehash: 5c12ca20deee06fcaca68365644fd9dff95379ff
ms.sourcegitcommit: 559fcfbe4871636494870a8b716bf7325df34ac5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/30/2019
ms.locfileid: "73121158"
---
# <a name="strongnamesignatureverificationfromimage-function"></a>StrongNameSignatureVerificationFromImage 函数
验证已映射到内存的程序集对关联的公钥是否有效。  
  
 此函数已弃用。 改为使用[ICLRStrongName：： StrongNameVerificationFromImage](../hosting/iclrstrongname-strongnamesignatureverificationfromimage-method.md)方法。  
  
## <a name="syntax"></a>语法  
  
```cpp  
BOOLEAN StrongNameSignatureVerificationFromImage (  
    [in]  BYTE    *pbBase,  
    [in]  DWORD   dwLength,  
    [in]  DWORD   dwInFlags,  
    [out] DWORD   *pdwOutFlags  
);  
```  
  
## <a name="parameters"></a>参数  
 `pbBase`  
 中映射的程序集清单的相对虚拟地址。  
  
 `dwLength`  
 中映射的图像的大小（以字节为单位）。  
  
 `dwInFlags`  
 中影响验证行为的标志。 支持以下值：  
  
- `SN_INFLAG_FORCE_VER` （0x00000001）-即使需要重写注册表设置，也强制进行验证。  
  
- `SN_INFLAG_INSTALL` （0x00000002）-指定这是在此映像上执行的第一次验证。  
  
- `SN_INFLAG_ADMIN_ACCESS` （0x00000004）-指定缓存只允许具有管理权限的用户访问。  
  
- `SN_INFLAG_USER_ACCESS` （0x00000008）-指定只有当前用户才能访问该程序集。  
  
- `SN_INFLAG_ALL_ACCESS` （0x00000010）-指定缓存将不提供访问限制。  
  
- `SN_INFLAG_RUNTIME` （0x80000000）-保留用于内部调试。  
  
 `pdwOutFlags`  
 弄用于附加输出信息的标志。 支持以下值：  
  
- `SN_OUTFLAG_WAS_VERIFIED` （0x00000001）-此值设置为 `false` 以指定验证是否已成功（因为注册表设置）。  
  
## <a name="return-value"></a>返回值  
 成功完成后 `true`;否则，`false`。  
  
## <a name="remarks"></a>备注  
 如果 `StrongNameSignatureVerificationFromImage` 函数未成功完成，请调用[StrongNameErrorInfo](strongnameerrorinfo-function.md)函数以检索上次生成的错误。  
  
## <a name="requirements"></a>要求  
 **平台：** 请参阅[系统要求](../../get-started/system-requirements.md)。  
  
 **标头：** Stackexchange.redis.strongname  
  
 **库：** 作为资源包括在 mscoree.dll 中  
  
 **.NET Framework 版本：** [!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]  
  
## <a name="see-also"></a>请参阅

- [StrongNameSignatureVerificationFromImage 方法](../hosting/iclrstrongname-strongnamesignatureverificationfromimage-method.md)
- [ICLRStrongName 接口](../hosting/iclrstrongname-interface.md)
