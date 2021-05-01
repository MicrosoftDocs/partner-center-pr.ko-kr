---
title: Marketplace 제품의 라이선스 관리
ms.topic: how-to
ms.date: 04/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: ISV 상업적 marketplace 제품에 대 한 라이선스를 설정 하 고 관리 하는 방법을 알아봅니다.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3b2281696a2fe69253cd033eb2a7eef7fb3046f3
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284879"
---
# <a name="manage-licensing-in-marketplace-offers"></a>Marketplace 제품의 라이선스 관리

**적절한 역할**

- 글로벌 관리자
- 계정 관리자

이 문서에서는 파트너 센터에서 제품을 설정 하 고 Microsoft AppSource에서 사용할 수 있도록 한 다음 해당 제품에 대 한 라이선스를 관리 하는 과정을 안내 합니다.  

>[!IMPORTANT]
>이 문서의 기능은 현재 공개 미리 보기로 제공 됩니다.

## <a name="before-you-begin"></a>시작하기 전에

이 프로세스를 시작 하기 전에 아래 정보를 숙지 해야 합니다.

### <a name="review-the-azure-marketplace-documentation"></a>Azure Marketplace 설명서 검토

다음 문서에는 계속 하기 전에 알아두어야 할 정보가 포함 되어 있습니다. 

- [Dynamics 365 for Customer Engagement 및 PowerApps 제품 만들기](https://docs.microsoft.com/azure/marketplace/dynamics-365-customer-engage-offer-setup)
- [파트너 센터에서 상용 마켓플레이스 계정 만들기](https://docs.microsoft.com/azure/marketplace/create-account)

### <a name="create-your-offer-id"></a>제안 ID 만들기

아래 절차에는 제품 ID를 입력 하 라는 메시지가 표시 됩니다. 이제 다음 사항을 염두에 둔 적절 한 제안 ID를 제공 합니다.

- 이 ID는 마켓플레이스 제품 및 Azure Resource Manager 템플릿의 웹 주소에서 고객에게 표시됩니다(해당하는 경우).
- 게시자 ID와 결합 된 제품 ID의 길이는 40 자 미만 이어야 합니다.
- 소문자와 숫자만 사용할 수 있습니다. 제안 ID는 하이픈 및 밑줄을 포함할 수 있지만 공백은 포함할 수 없습니다. 예를 들어 게시자 ID가 testpublisherid이 고 테스트-1을 입력 하는 경우 제품 웹 주소는가 됩니다 https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1 .
- **만들기** 를 선택한 후에는이 ID를 변경할 수 없습니다.

### <a name="create-your-offer-alias"></a>제품 별칭 만들기

제품 별칭은 파트너 센터의 제품에 사용 되는 이름입니다. 또한 아래 지침을 따르는 적절 한 제안 별칭이 필요 합니다.

- 이 이름은 마켓플레이스에서 사용되지 않으며 고객에게 표시되는 제품 이름 및 기타 값과 다릅니다.
- 만들기를 선택한 후에는이 이름을 변경할 수 없습니다.

## <a name="create-your-offer"></a>제품 만들기

라이선스 프로세스의 첫 번째 단계는 상업적 마켓플레이스 제품을 만드는 것입니다. 

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

다음 단계는 방금 복사한 각 계획에 대 한 서비스 Id를 추가 하 여 솔루션을 업데이트 하는 것입니다. 이에 대 한 지침은 [솔루션에 대 한 AppSource 패키지 만들기](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource)를 참조 하세요.

## <a name="upload-your-package-and-publish-your-offer"></a>패키지 업로드 및 제품 게시

1. 왼쪽 탐색 창에서 **상업용 마켓플레이스** 를 선택 하 고 **기술 구성** 을 선택 합니다.
2. **기본 라이선스 모델** 아래에서 **사용자** 를 선택 합니다.
3. **CRM 패키지** 에서 패키지 위치의 URL을 입력 합니다.
4. 왼쪽 탐색 창의 다른 탭을 사용 하 여 기타 필요한 정보를 입력할 수 있습니다. 완료 되 면 **검토 및 게시** 를 선택 합니다.

제품을 게시 한 후에는 정보를 검토 하 고 확인 합니다. 이 프로세스에 문제가 있는 경우 사용자에 게 알려 드리겠습니다. 모든 문제가 해결 되 면 제품이 AppSource에서 사용 가능 하다는 알림을 받게 됩니다. 이 시점에서 라이브로 설정할 수 있습니다.

## <a name="make-your-offer-live-in-partner-center"></a>파트너 센터에서 제품을 라이브 상태로 만들기

아래 절차는 AppSource에서 제품을 라이브 상태로 만드는 과정을 안내 합니다. 이 프로세스에 대해 자세히 알아보려면 [목록 옵션 소개](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type)를 참조 하세요.

>[!NOTE]
>제품을 게시 한 후에는 사용 시간이 4-6 시간이 소요 됩니다.

1. [파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.
2. 왼쪽 탐색 메뉴에서 **상업용 마켓플레이스/개요** 를 선택 합니다.
3. **개요** 페이지에서 원하는 제품을 찾습니다. 게시할 준비가 된 제품은 **미리 보기** 상태를 갖습니다. 제품을 선택 합니다.
4. **제품 개요** 페이지에서 **라이브 이동** 을 선택 합니다.
제품은 4-6 시간 이내에 라이브 됩니다.
5. AppSource에 대 한 제품 목록을 보려면 **제품 개요** 페이지의 맨 아래에 있는 **appsource** 링크를 선택 합니다.

    - **라이선스가 지원 되는 제품의** 경우: 제품에 라이선스 확인이 필요한 경우 사용자는 연락처를 클릭 하 여 잠재 고객에 **게 연락** 하 여 통신할 수 있습니다.

    - **무료 설치 옵션을 사용 하는 라이선스 사용 제품의** 경우: 제품에 라이선스 확인이 필요 하지 않은 경우 관리자에 **게 연락** 뿐만 아니라 **지금 가져오기** 단추가 표시 됩니다. 무료 설치 옵션을 시도 하려는 사용자는 **지금 가져오기** 를 클릭 해야 합니다. 그러면 Power Platform 관리 센터에 제품을 설치 하 게 됩니다. 사용자는 궁금한 점이 있거나 유료 요금제로 업그레이드 하려는 경우에도 사용자 **에 게 연락** 하는 것을 사용할 수 있습니다.

## <a name="register-isv-connect-deal-in-dealreg"></a>DealReg의 ISV Connect 거래 등록

다음 단계는 거래를 등록 하는 것입니다. 이렇게 하려면 [거래 등록](https://docs.microsoft.com/partner-center/register-deals)을 참조 하세요.

## <a name="invite-the-customer"></a>고객 초대

다음 절차를 사용 하 여 고객에 게이 거래에 참여할 수 있도록 초대 합니다.  

1. [파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.
2. 왼쪽 탐색 메뉴에서 **상업용 마켓플레이스/개요** 를 선택 합니다.
3. **제출** 된 거래에 대해 필터링 하 고 **진행** 중인 탭을 선택한 후 원하는 거래를 선택 합니다.
4. 이 거래의 개요 페이지에서 **라이선스 관리** 를 선택 합니다.
5. **라이선스 관리** 창의 **고객 세부 정보** 드롭다운 목록에서 고객을 선택 합니다. 고객 관계가 아직 없는 경우 **+ 새 고객 초대를 선택 하 여 동의** 합니다.
6. 표시 되는 링크를 복사 합니다.
7. 이 링크를 고객의 청구 관리자 또는 전역 관리자에 게 전자 메일로 보내고,이 링크를 사용 하 여 admin.microsoft.com에 액세스 하 고, 사용자가 설정 하는 관계를 승인 하 고 권한을 부여 합니다.

    >[!NOTE]
    >관계는 고객이이 단계를 수행할 때까지 설정 되지 않습니다.

## <a name="activate-manage-and-remove-your-licenses"></a>라이선스 활성화, 관리 및 제거

고객이 설정 되 면 제품에서 요금제를 추가 하 고 각 계획에 라이선스를 할당할 수 있습니다.

1. 이 거래에 대 한 라이선스 관리 창에서 **+ 계획 추가** 를 선택 합니다.
2. **이 솔루션에 대 한 계획** 및 **라이선스 수** 필드를 완료 한 후 **라이선스 업데이트** 를 선택 합니다. 라이선스는 고객이 관리 하 고 직원에 게 할당할 수 있는 admin.microsoft.com에서 제공 됩니다.

    - 기존 계획의 라이선스 수를 변경 하려면 **라이선스 수** 필드에 새 숫자를 입력 한 다음 **라이선스 업데이트** 를 선택 합니다.

    - 거래의 라이선스를 비활성화 하거나 제거 하려면 **작업** 필드에서 휴지통 아이콘을 선택 하 고 **라이선스 업데이트** 를 선택 합니다.