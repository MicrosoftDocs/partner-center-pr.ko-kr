---
title: 고객 계정에 대해 여러 사용자를 가져오는 .csv 파일의 필드
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 고객 계정에 여러 사용자를 추가하려면 적절한 필드가 있는 쉼표로 구분된 값(.csv) 파일을 만듭니다.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 152daadde25a9325937797f7a3daa90dfb59a9b4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150984"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>.csv 파일을 만들어 고객 계정에 여러 사용자 추가

**적절한 역할**: 전역 관리자

쉼표로 구분된 값 파일 형식(.csv)으로 데이터 파일을 파트너 센터 업로드하여 한 번에 고객 계정에 여러 사용자를 추가합니다. 파트너 센터 샘플 데이터 파일을 다운로드한 다음, 사용하기 위해 편집하거나 아래에 정의된 데이터 모델을 사용하여 새 데이터 파일을 만들 수 있습니다.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>데이터 파일 요구 사항

대량 업로드 프로세스를 사용하여 고객 계정에 여러 사용자를 추가하려면 다음 요구 사항을 충족해야 합니다.

- 고객 계정에 대한 전역 관리자 권한이 있어야 합니다.
- 각 사용자에게는 고객의 이메일 도메인에 추가된 고유한 이메일 주소가 있어야 합니다.
- 한 번에 최대 100개 레코드를 업로드할 수 있습니다. 100명 이상의 사용자를 추가해야 하는 경우 추가 데이터 파일을 만들고 업로드합니다.
- 모든 사용자는 동일한 지리적 **위치** 에 있어야 합니다.
- 아래에 설명된 데이터만 입력합니다. 데이터가 있으면 업로드가 실패합니다.

데이터 파일에 다음 데이터를 입력합니다.

| **열 이름** | **설명**  | **제한 사항**  |
|:-------- |:------  |:----- |
| 이름  | 사용자의 이름(선택적 필드)  | 50자로 제한  |
| 성  | 사용자의 성(선택적 필드)  | 50자로 제한  |
| 표시 이름    | 파트너 센터 표시되는 이름(필수 필드)                            | 50자로 제한                         |
| 메일   | 고객 회사의 사용자 비즈니스 이메일 주소(필수 필드)           | 각 사용자에게는 고유한 전자 메일 주소가 있어야 합니다. |
| 상태 업데이트   | 새 사용자 레코드가 성공적으로 만들어졌는지 여부를 나타내는 데 사용됩니다. | \*\*비워 둠\*\*                        |

## <a name="next-steps"></a>다음 단계

- [고객에 대해 다수 사용자를 추가하는 방법](adding-multiple-users-to-a-customer-account.md)