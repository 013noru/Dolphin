# 📢 패치노트

> **안내**: 돌고래 서버의 컨텐츠 업데이트, 시스템 변경, 밸런스 조정 및 버그 수정 내역을 기록하는 공식 패치노트입니다.

---

## 📑 업데이트 기록 바로가기

* [2026. 10. 25 업데이트 미리보기](#2026-10-25-업데이트-미리보기)
* [2026. 10. 23 업데이트](#2026-10-23-업데이트)
* [2026. 10. 22 업데이트](#2026-10-22-업데이트)
* [2026. 10. 21 업데이트](#2026-10-21-업데이트)

---

## 2026. 10. 25 업데이트 미리보기

> 📢 **업데이트 핵심 한눈에 보기 (미리보기)**
> * 📜 **신규 호미 전용 인챈트 2종 추가**: 스컬크 일괄 채굴 `스컬크 수확` 및 경험치 2~3배 증폭 `스컬크 흡수` (A등급)
> * 🏆 **도감 점수 티어제 & 전용 칭호 연동**: 수집 점수 기반 8단계 티어 도입 및 티어 달성 시 전용 칭호 자동 해금
> * 🖥️ **도감 메인 GUI 프로필 개편**: 내 도감 점수, 티어 랭크, 승급 진행도 바 확인 기능 추가
> * 📢 **유저 전용 글로벌 확성기(`/확성기`) 신설**: 5분 쿨다운 및 50,000원으로 전 서버 브로드캐스트 확성기 사용 가능
> * 🍲 **요리 섭취 지원금 알림 UI 개선**: 채팅창 메시지에서 화면 하단 액션바(ActionBar, 2초 유지) 출력으로 변경

---

### 📜 신규 커스텀 인챈트 추가
* **호미 전용 신규 A등급 인챈트 2종 추가**:
  * `스컬크 수확(sculkharvest)`과 `스컬크 흡수(sculkabsorb)`는 상호 배타적으로 적용되어 하나의 호미에 동시 부여할 수 없습니다.

<table>
  <thead>
    <tr>
      <th width="140">인챈트명</th>
      <th align="center" width="70">등급</th>
      <th align="center" width="85">최대 레벨</th>
      <th align="center" width="90">쿨다운</th>
      <th width="130">적용 도구</th>
      <th>효과 및 상세 스펙</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>스컬크 수확</strong><br>(<code>sculkharvest</code>)</td>
      <td align="center">A</td>
      <td align="center">1</td>
      <td align="center">0.5초</td>
      <td>모든 호미<br>(<code>ALL_HOE</code>)</td>
      <td>• 스컬크 블록 채굴 시 인접한 스컬크 블록을 <strong>최대 9개(1+8)까지 일괄 채굴</strong><br>• <strong>섬세한 손길 연동</strong>: 섬세한 손길 보유 시 블록 아이템 드롭, 미보유 시 고유 XP 구슬 드롭<br>• <strong>도구 보호</strong>: 호미 내구도가 1 이하일 경우 발동 중단 및 도구 파괴 방지<br>• 대상 블록: 스컬크, 스컬크 촉매, 스컬크 감지체, 조율된 스컬크 감지체, 스컬크 비명체, 스컬크 맥</td>
    </tr>
    <tr>
      <td><strong>스컬크 흡수</strong><br>(<code>sculkabsorb</code>)</td>
      <td align="center">A</td>
      <td align="center">1</td>
      <td align="center">없음</td>
      <td>모든 호미<br>(<code>ALL_HOE</code>)</td>
      <td>• 섬세한 손길이 없는 호미로 스컬크 블록 채굴 시 드롭되는 <strong>경험치 2~3배 증폭</strong><br>• 기본 스컬크: 1 XP ➔ <strong>2 ~ 3 XP</strong><br>• 스컬크 촉매: 20 XP ➔ <strong>40 ~ 60 XP</strong><br>• 스컬크 감지체 / 비명체: 5 XP ➔ <strong>10 ~ 15 XP</strong><br>• 발동 시 스컬크 영혼 파티클 및 전용 사운드 출력</td>
    </tr>
  </tbody>
</table>

### 🏆 도감 점수 티어제 & 전용 칭호 시스템
* **도감 완주 점수 기반 8단계 티어 도입**:
  * 도감 페이지를 완주할 때마다 획득하는 수집 점수(E등급: 1점 ~ SS등급: 64점)의 누적치에 따라 8단계 티어가 부여됩니다.
  * 새로운 티어 기준 점수 달성 시 해당 티어의 **전용 칭호가 즉시 영구 해금**되며 전 서버 네트워크에 동기화됩니다.

<table>
  <thead>
    <tr>
      <th align="center" width="130">티어 등급</th>
      <th align="center" width="95">요구 점수</th>
      <th width="160">GUI 대표 아이콘</th>
      <th width="140">해금 칭호 ID</th>
      <th>칭호 인게임 출력</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center"><strong>브론즈 수집가</strong></td>
      <td align="center">0점</td>
      <td>구리 주괴</td>
      <td><code>col_bronze</code></td>
      <td><span style="color:#CD7F32;">[브론즈 수집가]</span></td>
    </tr>
    <tr>
      <td align="center"><strong>실버 수집가</strong></td>
      <td align="center">50점</td>
      <td>철 주괴</td>
      <td><code>col_silver</code></td>
      <td><span style="color:#C0C0C0;">[실버 수집가]</span></td>
    </tr>
    <tr>
      <td align="center"><strong>골드 수집가</strong></td>
      <td align="center">150점</td>
      <td>금 주괴</td>
      <td><code>col_gold</code></td>
      <td><span style="color:#FFD700;">[골드 수집가]</span></td>
    </tr>
    <tr>
      <td align="center"><strong>플래티넘 수집가</strong></td>
      <td align="center">350점</td>
      <td>다이아몬드</td>
      <td><code>col_platinum</code></td>
      <td><span style="color:#E5E4E2;">[플래티넘 수집가]</span></td>
    </tr>
    <tr>
      <td align="center"><strong>다이아 수집가</strong></td>
      <td align="center">700점</td>
      <td>네더라이트 강화 형판</td>
      <td><code>col_diamond</code></td>
      <td><span style="color:#B9F2FF;">[다이아 수집가]</span></td>
    </tr>
    <tr>
      <td align="center"><strong>마스터 수집가</strong></td>
      <td align="center">1,500점</td>
      <td>네더의 별</td>
      <td><code>col_master</code></td>
      <td><span style="color:#BA55D3;">[마스터 수집가]</span></td>
    </tr>
    <tr>
      <td align="center"><strong>그랜드마스터</strong></td>
      <td align="center">3,000점</td>
      <td>드래곤 알</td>
      <td><code>col_grandmaster</code></td>
      <td><span style="color:#FF4500;">[그랜드마스터]</span></td>
    </tr>
    <tr>
      <td align="center"><strong>챌린저</strong></td>
      <td align="center">6,000점</td>
      <td>무거운 코어</td>
      <td><code>col_challenger</code></td>
      <td><span style="color:#FFD700; font-weight:bold;">[챌린저]</span></td>
    </tr>
  </tbody>
</table>

* **도감 메인 GUI 프로필 슬롯 추가**:
  * `/도감` 메인 GUI 0번 슬롯에 [내 도감 정보] 프로필 아이콘이 추가되었습니다.
  * 총 도감 점수, 현재 달성 티어, 다음 목표 티어까지 남은 점수, 승급 진행도 바(`■■■■■■□□□□ 60.0%`), 현재 착용 가능한 전용 칭호가 표시됩니다.

### 📢 확성기 및 알림 시스템 개편
* **유저 확성기(`/확성기`) 신설**:
  * 전 서버의 유저들에게 메시지를 브로드캐스트하는 `/확성기 <메시지>` 명령어가 추가되었습니다.
  * **사용 비용**: 1회 50,000 코인
  * **재사용 대기시간**: 5분 (300초)
  * **출력 형태**: 네온 라임/일렉트릭 민트 그라데이션 발신자 닉네임 표기 한 줄 브로드캐스트
* **관리자 공지(`/공지`) 분리**:
  * 기존 확성기에서 관리자 전용 글로벌 공지 기능이 `/공지` 명령어로 분리되었습니다.
* **요리 섭취 보상 알림 UI 개선**:
  * 요리 섭취 시 획득하는 랜덤 코인 지원금 안내가 채팅창 메시지에서 **화면 하단 액션바(ActionBar, 2초 노출 후 자동 제거)**로 변경되었습니다.

---

## 2026. 10. 23 업데이트

> 📢 **오늘의 업데이트 핵심 한눈에 보기 (선반영)**
> * 🌟 **직업 특성 마스터 랭크업 시스템 추가**: 특성 선택 후 레벨 도달 시 2단계(⭐⭐) 및 3단계(⭐⭐⭐)로 특성 자동 강화
> * ⚖️ **4대 생활 직업 특성 리밸런싱**: 광부·농부·어부·사냥꾼 특성의 쿨다운, 발동 확률, 효과 수치 조정 및 신규 특성 배치
> * ⚗️ **연금술 양조 경험치 & 피로도 수치 조정**: 포션 양조 완료 시 획득하는 AuraSkills 연금술 경험치 1.5배 상향 및 양조 소모 피로도 갱신

---

### 🌟 직업 특성 마스터 랭크업 및 리밸런싱
* **마스터 랭크업 시스템 적용**:
  * 각 생활 직업 **Lv. 5, 15, 30, 50, 80** 달성 시 2가지 특성 중 하나를 선택(2중 택 1)합니다.
  * 직업 레벨 도달 시 선택된 특성이 **자동으로 2단계(⭐⭐) 또는 3단계(⭐⭐⭐)로 마스터 랭크업**되어 효과 수치 및 쿨다운이 변경됩니다.
* **직업별 5단계 특성 트리 및 마스터 랭크 요약**:

{% tabs %}
{% tab title="⛏️ 광부 특성 트리" %}
<table>
  <thead>
    <tr>
      <th align="center" width="120">티어 (해금 Lv)</th>
      <th width="330">[선택 A 특성]</th>
      <th width="330">[선택 B 특성]</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center"><strong>Tier 1</strong><br>(Lv. 5)</td>
      <td><strong>가벼운 곡괭이</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 5)</strong>: 채굴 시 5초간 <strong>신속 I</strong> (쿨 30초)<br>• ⭐⭐ <strong>2단계 (Lv. 60)</strong>: 채굴 시 5초간 <strong>신속 I</strong> (쿨 <strong>15초</strong>)<br>• <em>(내부 쿨다운 적용)</em></td>
      <td><strong>지식의 광석</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 5)</strong>: 직업 EXP <strong>+10%</strong> / 바닐라 EXP <strong>+2</strong><br>• ⭐⭐ <strong>2단계 (Lv. 60)</strong>: 직업 EXP <strong>+15%</strong> / 바닐라 EXP <strong>+3</strong><br>• <em>(패시브 상시 적용)</em></td>
    </tr>
    <tr>
      <td align="center"><strong>Tier 2</strong><br>(Lv. 15)</td>
      <td><strong>광부의 도파민</strong> <em>(3단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 15)</strong>: 채굴 시 10% 확률 <strong>성급함 (6초)</strong> (쿨 30초)<br>• ⭐⭐ <strong>2단계 (Lv. 40)</strong>: 채굴 시 10% 확률 <strong>성급함 (8초)</strong> (쿨 30초)<br>• ⭐⭐⭐ <strong>3단계 (Lv. 70)</strong>: 채굴 시 10% 확률 <strong>성급함 (10초)</strong> (쿨 30초)</td>
      <td><strong>광맥의 잔상</strong> <em>(3단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 15)</strong>: 광석 채굴 시 10% 확률 <strong>반경 8블록</strong> 광물 투시 (쿨 60초)<br>• ⭐⭐ <strong>2단계 (Lv. 40)</strong>: 광석 채굴 시 10% 확률 <strong>반경 10블록</strong> 광물 투시 (쿨 60초)<br>• ⭐⭐⭐ <strong>3단계 (Lv. 70)</strong>: 광석 채굴 시 10% 확률 <strong>반경 14블록</strong> 광물 투시 (쿨 60초)</td>
    </tr>
    <tr>
      <td align="center"><strong>Tier 3</strong><br>(Lv. 30)</td>
      <td><strong>지층 파쇄</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 30)</strong>: 채굴 시 10% 확률 <strong>2×2 파괴</strong> (쿨 30초)<br>• ⭐⭐ <strong>2단계 (Lv. 85)</strong>: 채굴 시 10% 확률 <strong>3×3 (총 9칸) 파괴</strong> (쿨 30초)</td>
      <td><strong>연쇄 채광</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 30)</strong>: 광맥 <strong>최대 32개 일괄 파괴</strong> (쿨 60초)<br>• ⭐⭐ <strong>2단계 (Lv. 85)</strong>: 광맥 <strong>최대 64개 일괄 파괴</strong> (쿨 60초)</td>
    </tr>
    <tr>
      <td align="center"><strong>Tier 4</strong><br>(Lv. 50)</td>
      <td><strong>은빛 결실</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 50)</strong>: 광석 채굴 시 <strong>5% 확률</strong> 원석 +1 추가 드롭 (쿨 60초)<br>• ⭐⭐ <strong>2단계 (Lv. 95)</strong>: 광석 채굴 시 <strong>10% 확률</strong> 원석 +1 추가 드롭 (쿨 60초)</td>
      <td><strong>금빛 결실</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 50)</strong>: 광석 채굴 시 <strong>5% 확률</strong> 완제품 +1개 추가 지급 (쿨 60초)<br>• ⭐⭐ <strong>2단계 (Lv. 95)</strong>: 광석 채굴 시 <strong>10% 확률</strong> 완제품 +1개 추가 지급 (쿨 60초)<br>• <em>(섬세한 손길 곡괭이 제외)</em></td>
    </tr>
    <tr>
      <td align="center"><strong>Tier 5</strong><br>(Lv. 80)</td>
      <td><strong>대지의 숨결</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 80)</strong>: 채굴 시 3% 확률 배고픔 1칸 + 체력 1칸 + 내구도 1 수리 (쿨 60초)<br>• ⭐⭐ <strong>2단계 (Lv. 100)</strong>: 채굴 시 <strong>5% 확률</strong> 배고픔 2칸 + 체력 2칸 + 내구도 1 수리 (쿨 60초)</td>
      <td><strong>고대 지층 발굴</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 80)</strong>: <strong>심층암</strong> 채굴 시 <strong>0.1% 확률</strong>로 고대 잔해 발견 (쿨 60초)<br>• ⭐⭐ <strong>2단계 (Lv. 100)</strong>: <strong>심층암</strong> 채굴 시 <strong>0.2% 확률</strong>로 고대 잔해 발견 (쿨 60초)</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="🌾 농부 특성 트리" %}
<table>
  <thead>
    <tr>
      <th align="center" width="120">티어 (해금 Lv)</th>
      <th width="330">[선택 A 특성]</th>
      <th width="330">[선택 B 특성]</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center"><strong>Tier 1</strong><br>(Lv. 5)</td>
      <td><strong>풍요의 만찬</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 5)</strong>: 수확 시 5% 확률 배고픔 2칸 + 체력 2칸 + 괭이 내구도 2 수리<br>• ⭐⭐ <strong>2단계 (Lv. 60)</strong>: 수확 시 <strong>10% 확률</strong> 배고픔 3칸 + 체력 3칸 + <strong>괭이 내구도 4 수리</strong><br>• <em>(패시브 상시)</em></td>
      <td><strong>풍요의 씨앗</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 5)</strong>: 직업 EXP <strong>+10%</strong> / 바닐라 EXP <strong>+1</strong> (쿨 5초)<br>• ⭐⭐ <strong>2단계 (Lv. 60)</strong>: 직업 EXP <strong>+15%</strong> / 바닐라 EXP <strong>+2</strong> (쿨 <strong>3초</strong>)<br>• <em>(내부 쿨다운 적용)</em></td>
    </tr>
    <tr>
      <td align="center"><strong>Tier 2</strong><br>(Lv. 15)</td>
      <td><strong>씨앗 감정사</strong> <em>(CustomCrops / 3단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 15)</strong>: 수확 시 <strong>1% 확률</strong> 커스텀 씨앗 1개 획득 (쿨 40초)<br>• ⭐⭐ <strong>2단계 (Lv. 40)</strong>: 수확 시 <strong>2% 확률</strong> 커스텀 씨앗 1개 획득 (쿨 40초)<br>• ⭐⭐⭐ <strong>3단계 (Lv. 70)</strong>: 수확 시 <strong>4% 확률</strong> 커스텀 씨앗 1개 획득 (쿨 40초)</td>
      <td><strong>풍작</strong> <em>(3단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 15)</strong>: 수확 시 <strong>10% 확률</strong>로 동일 작물(별 등급 동일) +1개 지급 (쿨 40초)<br>• ⭐⭐ <strong>2단계 (Lv. 40)</strong>: 수확 시 <strong>10% 확률</strong>로 동일 작물(별 등급 동일) +1개 지급 (쿨 40초)<br>• ⭐⭐⭐ <strong>3단계 (Lv. 70)</strong>: 수확 시 <strong>10% 확률</strong>로 동일 작물(별 등급 동일) +1개 지급 (쿨 40초)</td>
    </tr>
    <tr>
      <td align="center"><strong>Tier 3</strong><br>(Lv. 30)</td>
      <td><strong>대지의 행운</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 30)</strong>: 수확 시 <strong>2% 확률</strong> 황금 당근 또는 황금 사과 드롭 (쿨 60초)<br>• ⭐⭐ <strong>2단계 (Lv. 85)</strong>: 수확 시 <strong>3% 확률</strong> 황금 당근 또는 황금 사과 드롭 (쿨 60초)</td>
      <td><strong>대지의 파동</strong> <em>(CustomCrops / 2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 30)</strong>: 수확 시 <strong>2% 확률</strong> 반경 <strong>3블록</strong> 작물 1단계 성장 (쿨 60초)<br>• ⭐⭐ <strong>2단계 (Lv. 85)</strong>: 수확 시 <strong>5% 확률</strong> 반경 <strong>5블록</strong> 작물 1단계 성장 (쿨 60초)</td>
    </tr>
    <tr>
      <td align="center"><strong>Tier 4</strong><br>(Lv. 50)</td>
      <td><strong>보라빛 결실</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 50)</strong>: 수확 시 <strong>2% 확률</strong> 최고급 보라별 작물 1개 지급 (쿨 60초)<br>• ⭐⭐ <strong>2단계 (Lv. 95)</strong>: 수확 시 <strong>3% 확률</strong> 최고급 보라별 작물 1개 지급 (쿨 60초)</td>
      <td><strong>풍요의 손길</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 50)</strong>: 수확 시 <strong>5% 확률</strong> 완제품 작물 <strong>+2개 드롭</strong> (쿨 60초)<br>• ⭐⭐ <strong>2단계 (Lv. 95)</strong>: 수확 시 <strong>10% 확률</strong> 완제품 작물 <strong>+2개 드롭</strong> (쿨 60초)</td>
    </tr>
    <tr>
      <td align="center"><strong>Tier 5</strong><br>(Lv. 80)</td>
      <td><strong>드러난 광물</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 80)</strong>: 수확 시 <strong>2% 확률</strong> 기본 광물·주괴 발굴 (합금 제외, 쿨 60초)<br>• ⭐⭐ <strong>2단계 (Lv. 100)</strong>: 수확 시 <strong>3% 확률</strong> 기본 광물·주괴 발굴 (합금 제외, 쿨 60초)</td>
      <td><strong>고대 대지의 유물</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 80)</strong>: 수확 시 <strong>0.1% 확률</strong>로 고대 잔해 발굴 (쿨 60초)<br>• ⭐⭐ <strong>2단계 (Lv. 100)</strong>: 수확 시 <strong>0.2% 확률</strong>로 고대 잔해 발굴 (쿨 60초)</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="🎣 어부 특성 트리" %}
<table>
  <thead>
    <tr>
      <th align="center" width="120">티어 (해금 Lv)</th>
      <th width="330">[선택 A 특성]</th>
      <th width="330">[선택 B 특성]</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center"><strong>Tier 1</strong><br>(Lv. 5)</td>
      <td><strong>잽싼 챔질</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 5)</strong>: 입질 대기시간 <strong>10% 단축</strong><br>• ⭐⭐ <strong>2단계 (Lv. 60)</strong>: 입질 대기시간 <strong>20% 단축</strong><br>• <em>(패시브 상시)</em></td>
      <td><strong>지식의 낚싯바늘</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 5)</strong>: 직업 EXP <strong>+10%</strong> / 바닐라 EXP <strong>+3</strong><br>• ⭐⭐ <strong>2단계 (Lv. 60)</strong>: 직업 EXP <strong>+15%</strong> / 바닐라 EXP <strong>+5</strong><br>• <em>(패시브 상시)</em></td>
    </tr>
    <tr>
      <td align="center"><strong>Tier 2</strong><br>(Lv. 15)</td>
      <td><strong>통발 장인</strong> <em>(CustomFishTraps / 3단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 15)</strong>: 통발 회수율 <strong>+10%</strong>, 통발 직업 EXP <strong>+10%</strong><br>• ⭐⭐ <strong>2단계 (Lv. 40)</strong>: 통발 회수율 <strong>+12%</strong>, 통발 직업 EXP <strong>+12%</strong><br>• ⭐⭐⭐ <strong>3단계 (Lv. 70)</strong>: 통발 회수율 <strong>+15%</strong>, 통발 직업 EXP <strong>+15%</strong><br>• <em>(패시브 상시)</em></td>
      <td><strong>무아지경</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 15)</strong>: 입질 반응 실패 시 <strong>25% 확률 자동 챔질</strong> (쿨 30초)<br>• ⭐⭐ <strong>2단계 (Lv. 70)</strong>: 입질 반응 실패 시 <strong>50% 확률 자동 챔질</strong> (쿨 30초)</td>
    </tr>
    <tr>
      <td align="center"><strong>Tier 3</strong><br>(Lv. 30)</td>
      <td><strong>쌍둥이 월척</strong> <em>(3단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 30)</strong>: 낚시 성공 시 <strong>10% 확률</strong> 잡힌 물고기 <strong>2배 복제 지급</strong> (쿨 60초)<br>• ⭐⭐ <strong>2단계 (Lv. 65)</strong>: <strong>15% 확률</strong> 잡힌 물고기 2배 복제 지급 (쿨 60초)<br>• ⭐⭐⭐ <strong>3단계 (Lv. 85)</strong>: <strong>30% 확률</strong> 잡힌 물고기 2배 복제 지급 (쿨 60초)</td>
      <td><strong>보물 낚시꾼</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 30)</strong>: 낚시 성공 시 <strong>10% 확률</strong> 보물 인양 (쿨 60초)<br>• ⭐⭐ <strong>2단계 (Lv. 85)</strong>: 낚시 성공 시 <strong>20% 확률</strong> 보물 인양 (쿨 60초)<br>• <em>(보물: 인챈트북, 앵무조개 껍질, 이름표, 안장 등)</em></td>
    </tr>
    <tr>
      <td align="center"><strong>Tier 4</strong><br>(Lv. 50)</td>
      <td><strong>소나기의 가호</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 50)</strong>: 우천 시 바닐라 EXP <strong>2배 (+100%)</strong> (쿨 20초)<br>• ⭐⭐ <strong>2단계 (Lv. 95)</strong>: 우천 시 바닐라 EXP <strong>3배 (+200%)</strong> (쿨 20초)</td>
      <td><strong>미끼 재활용</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 50)</strong>: 낚시 시 <strong>15% 확률</strong> 미끼 소모 무효화 (쿨 20초)<br>• ⭐⭐ <strong>2단계 (Lv. 95)</strong>: 낚시 시 <strong>30% 확률</strong> 미끼 소모 무효화 (쿨 20초)</td>
    </tr>
    <tr>
      <td align="center"><strong>Tier 5</strong><br>(Lv. 80)</td>
      <td><strong>바다의 가호</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 80)</strong>: 낚시 성공 시 <strong>1% 확률</strong> 낚싯대 내구도 <strong>3 수리</strong><br>• ⭐⭐ <strong>2단계 (Lv. 100)</strong>: 낚시 성공 시 <strong>2% 확률</strong> 낚싯대 내구도 <strong>3 수리</strong><br>• <em>(패시브 상시)</em></td>
      <td><strong>심해의 심장</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 80)</strong>: 낚시 성공 시 <strong>0.1% 확률</strong>로 <strong>바다의 심장(Heart of the Sea)</strong> 낚음<br>• ⭐⭐ <strong>2단계 (Lv. 100)</strong>: 낚시 성공 시 <strong>0.2% 확률</strong>로 <strong>바다의 심장</strong> 낚음<br>• <em>(패시브 상시)</em></td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="🏹 사냥꾼 특성 트리" %}
<table>
  <thead>
    <tr>
      <th align="center" width="120">티어 (해금 Lv)</th>
      <th width="330">[선택 A 특성]</th>
      <th width="330">[선택 B 특성]</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center"><strong>Tier 1</strong><br>(Lv. 5)</td>
      <td><strong>사냥의 도파민</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 5)</strong>: 처치 시 15% 확률 5초간 <strong>신속 II + 재생 I</strong> (쿨 20초)<br>• ⭐⭐ <strong>2단계 (Lv. 60)</strong>: 처치 시 <strong>20% 확률 7초간 신속 II + 재생 II</strong> (쿨 <strong>15초</strong>)<br>• <em>(내부 쿨다운 적용)</em></td>
      <td><strong>추적자의 지혜</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 5)</strong>: 직업 EXP <strong>+10%</strong> / 바닐라 EXP <strong>+5</strong><br>• ⭐⭐ <strong>2단계 (Lv. 60)</strong>: 직업 EXP <strong>+15%</strong> / 바닐라 EXP <strong>+10</strong><br>• <em>(패시브 상시)</em></td>
    </tr>
    <tr>
      <td align="center"><strong>Tier 2</strong><br>(Lv. 15)</td>
      <td><strong>전투 광란</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 15)</strong>: 처치 시 <strong>30% 확률</strong>로 <strong>배고픔 1칸 + 체력 1칸 회복</strong><br>• ⭐⭐ <strong>2단계 (Lv. 70)</strong>: 처치 시 <strong>50% 확률</strong>로 <strong>배고픔 2칸 + 체력 2칸 회복</strong><br>• <em>(패시브 상시)</em></td>
      <td><strong>피의 축제</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 15)</strong>: 처치 시 <strong>30% 확률</strong>로 5초간 <strong>흡혈 + 이동속도 +5%</strong> (쿨 10초)<br>• ⭐⭐ <strong>2단계 (Lv. 70)</strong>: 처치 시 <strong>50% 확률</strong>로 5초간 <strong>흡혈 + 이동속도 +10%</strong> (쿨 10초)</td>
    </tr>
    <tr>
      <td align="center"><strong>Tier 3</strong><br>(Lv. 30)</td>
      <td><strong>강화 타격</strong> <em>(3단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 30)</strong>: 타격 시 <strong>10% 확률 1.5배 피해</strong> (쿨 10초)<br>• ⭐⭐ <strong>2단계 (Lv. 65)</strong>: 타격 시 <strong>15% 확률 1.8배 피해</strong> (쿨 10초)<br>• ⭐⭐⭐ <strong>3단계 (Lv. 85)</strong>: 타격 시 <strong>20% 확률 2.0배 피해</strong> (쿨 10초)</td>
      <td><strong>광역 타격</strong> <em>(3단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 30)</strong>: 타격 시 <strong>10% 확률</strong>로 <strong>반경 5블록 피해 15</strong> (쿨 20초)<br>• ⭐⭐ <strong>2단계 (Lv. 65)</strong>: 타격 시 <strong>15% 확률</strong>로 <strong>반경 5블록 피해 15</strong> (쿨 20초)<br>• ⭐⭐⭐ <strong>3단계 (Lv. 85)</strong>: 타격 시 <strong>20% 확률</strong>로 <strong>반경 5블록 피해 15</strong> (쿨 20초)</td>
    </tr>
    <tr>
      <td align="center"><strong>Tier 4</strong><br>(Lv. 50)</td>
      <td><strong>거물 사냥꾼</strong> <em>(MythicMobs / 2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 50)</strong>: <strong>체력 50 이상 대상</strong> 타격 시 <strong>데미지 1.5배</strong> (쿨 20초)<br>• ⭐⭐ <strong>2단계 (Lv. 95)</strong>: <strong>체력 50 이상 대상</strong> 타격 시 <strong>데미지 2.0배</strong> (쿨 20초)</td>
      <td><strong>현상금 사냥꾼</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 50)</strong>: 처치 시 <strong>5% 확률 500~1,500원</strong> 드롭 (쿨 120초)<br>• ⭐⭐ <strong>2단계 (Lv. 95)</strong>: 처치 시 <strong>10% 확률 1,000~2,000원</strong> 드롭 (쿨 <strong>90초</strong>)</td>
    </tr>
    <tr>
      <td align="center"><strong>Tier 5</strong><br>(Lv. 80)</td>
      <td><strong>추가 약탈</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 80)</strong>: 처치 시 <strong>5% 확률</strong>로 전리품 1회 추가 추첨 (쿨 60초)<br>• ⭐⭐ <strong>2단계 (Lv. 100)</strong>: 처치 시 <strong>10% 확률</strong>로 전리품 1회 추가 추첨 (쿨 60초)</td>
      <td><strong>고대 잔해 약탈</strong> <em>(2단계 마스터)</em><br>• ⭐ <strong>1단계 (Lv. 80)</strong>: 처치 시 <strong>0.2% 확률</strong>로 <strong>고대 잔해(Ancient Debris)</strong> 드롭<br>• ⭐⭐ <strong>2단계 (Lv. 100)</strong>: 처치 시 <strong>0.5% 확률</strong>로 <strong>고대 잔해</strong> 드롭<br>• <em>(쿨다운 없음 / 상시 패시브)</em></td>
    </tr>
  </tbody>
</table>
{% endtab %}
{% endtabs %}

### ⚗️ 연금술 양조 경험치 & 소모 피로도 조정
* **AuraSkills 연금술 경험치(`aura_exp`) 1.5배 (+50%) 상향 조정**:
  * 포션 양조 완료 시 획득하는 AuraSkills 연금술 경험치(`aura_exp`)가 기존 수치 대비 1.5배로 상향되었습니다.
  * **0단계 베이스 포션**: 어색한 포션 `30.0` ➔ **`45.0 EXP`**
  * **1단계 특수 포션 (20초/30초군 10종)**: `1,500` ➔ **`2,250 EXP`**
  * **1단계 특수 포션 (40초/45초군 9종)**: `2,000` ➔ **`3,000 EXP`**
  * **1단계 특수 포션 (50초 상급군 2종)**: `2,500` ➔ **`3,750 EXP`**
  * **2단계 강화 & 연장 포션 (전체 45종)**: `800` ➔ **`1,200 EXP`**
  * **특수 강화 포션 (빛나는 체력 포션)**: `20.0` ➔ **`30.0 EXP`**
* **양조 소모 피로도(`fatigue`) 수치 조정**:
  * **1단계 특수 포션 전 품목 (21종)**: 1회 소모 피로도 `4` ➔ **`16`**
  * **2단계 강화 & 연장 포션 (45종)**: 1회 소모 피로도 `1` ➔ **`4`**
  * **특수 강화 포션 (빛나는 체력 포션)**: 1회 소모 피로도 `2` ➔ **`8`**

#### 📊 포션 등급별 양조 수치 변동표
| 포션 단계 및 분류 | 대표 품목 | 양조 시간 | 1회 소모 피로도 | 직업 EXP | 기존 Aura EXP | 변경 Aura EXP | 변동률 |
| :--- | :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| **0단계 베이스** | 어색한 포션 | 5초 | 0 | 0 | 30.0 | **45.0** | **+50% (1.5배)** |
| **1단계 기초 (20~30초)** | 정령의 호흡, 요정의 축복, 번개 걸음 등 10종 | 20~30초 | **16** *(구 4)* | 100 | 1,500 | **2,250** | **+50% (1.5배)** |
| **1단계 중급 (40~45초)** | 그림자 망토, 불사조의 가호, 태양의 치유 등 9종 | 40~45초 | **16** *(구 4)* | 100 | 2,000 | **3,000** | **+50% (1.5배)** |
| **1단계 상급 (50초)** | 세계수의 활력, 베히모스의 분노 | 50초 | **16** *(구 4)* | 100 | 2,500 | **3,750** | **+50% (1.5배)** |
| **2단계 발광석 농축** | 농축된 포션 20종 | 15초 | **4** *(구 1)* | 150 | 800 | **1,200** | **+50% (1.5배)** |
| **2단계 레드스톤 안정화** | 안정된 포션 25종 | 15초 | **4** *(구 1)* | 150 | 800 | **1,200** | **+50% (1.5배)** |
| **특수 강화 포션** | 빛나는 체력 포션 (Lv. 10) | 25초 | **8** *(구 2)* | 20 | 20.0 | **30.0** | **+50% (1.5배)** |

---

## 2026. 10. 22 업데이트

> 📢 **오늘의 업데이트 핵심 한눈에 보기**
> * 🌟 **4대 생활 직업 5단계 특성 추가**: 광부·농부·어부·사냥꾼 레벨에 따라 2중 택 1 특성 해금 (`/직업`)
> * 🎣 **수중 통발 어부 경험치 상향**: 통발 수확 시 획득 어부 경험치 조정 (150 ~ 1,500 EXP)
> * ⛏️ **디 엔드 신규 광물 배치**: 엔드 차원(Y 15 ~ 80)에 **엔드 철 광석** 자연 생성 추가
> * ⚔️ **+20강 장비 강화 & 합금 연동**: 네더라이트 모루 강화 시스템 추가 및 1~5티어 합금 주괴 수리망치 연동
> * 🐛 **버그 수정**: 밭 블럭 채굴 시 아이템 미드롭 버그 수정, 화로 호퍼 경험치 누적 꼼수 수정

---

### 🌟 직업 특성 시스템 추가
* **4대 생활 직업 전용 특성 트리 도입**: 광부, 농부, 어부, 사냥꾼 직업에 5단계 특성 트리가 추가되었습니다. ([🌲 생활 직업 및 특성](guide/06-1.md) 참고)
* **특성 해금 구간 (2중 택 1)**:
  * 각 생활 직업 **Lv. 5, Lv. 15, Lv. 30, Lv. 50, Lv. 80** 달성 시마다 2가지 특성 중 하나를 선택합니다.
* **특성 관리 GUI**:
  * 채팅창에 `/직업` (`/job`, `/wlrdjq`) 입력 후 생활 직업 아이콘을 클릭하여 특성을 선택합니다.
* **내부 쿨다운(ICD) 적용**:
  * 확률 발동형 특성에 개별 내부 쿨다운이 적용됩니다.

### ⚔️ 장비 강화 시스템 도입
* **대장장이 작업대 강화 시스템 추가**: 네더라이트 모루 블록에서 무기 및 방어구를 최대 +20강까지 강화할 수 있습니다. ([💎 강화](guide/09-4.md) 참고)
* **2가지 강화 루트**:
  * **일반 강화**: 플라즈마 합금 주괴를 소모하여 타이밍 미니게임을 통해 강화 진행
  * **확정 강화**: 드래곤 알 1개를 소모하여 +4강 ➔ +5강부터 +14강 ➔ +15강 구간을 100% 확률로 강화
* **천장 시스템**:
  * **하락 천장**: 강화 등급 하락 시 하락 스택을 적립하여 다음 강화 성공 시 이전 단계로 복구
  * **장인의 기운**: +15강 이상 구간에서 실패 시 실패 스택을 누적하여 100% 확정 성공 지원
* **장비 귀속**: +5강 이상 강화 성공 시 해당 플레이어에게 영구 귀속 처리

### ⚒️ 아이템 조합법 및 대장기술 정돈
* **특수 수리 망치 레시피 변경**: 이전 조합대 수리 망치 레시피를 비활성화하고, 대장장이 전용 1~5티어 합금 주괴 체계로 연동했습니다.
* **조합법 가이드 정리**: 05번 문서 1~7번 대단락 번호 체계 및 2번 합금 제련표 최상단 망치 주괴 목록 배치

### 💼 생활 및 전문 직업 시스템 개편
* **/직업경험치 명령어 이동**: 채광, 수확, 낚시, 사냥 시 경험치와 드롭 확률을 확인하는 `/직업경험치` 명령어를 생활 직업([🌲 생활 직업 및 특성](guide/06-1.md)) 문서로 재배치했습니다.
* **전문 직업 개요 탭 분리**: [🔨 전문 직업 및 제작](guide/06-2.md) 문서 1번 개요를 대장장이, 요리사, 연금술사, 마법부여사 탭으로 분리하고 요리 및 포션 양조 레시피 표를 추가했습니다.

### 🎣 수중 통발(CustomFishTraps) 어부 경험치 상향
* **통발 등급별 어부 직업 경험치(EXP) 상향**: 통발 수확 시 획득하는 어부 직업 경험치가 상향 조정되었습니다. ([🌲 생활 직업 및 특성](guide/06-1.md) 통발 도감 연동)
* **등급별 경험치 수치 변경 내역**:
  * **브론즈 통발** (소요 시간: 30분): 기존 30 EXP ➔ **150 EXP** *(5.0배)*
  * **실버 통발** (소요 시간: 1시간): 기존 36 EXP ➔ **250 EXP** *(약 6.9배)*
  * **골드 통발** (소요 시간: 1.5시간): 기존 45 EXP ➔ **400 EXP** *(약 8.9배)*
  * **다이아몬드 통발** (소요 시간: 2시간): 기존 52 EXP ➔ **650 EXP** *(12.5배)*
  * **플래티넘 통발** (소요 시간: 8시간): 기존 60 EXP ➔ **950 EXP** *(약 15.8배)*
  * **신화 통발** (소요 시간: 12시간): 기존 75 EXP ➔ **1,500 EXP** *(20.0배)*

### ⛏️ 신규 광물: 엔드 철 광석(`end_iron_ore`) 추가
* **디 엔드 차원 월드 자연 생성(`placed_features`) 추가**:
  * **생성 위치**: 엔드 차원 **Y 15 ~ 80**
  * **광맥 크기 및 빈도**: 광맥당 **4개**, 청크당 빈도 **10회**
  * **대체 블록**: 엔드 돌(`minecraft:end_stone`)
* **채굴 및 드롭 설정**:
  * **채굴 요구 도구**: `Level 1` (나무 곡괭이 이상)
  * **블록 경도 및 폭발 저항**: 경도 3.0 / 폭발 저항 9.0
  * **드롭 아이템**: 일반 채굴 시 **철 조각(`iron_nugget`) 2~6개** 및 경험치 1~2 EXP (행운 마법부여 적용)
  * **제련 결과**: 섬세한 손길 채굴 시 블록 획득, 화로/용광로 제련 시 **철 주괴 1개**

### 🐛 버그 수정 및 이슈 해결
* **농사용 밭 블럭(`dry_pot`, `wet_pot`) 채굴 및 드롭 수정**:
  * 도끼 외 도구(맨손, 삽, 곡괭이, 괭이 등)로 채굴 시 아이템이 드롭되지 않던 현상 수정
  * `correct_tools` 속성 제거 및 `tags: ["minecraft:mineable/axe"]` 적용 (모든 도구 및 맨손으로 채굴 시 밭 블럭 100% 드롭, 도끼 채굴 가속 유지)
  * 젖은 밭 블럭(`wet_pot`) 파괴 시 기본 밭 블럭(`dry_pot`) 아이템으로 드롭되도록 설정 통일
* **화로 호퍼 경험치 누적 및 추출 수정 (`UtilityCore`)**:
  * 호퍼 및 호퍼 마인카트가 화로/훈연기/용광로에서 아이템을 추출할 때 화로 내부의 누적 경험치(`RecipesUsed`)가 즉시 초기화되도록 수정
  * 화로/훈연기/용광로 블록 파괴 시 잔여 경험치 드롭 차단 (0 EXP)
  * 화로에서 구운 감자(`BAKED_POTATO`) 및 목탄(`CHARCOAL`) 직접 추출 시 획득 경험치 0 고정 (철, 금, 구리 등 광물 및 요리는 정상 지급)

---

## 2026. 10. 21 업데이트

### 📖 가이드북 작성 및 개편
* **가이드북 등록**: 튜토리얼, 경제, 마을, 직업, 스킬, 인챈트, 편의 기능, VIP 혜택 가이드 등록
* **커스텀 인챈트 도감 등록**: 157종 커스텀 인챈트의 등급별(D~SS) 발동 확률 및 효과 스펙 도감 등록
* **VIP 회원 혜택 분리**: 일반 편의 기능과 VIP 전용 혜택(16색 발광, 파티클, 비행) 문서 분리
