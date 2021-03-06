---
title: 마켓플레이스 제품의 라이선스 관리
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: ISV 상업용 Marketplace 제안에 대한 라이선스를 설정하고 관리하는 방법을 알아봅니다.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c128b99b034564bcaa100ca975253f8b1bad7a42
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147958"
---
# <a name="manage-licensing-in-marketplace-offers"></a>마켓플레이스 제품의 라이선스 관리

**적절한 역할:** 전역 관리자 | 계정 관리자

이 문서에서는 파트너 센터 제안을 설정하고, Microsoft AppSource 사용할 수 있게 한 다음, 해당 제안에 대한 라이선스를 관리하는 프로세스를 안내합니다.  

>[!IMPORTANT]
>이 문서의 기능은 현재 공개 미리 보기로 제공됩니다.

## <a name="before-you-begin"></a>시작하기 전에

### <a name="commercial-marketplace-basics"></a>상업용 마켓플레이스 기본 사항

이 프로세스를 시작하기 전에 상업용 Marketplace의 기본 사항들을 숙지해야 합니다. 아래 표의 문서는 시작하는 데 도움이 됩니다. 

| 토픽  | 아티클  |
|-------|--------|
|상업용 마켓플레이스 플랜 | [상업용 마켓플레이스 제품에 대한 요금제 및 가격 책정](/azure/marketplace/plans-pricing)    |
|상업용 마켓플레이스 제안  | [목록 유형](/azure/marketplace/determine-your-listing-type)    |
|상업용 마켓플레이스 계정 |  [파트너 센터에서 상업용 마켓플레이스 계정 관리](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a>제안 ID 확인

아래 절차에서는 제안 ID를 입력하라는 메시지가 표시됩니다. 이제 다음 사항에 유의하여 적절한 제안 ID를 생각해보십시오.

- 이 ID는 마켓플레이스 제품 및 Azure Resource Manager 템플릿의 웹 주소에서 고객에게 표시됩니다(해당하는 경우).
- 게시자 ID와 결합된 제품 ID의 길이는 40자 미만이어야 합니다.
- 소문자와 숫자만 사용할 수 있습니다. 제안 ID에는 하이픈과 밑줄이 포함될 수 있지만 공백은 포함될 수 없습니다. 예를 들어 게시자 ID가 `testpublisherid` 이고 를 입력하면 제안 웹 주소는 가 `test-offer-1` `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` 됩니다.
- 이 ID는 **만들기** 를 선택한 후에는 변경할 수 없습니다.

### <a name="determine-your-offer-alias"></a>제안 별칭 확인

제안 별칭은 파트너 센터 제안에 사용되는 이름입니다. 또한 아래 지침을 따르는 적절한 제안 별칭이 필요합니다.

- 이 이름은 마켓플레이스에서 사용되지 않으며 고객에게 표시되는 제품 이름 및 기타 값과 다릅니다.
- 이 이름은 만들기를 선택한 후에는 변경할 수 없습니다.

## <a name="create-your-offer"></a>제품 만들기

라이선스 프로세스의 첫 번째 단계는 상업용 Marketplace 제안을 만드는 것입니다. 

1. [파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.
2. 왼쪽 탐색 메뉴에서 **상업용 마켓플레이스/개요** 를 선택 합니다.
3. 개요 페이지의 맨 위에서 **새 제품** 을 선택 하 고 **고객 Engagement & PowerApps에 대해 Dynamics 365을** 선택 합니다.
4. 이전에 만든 **제품 ID** 및 제품 **별칭** 을 입력 합니다.
5. **만들기** 를 선택하여 제품을 생성하고 계속합니다.
6. 라이선스 옵션을 선택 합니다.

    - 제품에 대 한 라이선스 관리를 사용 하도록 설정 하려면 **Microsoft에서 앱 라이선스 관리 사용** 을 선택 합니다. 이는 일회성 설정 이며 제품이 게시 된 후에는 변경할 수 없습니다.

    - 고객이 라이선스 없이 앱의 기본 기능을 실행 하도록 설정 하 고, 라이선스를 구매한 후에 프리미엄 기능을 실행할 수도 있습니다. 이렇게 하려면 **라이선스가 할당 되지 않은 경우에도 고객이 앱을 설치할 수 있도록 허용** 을 선택 합니다.

    - 제품에서 라이선스 관리를 사용 하도록 설정 하지 않으려는 경우 **지금 받기 (무료)**, **무료 평가판** 또는 **문의처** 를 선택 합니다.

## <a name="create-your-plan"></a>계획 만들기

이러한 단계에서는 제품에 대해 사용 하도록 설정 하려는 계획을 정의 합니다.

1. 왼쪽 탐색 메뉴에서 **계획 개요** 를 선택한 다음 **새 계획 만들기** 를 선택 합니다.
2. **계획 ID** 및 **계획 이름을** 입력 하 고 **만들기** 를 선택 합니다.
3. **계획 목록** 페이지에서 **계획 설명을** 입력 합니다.
4. 설명을 저장 하 고 나중에 완료 하려면 **초안 저장** 을 선택 합니다.

5. 완료 되 면 **검토 및 게시** 를 선택 합니다. 이제 계획 정보가 제품 목록 (계획 섹션) 아래 appsource.microsoft.com에 표시 됩니다.

6. 이 제품에 대 한 모든 계획을 만든 후에는 각 계획의 서비스 ID를 복사 해야 합니다. 계획 목록 페이지의 맨 위에서 **계획 개요** 를 선택 합니다. 각 계획에 대 한 서비스 ID를 안전한 위치에 복사 합니다.

## <a name="add-service-ids-to-your-solution"></a>솔루션에 서비스 Id 추가

다음 단계는 방금 복사한 각 계획에 대한 서비스 ID를 추가하여 솔루션을 업데이트하는 것입니다. 이에 대한 지침은 [솔루션에 대한 AppSource 패키지 만들기를 참조하세요.](/powerapps/developer/data-platform/create-package-app-appsource)

## <a name="upload-your-package-and-publish-your-offer"></a>패키지 업로드 및 제안 게시

1. 왼쪽 탐색 창에서 **상업용 Marketplace** 를 선택한 다음, **기술 구성을** 선택합니다.
2. **기본 라이선스 모델에서** **사용자** 를 선택합니다.
3. **CRM 패키지** 에서 패키지 위치의 URL을 입력합니다.
4. 왼쪽 탐색 창의 다른 탭을 사용하여 다른 필수 정보를 입력합니다. 완료되면 **검토 및 게시를** 선택합니다.

제안을 게시한 후에는 정보를 검토하고 확인합니다. 이 프로세스에 문제가 있는 경우 알려드리겠습니다. 모든 문제가 해결되면 AppSource에서 제안을 사용할 수 있다는 알림이 표시됩니다. 이 시점에서 라이브로 만들 수 있습니다.

## <a name="make-your-offer-live-in-partner-center"></a>파트너 센터 라이브로 제공

아래 절차에서는 AppSource에서 제안을 라이브로 만드는 과정을 안내합니다. 이 프로세스에 대한 자세한 내용은 [목록 옵션 소개를 참조하세요.](/azure/marketplace/determine-your-listing-type)

>[!NOTE]
>제안을 게시하면 라이브로 이동하는 데 4-6시간이 걸립니다.

1. [파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.
2. 왼쪽 탐색 메뉴에서 **상업용 Marketplace/개요를** 선택합니다.
3. **개요** 페이지에서 찾고 있는 제안을 찾습니다. 게시할 준비가 된 제안의 상태는 **미리 보기** 입니다. 제안을 선택합니다.
4. **제품 개요** 페이지에서 **라이브 이동** 을 선택 합니다.
제품은 4-6 시간 이내에 라이브 됩니다.
5. AppSource에 대 한 제품 목록을 보려면 **제품 개요** 페이지의 맨 아래에 있는 **appsource** 링크를 선택 합니다.

    - **라이선스가 지원 되는 제품의** 경우: 제품에 라이선스 확인이 필요한 경우 사용자는 연락처를 클릭 하 여 잠재 고객에 **게 연락** 하 여 통신할 수 있습니다.

    - **무료 설치 옵션을 사용 하는 라이선스 사용 제품의** 경우: 제품에 라이선스 확인이 필요 하지 않은 경우 관리자에 **게 연락** 뿐만 아니라 **지금 가져오기** 단추가 표시 됩니다. 무료 설치 옵션을 시도 하려는 사용자는 **지금 가져오기** 를 클릭 해야 합니다. 그러면 Power Platform 관리 센터에 제품을 설치 하 게 됩니다. 사용자는 궁금한 점이 있거나 유료 요금제로 업그레이드 하려는 경우에도 사용자 **에 게 연락** 하는 것을 사용할 수 있습니다.

## <a name="register-isv-connect-deal-in-deal-registration"></a>ISV 연결을 위한 등록 처리 등록

고객에 게 라이선스를 할당 하려면 먼저 각 판매를 파트너 센터에 등록 해야 합니다. 이렇게 하려면 [거래 등록](register-deals.md)을 참조 하세요.

## <a name="invite-the-customer"></a>고객 초대

다음 절차를 사용 하 여 고객에 게이 거래에 참여할 수 있도록 초대 합니다.  

1. [파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.
2. 왼쪽 탐색 메뉴에서 **상업용 마켓플레이스/개요** 를 선택 합니다.
3. 왼쪽 탐색 메뉴에서 **조회** 를 선택 하 고 **거래 등록** 을 선택 합니다.
4. **제출** 된 거래에 대해 필터링 하 고 **진행** 중인 탭을 선택한 후 원하는 거래를 선택 합니다.
5. 이 거래의 개요 페이지에서 **라이선스 관리** 를 선택 합니다.
6. **라이선스 관리** 창의 **고객 세부 정보** 드롭다운 목록에서 고객을 선택 합니다. 고객 관계가 아직 없는 경우 **+ 새 고객 초대를 선택 하 여 동의** 합니다.
7. 표시 되는 링크를 복사 합니다.
8. 이 링크를 고객의 청구 관리자 또는 전역 관리자에 게 전자 메일로 보내고,이 링크를 사용 하 여 admin.microsoft.com에 액세스 하 고, 사용자가 설정 하는 관계를 승인 하 고 권한을 부여 합니다.

    >[!NOTE]
    >고객이 이 단계를 수행할 때까지 관계가 설정되지 않습니다.

## <a name="activate-manage-and-remove-your-licenses"></a>라이선스 활성화, 관리 및 제거

고객이 사용자와의 관계에 권한을 부여하면 제안에서 계획을 추가하고 각 플랜에 라이선스를 할당할 수 있습니다.

1. 이 계약의 라이선스 관리 창에서 **+계획 추가를** 선택합니다.
2. 이 **솔루션에 대한 계획** 및 **라이선스 수** 필드를 완료한 다음, 라이선스 **업데이트를 선택합니다.** 고객이 직원을 관리하고 할당할 수 있도록 admin.microsoft.com 라이선스를 사용할 수 있습니다.

    - 기존 플랜의 라이선스 수를 변경하려면 **라이선스 수** 필드에 새 번호를 입력한 **다음, 라이선스 업데이트를 선택합니다.**

    - 거래 라이선스를 비활성화하거나 제거하려면 **작업** 필드에서 휴지통 아이콘을 선택한 **다음, 라이선스 업데이트를 선택합니다.**

## <a name="next-steps"></a>다음 단계

[라이선스 리소스](support-resources-licensing.md)