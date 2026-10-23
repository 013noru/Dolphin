# 📢 패치노트

> **안내**: 돌고래 서버의 신규 컨텐츠 업데이트, 시스템 개편, 밸런스 조정 및 버그 수정 내역을 기록하는 공식 패치노트입니다.  
> 어떤 내용이 변경되었는지 쉽게 확인하고 기록할 수 있도록 최신 업데이트 순서대로 정리됩니다.

---

## 📑 업데이트 기록 바로가기

* [2026. 10. 23 업데이트](#2026-10-23-업데이트)
* [2026. 10. 22 업데이트](#2026-10-22-업데이트)
* [2026. 10. 21 업데이트](#2026-10-21-업데이트)

---

## 2026. 10. 23 업데이트

> 📢 **오늘의 업데이트 핵심 한눈에 보기 (선반영)**
> * 🌟 **직업 특성 자동 마스터 랭크업(Rank-up) 시스템 도입**: 특성 선택 후 레벨 도달 시 별도 포인트 없이 2단계(⭐⭐) 및 3단계(⭐⭐⭐)로 특성 자동 강화
> * ⚖️ **4대 생활 직업 전 직업 특성 밸런스 및 명칭 전면 개편**: 광부·농부·어부·사냥꾼 특성의 쿨다운, 발동 확률, 범위, 효과 전면 상향 및 신규 특성 배치

---

### 🌟 직업 특성 마스터 랭크업 및 전면 리밸런싱
* **자동 마스터 랭크업 시스템 신규 적용**:
  * 각 생활 직업은 **Lv. 5, 15, 30, 50, 80** 달성 시 티어별로 **2가지 특성 중 하나를 선택(2중 택 1)**합니다.
  * 별도의 스킬 포인트 소모 없이, 캐릭터의 직업 레벨이 도달함에 따라 **자동으로 2단계(⭐⭐) 또는 3단계(⭐⭐⭐)로 마스터 랭크업**되어 효과 수치 증가 및 쿨다운 단축 혜택이 적용됩니다.
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

---

## 2026. 10. 22 업데이트

> 📢 **오늘의 업데이트 핵심 한눈에 보기**
> * 🌟 **4대 생활 직업 5단계 특성 추가**: 광부·농부·어부·사냥꾼 레벨에 따라 2중 택 1 고유 특성 해금 (`/직업`)
> * 🎣 **수중 통발 어부 경험치 대폭 상향**: 통발 수확 시 획득 경험치 대폭 증가 (최대 1,500 EXP, 최대 20배)
> * ⛏️ **디 엔드 신규 광물 배치**: 엔드 차원 전역에 철 자원을 수급하는 **엔드 철 광석** 신규 생성
> * ⚔️ **+20강 장비 강화 & 대장기술 정돈**: 네더라이트 모루 강화 시스템 오픈 및 1~5티어 합금 주괴 연동
> * 🐛 **버그 수정 및 시스템 안정화**: 밭 블럭 맨손/도구 채굴 시 증발 문제 해결, 화로 호퍼 경험치 무한 파밍 꼼수 원천 차단

---

### 🌟 직업 특성 시스템 추가
* **4대 생활 직업 전용 특성 트리 신규 도입**: 광부, 농부, 어부, 사냥꾼 직업 육성 시 레벨에 따라 고유 패시브 및 액티브 능력을 해금할 수 있는 5단계 특성 트리가 추가되었습니다. ([🌲 생활 직업 및 특성](guide/06-1.md) 참고)
* **특성 해금 구간 (2중 택 1)**:
  * 각 생활 직업 **Lv. 5, Lv. 15, Lv. 30, Lv. 50, Lv. 80** 달성 시마다 2가지 특성 중 하나를 자유롭게 선택할 수 있습니다.
* **직업별 5단계 특성 트리 도감**:

{% tabs %}
{% tab title="⛏️ 광부 (Miner)" %}
<table>
  <thead>
    <tr>
      <th align="center" width="120">해금 레벨</th>
      <th width="320">[선택 A]</th>
      <th width="320">[선택 B]</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center"><strong>Lv. 5</strong></td>
      <td><strong>가벼운 곡괭이</strong><br>• 채굴 시 5초 동안 <strong>신속 II</strong><br>• <em>(내부 쿨다운: 15초)</em></td>
      <td><strong>지식의 광석</strong><br>• 광부 직업 경험치 <strong>+10%</strong><br>• 광석 채굴 시 바닐라 경험치 <strong>+2</strong><br>• <em>(패시브 상시 적용)</em></td>
    </tr>
    <tr>
      <td align="center"><strong>Lv. 15</strong></td>
      <td><strong>광부의 도파민</strong><br>• 채굴 시 10% 확률로 6초간 <strong>성급함 II</strong><br>• <em>(내부 쿨다운: 30초)</em></td>
      <td><strong>광맥의 잔상</strong><br>• 광석 채굴 시 20% 확률로 9블록 내 광물 홀로그램 투시<br>• <em>(내부 쿨다운: 45초)</em></td>
    </tr>
    <tr>
      <td align="center"><strong>Lv. 30</strong></td>
      <td><strong>2x2 지층 파쇄</strong><br>• 채굴 시 25% 확률로 2×2(총 4칸) 일괄 파괴<br>• <em>(내부 쿨다운: 8초)</em></td>
      <td><strong>풍요의 메아리</strong><br>• 광석 채굴 시 30% 확률로 원석 1~2개 추가 드롭<br>• <em>(내부 쿨다운: 5초)</em></td>
    </tr>
    <tr>
      <td align="center"><strong>Lv. 50</strong></td>
      <td><strong>연쇄 채광 (Vein Mining)</strong><br>• 광석 채굴 시 연결된 광맥 <strong>최대 32개</strong> 일괄 연쇄 채굴<br>• <em>(내부 쿨다운: 60초)</em></td>
      <td><strong>황금빛 대박</strong><br>• 광석 채굴 시 <strong>원석 +2개 추가 드롭</strong><br>• <em>(내부 쿨다운: 60초)</em></td>
    </tr>
    <tr>
      <td align="center"><strong>Lv. 80</strong></td>
      <td><strong>대지의 숨결</strong><br>• 채굴 시 5% 확률로 배고픔 1칸 + 체력 1칸 회복 &amp; 곡괭이 내구도 1 수리<br>• <em>(패시브 상시 적용)</em></td>
      <td><strong>고대 지층 발굴</strong><br>• Y &lt; 0 채굴 시 1% 확률로 고대 잔해 파편 발견<br>• <em>(내부 쿨다운: 60초)</em></td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="🌾 농부 (Farmer)" %}
<table>
  <thead>
    <tr>
      <th align="center" width="120">해금 레벨</th>
      <th width="320">[선택 A]</th>
      <th width="320">[선택 B]</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center"><strong>Lv. 5</strong></td>
      <td><strong>풍요의 만찬</strong><br>• 수확 시 5% 확률로 배고픔 2칸 + 체력 2칸 회복 &amp; 괭이 내구도 2 수리<br>• <em>(패시브 상시 적용)</em></td>
      <td><strong>풍요의 씨앗</strong><br>• 농부 직업 경험치 <strong>+10%</strong><br>• 수확 시 바닐라 경험치 <strong>+1</strong><br>• <em>(내부 쿨다운: 5초)</em></td>
    </tr>
    <tr>
      <td align="center"><strong>Lv. 15</strong></td>
      <td><strong>씨앗 감정사</strong><br>• 수확 시 5% 확률로 <strong>해당 커스텀 씨앗 1개 획득</strong><br>• <em>(내부 쿨다운: 10초)</em></td>
      <td><strong>효율적 수확</strong><br>• 수확 시 5% 확률로 <strong>주변 작물 일괄 수확 (1단계로 보존)</strong><br>• <em>(내부 쿨다운: 10초)</em></td>
    </tr>
    <tr>
      <td align="center"><strong>Lv. 30</strong></td>
      <td><strong>풍요의 손길</strong><br>• 수확 시 10% 확률로 <strong>완제품 작물 +1개 추가 드롭</strong><br>• <em>(내부 쿨다운: 20초)</em></td>
      <td><strong>대지의 파동</strong><br>• 수확 시 10% 확률로 <strong>주변 작물 마지막 단계 즉시 성장</strong><br>• <em>(내부 쿨다운: 30초)</em></td>
    </tr>
    <tr>
      <td align="center"><strong>Lv. 50</strong></td>
      <td><strong>보라빛 결실</strong><br>• 수확 시 10% 확률로 <strong>최고급 보라별 작물 1개</strong> 지급<br>• <em>(내부 쿨다운: 60초)</em></td>
      <td><strong>황금빛 결실</strong><br>• 수확 시 10% 확률로 <strong>황금 당근/황금 사과</strong> 드롭<br>• <em>(내부 쿨다운: 30초)</em></td>
    </tr>
    <tr>
      <td align="center"><strong>Lv. 80</strong></td>
      <td><strong>대지의 광맥</strong><br>• 수확 시 10% 확률로 <strong>바닐라/커스텀 주괴 및 광물</strong> 발굴<br>• <em>(내부 쿨다운: 60초)</em></td>
      <td><strong>고대 대지의 유물</strong><br>• 수확 시 0.5% 확률로 <strong>고대 잔해 (Ancient Debris)</strong> 발굴<br>• <em>(내부 쿨다운: 60초)</em></td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="🎣 어부 (Fisherman)" %}
<table>
  <thead>
    <tr>
      <th align="center" width="120">해금 레벨</th>
      <th width="320">[선택 A]</th>
      <th width="320">[선택 B]</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center"><strong>Lv. 5</strong></td>
      <td><strong>잽싼 챔질</strong><br>• 낚시 찌 입질 대기시간 <strong>20% 단축</strong><br>• <em>(패시브 상시 적용)</em></td>
      <td><strong>지식의 낚싯바늘</strong><br>• 어부 직업 경험치 <strong>+10%</strong><br>• 낚시 성공 시 바닐라 경험치 <strong>+3</strong><br>• <em>(패시브 상시 적용)</em></td>
    </tr>
    <tr>
      <td align="center"><strong>Lv. 15</strong></td>
      <td><strong>통발 장인</strong><br>• 통발 수확 시 통발 온전 회수 확률 <strong>+15%</strong><br>• <em>(패시브 상시 적용)</em></td>
      <td><strong>바다의 직감</strong><br>• 입질 실패 시 30% 확률로 자동 챔질 성공<br>• <em>(내부 쿨다운: 15초)</em></td>
    </tr>
    <tr>
      <td align="center"><strong>Lv. 30</strong></td>
      <td><strong>쌍둥이 월척</strong><br>• 낚시 성공 시 30% 확률로 동일 수확물 <strong>+1마리(총 2개)</strong><br>• <em>(내부 쿨다운: 10초)</em></td>
      <td><strong>심해의 보물 사냥꾼</strong><br>• 쓰레기 낚시 제거 + 보물 인양 확률 <strong>+20%</strong><br>• <em>(패시브 상시 적용)</em></td>
    </tr>
    <tr>
      <td align="center"><strong>Lv. 50</strong></td>
      <td><strong>소나기의 가호</strong><br>• 비/눈/뇌우 시 바닐라 경험치 <strong>2배 (+100%)</strong><br>• <em>(패시브 - 날씨 조건부)</em></td>
      <td><strong>소나기의 풍어</strong><br>• 낚시 시 <strong>30% 확률로 미끼(Bait) 소모 무효화</strong><br>• <em>(패시브 상시 적용)</em></td>
    </tr>
    <tr>
      <td align="center"><strong>Lv. 80</strong></td>
      <td><strong>바다의 가호</strong><br>• 낚시 시 20% 확률로 배고픔 2칸 + 체력 2칸 회복 &amp; 낚싯대 내구도 2 수리<br>• <em>(내부 쿨다운: 60초)</em></td>
      <td><strong>고대 심해 발굴</strong><br>• 낚시 시 1% 확률로 <strong>고대 잔해 (Ancient Debris)</strong> 낚음<br>• <em>(내부 쿨다운: 60초)</em></td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="🏹 사냥꾼 (Hunter)" %}
<table>
  <thead>
    <tr>
      <th align="center" width="120">해금 레벨</th>
      <th width="320">[선택 A]</th>
      <th width="320">[선택 B]</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center"><strong>Lv. 5</strong></td>
      <td><strong>사냥의 도파민</strong><br>• 처치 시 15% 확률로 <strong>5초간 신속 II + 재생 I</strong><br>• <em>(내부 쿨다운: 20초)</em></td>
      <td><strong>추적자의 지혜</strong><br>• 사냥꾼 직업 경험치 <strong>+10%</strong><br>• 처치 시 바닐라 경험치 <strong>+5</strong><br>• <em>(패시브 상시 적용)</em></td>
    </tr>
    <tr>
      <td align="center"><strong>Lv. 15</strong></td>
      <td><strong>전투 광란</strong><br>• 처치 시 50% 확률로 <strong>배고픔 1칸 + 체력 1칸 회복</strong><br>• <em>(패시브 상시 적용)</em></td>
      <td><strong>날카로운 추격</strong><br>• 타격 시 10% 확률로 <strong>1.5배 피해 + 둔화 II (3초)</strong><br>• <em>(내부 쿨다운: 10초)</em></td>
    </tr>
    <tr>
      <td align="center"><strong>Lv. 30</strong></td>
      <td><strong>약탈자의 손길</strong><br>• 처치 시 15% 확률로 <strong>사냥 전리품 +1회 추가 추첨</strong><br>• <em>(내부 쿨다운: 20초)</em></td>
      <td><strong>연쇄 타격</strong><br>• 타격 시 10% 확률로 <strong>주변 5블록 범위 피해</strong><br>• <em>(내부 쿨다운: 15초)</em></td>
    </tr>
    <tr>
      <td align="center"><strong>Lv. 50</strong></td>
      <td><strong>거물 사냥꾼</strong><br>• 체력 100 이상 또는 보스 처치 시 <strong>전리품 2배 + 직업 경험치 2배</strong><br>• <em>(내부 쿨다운: 5분)</em></td>
      <td><strong>현상금 사냥꾼</strong><br>• 처치 시 10% 확률로 <strong>500 ~ 1,500 골드</strong> 획득<br>• <em>(내부 쿨다운: 2분)</em></td>
    </tr>
    <tr>
      <td align="center"><strong>Lv. 80</strong></td>
      <td><strong>피의 축제</strong><br>• 처치 시 10초간 <strong>힘 II + 화염 저항 &amp; 피해량 15% 흡혈</strong><br>• <em>(내부 쿨다운: 60초)</em></td>
      <td><strong>고대 사냥터의 유물</strong><br>• 처치 시 0.5% 확률로 <strong>고대 잔해 (Ancient Debris)</strong> 드롭<br>• <em>(내부 쿨다운: 60초)</em></td>
    </tr>
  </tbody>
</table>
{% endtab %}
{% endtabs %}
* **특성 관리 GUI**:
  * 채팅창에 `/직업` (`/job`, `/wlrdjq`) 입력 후 원하는 생활 직업 아이콘을 클릭하여 언제든지 특성을 선택하거나 활성화할 수 있습니다.
* **내부 쿨다운(ICD) 및 공정성 적용**:
  * 확률 발동형 고효율 특성에는 개별 내부 쿨다운이 적용되어 과도한 성능 왜곡을 방지하고 균형 잡힌 플레이를 지원합니다.

### 🎣 수중 통발(CustomFishTraps) 어부 경험치 대폭 상향
* **통발 등급별 어부 직업 경험치(EXP) 상향**: 통발 등급과 대기 소요 시간(30분 ~ 12시간)에 걸맞은 수준으로 수확 시 획득하는 어부 직업 경험치를 대폭 상향 조정하였습니다. ([🌲 생활 직업 및 특성](guide/06-1.md) 통발 도감 연동)
* **등급별 경험치 수치 변경 내역**:
  * **브론즈 통발** (소요 시간: 30분): 기존 30 EXP ➔ **150 EXP** *(+400%, 5.0배)*
  * **실버 통발** (소요 시간: 1시간): 기존 36 EXP ➔ **250 EXP** *(+594%, 약 6.9배)*
  * **골드 통발** (소요 시간: 1.5시간): 기존 45 EXP ➔ **400 EXP** *(+788%, 약 8.9배)*
  * **다이아몬드 통발** (소요 시간: 2시간): 기존 52 EXP ➔ **650 EXP** *(+1,150%, 12.5배)*
  * **플래티넘 통발** (소요 시간: 8시간): 기존 60 EXP ➔ **950 EXP** *(+1,483%, 약 15.8배)*
  * **신화 통발** (소요 시간: 12시간): 기존 75 EXP ➔ **1,500 EXP** *(+1,900%, 20.0배)*

### ⛏️ 신규 광물: 엔드 철 광석(`end_iron_ore`) 월드 생성 추가
* **디 엔드 차원 신규 광물 배치**: 엔드 차원 탐험 중 철 자원을 안정적으로 채취할 수 있도록 **엔드 철 광석**이 월드 자연 생성(`placed_features`)에 신규 추가되었습니다.
* **월드 생성 스펙**:
  * **생성 위치**: 엔드 차원 전역 **Y 15 ~ 80** (엔드 섬 하단 절벽부터 상층부까지 폭넓게 분포)
  * **광맥 크기 및 빈도**: 광맥당 **4개**, 청크당 빈도 **10회** (엔드 차원 내에서 가장 흔하게 스폰되는 핵심 자원)
  * **대체 블록**: 엔드 돌(`minecraft:end_stone`)
* **채굴 및 드롭 특성**:
  * **채굴 도구 난이도**: `Level 1` (나무 곡괭이 이상 모든 곡괭이로 채굴 가능)
  * **블록 물리 성질**: 엔드 돌의 단단한 성질을 계승하여 **경도 3.0 / 폭발 저항 9.0** 적용
  * **드롭 아이템**: 채굴 시 네더 금광석과 유사하게 **철 조각(`iron_nugget`) 2~6개** 및 바닐라 경험치 1~2 EXP 드롭 (행운 마법부여 시 드롭량 증가)
  * **실크터치 및 제련**: 섬세한 손길 채굴 시 광석 블록 획득, 화로 및 용광로에 제련 시 **철 주괴 1개** 획득

### 🐛 버그 수정 및 이슈 해결
* **농사용 밭 블럭(`dry_pot`, `wet_pot`) 채굴 및 드롭 정상화**:
  * **기존 문제**: 플레이어가 도끼가 아닌 다른 도구(맨손, 삽, 곡괭이, 괭이 등)로 밭 블럭을 캘 경우 아이템이 드롭되지 않고 증발하던 현상이 발생했습니다.
  * **원인 및 조치**: 블록의 도끼 전용 강제 제한(`correct_tools`)을 해제하고 채굴 가속 태그(`mineable/axe`)로 개편하였습니다.
  * **개선 결과**:
    * 이제 **맨손, 삽, 곡괭이, 괭이 등 어떤 도구로 파괴하더라도 밭 블럭 아이템이 100% 정상 드롭**됩니다.
    * 도끼로 채굴 시 고유의 빠른 속도 보너스는 그대로 유지됩니다.
    * 젖은 밭 블럭(`wet_pot`) 파괴 시에도 인벤토리 파편화를 방지하기 위해 기본 밭 블럭(`dry_pot`)으로 통일되어 깔끔하게 회수됩니다.
* **화로 경험치 은행(XP Bank) 꼼수 및 감자·목탄 경험치 무한 파밍 방어 (`UtilityCore`)**:
  * **기존 문제**: 화로 아래에 깔때기(호퍼)를 설치하여 감자나 목탄을 대량으로 구워낸 뒤, 화로를 부술 때 마인크래프트 내부 NBT(`RecipesUsed`)에 누적된 대량의 경험치 구슬이 한꺼번에 쏟아져 나와 악용되던 바닐라 취약점이 발견되었습니다.
  * **원인 및 조치**:
    1. **호퍼 자동 추출 시 누적 경험치 즉시 초기화**: 호퍼 및 호퍼 마인카트가 화로/훈연기/용광로에서 아이템을 추출할 때마다 화로 내부의 누적 경험치 기록을 즉시 비워 자동화 꼼수를 100% 원천 무력화했습니다.
    2. **화로 파괴 시 잔여 경험치 드롭 차단**: 화로/훈연기/용광로 블록을 부술 때 바닥으로 경험치 구슬이 일괄 드롭되지 않도록 안전 처리했습니다.
    3. **감자 및 목탄 경험치 0 고정**: 구운 감자(`BAKED_POTATO`) 및 목탄(`CHARCOAL`)을 화로에서 직접 꺼낼 때 경험치 지급을 0으로 강제 설정했습니다.
    4. *(※ 철, 금, 구리 등 정상 광석 제련 및 일반 요리는 바닐라 경험치가 정상 지급됩니다.)*

---

## 2026. 10. 21 업데이트

### 📖 통합 가이드북 체계 개편
* **체계적 유저 가이드북 구축**: 튜토리얼부터 경제, 마을, 직업, 스킬, 인챈트, 편의 기능, VIP 혜택까지 체계화된 공식 위키 가이드 구축
* **커스텀 인챈트 총도감 수록**: 157종 커스텀 인챈트의 등급별(D~SS) 상세 발동 확률 및 효과 스펙 총도감 작성
* **VIP 회원 혜택 분리**: 일반 편의 기능과 VIP 전용 치장(16색 발광, 파티클, 무제한 플라이) 혜택 명확화
