---
title: 고객 계정에 대 한 여러 사용자를 가져오기 위한 .csv 파일 필드
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 고객 계정에 여러 사용자를 추가 하려면 적절 한 필드를 사용 하 여 쉼표로 구분 된 값 (.csv) 파일을 만듭니다.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 07a28e5310716f3df11caa36e51339e877e65627
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/03/2020
ms.locfileid: "87528187"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>.Csv 파일을 만들어 여러 사용자를 고객 계정에 추가

**적용 대상**

- 파트너 센터

**적절한 역할**

- 전역 관리자

쉼표로 구분 된 값 파일 형식 (.csv)의 데이터 파일을 파트너 센터에 업로드 하 여 한 번에 여러 사용자를 고객 계정에 추가 합니다. 파트너 센터에서 샘플 데이터 파일을 다운로드 한 다음 사용자가 사용할 수 있도록 편집 하거나 아래에 정의 된 데이터 모델을 사용 하 여 새 데이터 파일을 만들 수 있습니다.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>데이터 파일 요구 사항

대량 업로드 프로세스를 사용 하 여 고객의 계정에 여러 사용자를 추가 하려면 다음 요구 사항을 충족 해야 합니다.

- 고객 계정에 대 한 전역 관리자 권한이 있어야 합니다.
- 각 사용자에 게는 고객의 메일 도메인에 추가 된 고유한 전자 메일 주소가 있어야 합니다.
- 한 번에 최대 100 개의 레코드를 업로드할 수 있습니다. 100 명 이상의 사용자를 추가 해야 하는 경우 추가 데이터 파일을 만들고 업로드 합니다.
- 모든 사용자는 동일한 지리적 **위치**에 있어야 합니다.
- 아래에 설명 된 데이터만 입력 합니다. 불필요 한 데이터를 업로드 하면 업로드가 실패 합니다.

데이터 파일에 다음 데이터를 입력 합니다.

| **열 이름** | **설명**  | **제한 사항**  |
|:-------- |:------  |:----- |
| 이름  | 사용자의 이름 (선택 필드)  | 50자로 제한  |
| 성  | 사용자의 성 (선택 필드)  | 50자로 제한  |
| 표시 이름    | 파트너 센터 (필수 필드)에 표시 되는 이름                            | 50자로 제한                         |
| Email   | 고객 회사의 사용자 회사 전자 메일 주소 (필수 필드)           | 각 사용자에게는 고유한 전자 메일 주소가 있어야 합니다. |
| 상태 업데이트   | 새 사용자 레코드가 성공적으로 만들어졌는지 여부를 나타내는 데 사용 됩니다. | \*\*비워 둠\*\*                        |

## <a name="next-steps"></a>다음 단계

- [고객에 대해 여러 사용자를 추가 하는 방법](adding-multiple-users-to-a-customer-account.md)