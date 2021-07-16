---
title: 예제 응용 프로그램
ms.topic: article
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 샘플 애플리케이션을 사용하여 프로그래밍 방식으로 파트너 인사이트 데이터에 액세스하는 고유한 애플리케이션을 빌드합니다.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: 6f334b9047c38e8b7763a4ba96d21d987c252682
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375856"
---
# <a name="sample-application"></a>예제 응용 프로그램

샘플 애플리케이션은 C# 및 JAVA 언어로 만들어지고 [GitHub](https://github.com/partneranalytics)

- [C# 샘플 애플리케이션](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [JAVA 샘플 애플리케이션](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

샘플 애플리케이션에서 아이디어를 얻어 원하는 언어로 자체 애플리케이션을 빌드할 수 있습니다.

샘플 애플리케이션은 다음 목표를 달성합니다.

- Azure AD(Azure Active Directory) 토큰을 생성합니다.
- 사용 가능한 데이터 세트를 가져옵니다.
- 사용자 정의 쿼리를 만듭니다.
- 사용자 정의 및 시스템 쿼리를 가져옵니다.
- 보고서를 예약합니다.

샘플 애플리케이션은 다른 기능에 대해 API를 호출하는 방법을 다루지 않습니다. 그러나 다른 API를 호출하는 프로세스는 위에 설명된 것과 동일하게 유지됩니다.

## <a name="how-to-run-the-application"></a>애플리케이션을 실행하는 방법

- 다음 명령을 사용하여 로컬 시스템에 리포지토리를 복제합니다.

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> 자세한 내용은 GitHub [리포지토리의](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)ProgrammaticExportSampleAppMPN/README.md 파일을 참조합니다.

- 앱을 신속하게 실행하려면appsettings.Development.js클라이언트 ID 및 클라이언트 비밀을 **업데이트합니다.**

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="앱설정 개발 json 설명":::

앱을 실행하면 로컬 웹 서버가 시작되고 페이지가 열립니다(`https://localhost:44365/ProgrammaticExportSampleApp/sample`).
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="샘플 애플리케이션의 UI 설명":::

이 페이지는 로컬 머신에서 실행되는 웹 서버에 대한 API 호출을 수행합니다. 이에 따라 실제 프로그래밍 방식 액세스 API 호출을 수행합니다.

## <a name="code-snippets"></a>코드 조각

프로그래밍 방식 액세스 API 호출을 수행하는 C# 코드의 기본 구조는 다음과 같습니다.
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="코드 조각 설명":::

## <a name="next-steps"></a>다음 단계

[파트너 인사이트 분석 데이터에 액세스하기 위한 API](insights-programmatic-analytics-available-api.md)
