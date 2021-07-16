---
title: 분석 데이터에 프로그래밍 방식으로 액세스하기 위한 사전 요구 사항
description: 분석 데이터에 프로그래밍 방식으로 액세스하기 위한 사전 요구 사항
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d4c39025aa3804435dd4d2359b93cd4a2e13ccc4
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375863"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a>분석 데이터에 프로그래밍 방식으로 액세스하기 위한 사전 요구 사항

**적절한 역할:** 전역 관리자 | MPN 관리자

프로그래밍 방식으로 파트너 인사이트 분석 데이터에 액세스하려면 다음 요구 사항을 충족해야 합니다.

## <a name="mpn-program-enrollment"></a>MPN 프로그램 등록

파트너 인사이트 분석 데이터에 프로그래밍 방식으로 액세스하려면 MPN 프로그램에 등록하고 파트너 센터 계정이 있어야 합니다. 방법을 알아보려면 [파트너 센터 MPN 계정 만들기를](mpn-create-a-partner-center-account.md) 참조하세요.

## <a name="create-azure-active-directory-aad-application"></a>AAD(Azure Active Directory) 애플리케이션 만들기

파트너 Insights Analytics 데이터의 프로그래밍 방식 액세스에는 일반 사용자 자격 증명을 사용할 수 없습니다. 프로그래밍 방식 액세스 API에 액세스하려면 AAD(Azure Active Directory) 애플리케이션을 비밀(애플리케이션 + 사용자 액세스)과 함께 만들어야 합니다. AAD 애플리케이션 및 비밀을 만드는 방법을 알아보려면 [빠른 시작: Microsoft ID 플랫폼 애플리케이션 등록을 참조하세요.](/azure/active-directory/develop/quickstart-register-app)   Microsoft 파트너 API 액세스하려면 권한이 필요합니다. 권한을 추가하는 방법을 알아보려면 [파트너 API 인증 - 파트너를 참조하세요.](/partner/develop/api-authentication#application-and-user-access)

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a>사용자에게 ERV(Executive Report Viewer) 역할 할당

파트너 인사이트 분석 데이터에 프로그래밍 방식으로 액세스하려면 ERV(Executive Report Viewer)가 있어야 합니다. 사용자에게 ERV 역할을 할당하는 방법을 알아보려면 [파트너 센터 Insights 역할 기반 액세스 - 파트너 센터](insights-roles.md)

## <a name="generate-an-aad-token"></a>AAD 토큰 생성

애플리케이션(클라이언트) ID, 클라이언트 암호, 사용자 ID 및 암호를 사용하여 AAD 토큰을 생성해야 합니다. AAD 토큰을 생성하는 단계는   [여기를 확인하세요.](insights-programmatic-first-api-call.md#token-generation)

> [!Note]
> 이 토큰은 1시간 동안 유효합니다.

## <a name="next-steps"></a>다음 단계
[프로그래밍 방식 액세스 페러다임](insights-programmatic-access-paradigm.md)