#수정중

# 🤖 협동로봇 스마트 생산 시스템 구축 프로젝트

경기인력개발원 [스마트로봇엔지니어] 과정 중 3조가 진행한 협동로봇 기반 스마트 생산 시스템 프로젝트입니다.  
**단순 반복 작업은 로봇에게, 핵심 역량은 작업자에게!**  

> 📅 기간: 2025년 5월 28 ~ 6월 27일  
> 👥 팀원: 성**(조장), 김**, 김명지(pmhyang69@naver.com), 유**, 정**, 정**  
---

## 🧠 프로젝트 개요

- **문제 인식:** 산업 현장에서 반복 작업과 고령화로 인한 작업자 부상 위험 증가
- **해결 방법:** 협동로봇을 활용하여 Pick & Place / Drilling / Sorting 등 반복 작업 자동화
- **기대 효과:**
  - 작업자 부담 경감
  - 공정 유연성 확보
  - 생산성 향상 및 자동화 효율성 증가
 
---

## 📍 공정 레이아웃
<p align="">
  <img src="./images/Overall_process.png" width="800"/>
</p>

---

## 🧰 프로젝트 구성

### 📦 공정 구성

| 공정 | 설명 |
|------|------|
| **Pick & Place** | 로봇이 제품을 집고 센싱을 합니다. 금속 & 근접 센서가 부품을 감지하면 로봇이 가공단계로 부품을 이동합니다. |
| **Drilling & Tapping** | 반사센서를 이용해 부품이 정위치에 놓였는지 감지 후, 드릴링 머신으로 정밀하게 구멍을 가공합니다. |
| **Sorting** | QR 스캐너로 제품 정보를 인식하여 정보별로 구분합니다. |

---

### 🧪 공정별 실습 & 시연

#### 🔹 Pick & Place

<p align="">
  <img src="./images/pickplace_demo.gif" width="500" style="margin-right:10px;"/>
</p>

> 작업순서
<p align="">
  <img src="./images/pickplace_steps.png" width="700" style="margin-right:10px;"/>
</p>  

- 공정 선택, 수동 조작, 설정, 알람, 통계 메뉴 등으로 구성
- 직관적인 아이콘 기반 UI와 실시간 센서 I/O 모니터링 제공

> 공정컨셉
<p align="">
  <img src="./images/pickplace_concept.png" width="700" style="margin-right:10px;"/>
</p>

---

#### 🔹 Drilling & Tapping

<p align="">
  <img src="./images/pickplace_demo.gif" width="500" style="margin-right:10px;"/>
</p>

> 작업순서
<p align="">
  <img src="./images/drilling_steps.png" width="700" style="margin-right:10px;"/>
</p>

> 공정컨셉
<p align="">
  <img src="./images/drilling_concept.png" width="700" style="margin-right:10px;"/>
</p>

---

#### 🔹 Sorting

<p align="">
  <img src="./images/pickplace_demo.gif" width="500" style="margin-right:10px;"/>
</p>

> 작업순서
<p align="">
  <img src="./images/sorting_steps.png" width="700" style="margin-right:10px;"/>
</p>

> 공정컨셉
<img src="./images/sorting_concept.png" width="700" style="margin-right:10px;"/>


---



### 🎛️ HMI 화면 구성

- 공정 선택, 수동 조작, 설정, 알람, 통계 메뉴 등으로 구성
- 직관적인 아이콘 기반 UI와 실시간 센서 I/O 모니터링 제공
<p align="center">
  <img src="./images/hmi_overview.png" width="45%"/>
  <img src="./images/hmi_settings.png" width="45%"/>
</p>


---

### 🔌 전장 설계

- PLC 기반 전장 시스템 설계 (EPLAN 사용)
- 입력/출력 단자 설계
- CC-Link를 통한 각 공정 간 통신
<p align="center">
  <img src="./images/enclosure_overview.png" width="45%"/>
  <img src="./images/electrical_overview.png" width="45%"/>
</p>

---

## 🛠️ 트러블슈팅 사례

| 문제 | 원인 | 해결 방법 |
|------|------|-----------|
| 로봇 관절이 비정상적으로 회전 | 비효율적인 티칭 경로 | 관절 1, 5 위주로 재티칭 |
| 공압실린더가 작동 안 됨 | 3선식 오토스위치 노후 | 2선식 스위치로 교체 후 배선 수정 |
| AUBO I/O 출력 불안정 | SMPS 출력 전압 강하 | 릴레이 및 커패시터 추가하여 회로 안정화 |

### 📸 트러블슈팅 사진

#### 🔹 로봇 관절 회전 이상
<table> <tr> <td align="center"><img src="./images/trouble_pose_1.jpg" width="250"/></td> <td align="center"><img src="./images/trouble_pose_2.jpg" width="250"/></td> <td align="center"><img src="./images/trouble_pose_3.jpg" width="250"/></td> </tr> <tr> <td align="center">문제 발생 시 동작</td> <td align="center">해결과정</td> <td align="center">재티칭 후 정상 동작</td> </tr> </table>

#### 🔹 공압실린더 문제
<p align="center">
  <img src="./images/trouble_switch_1.jpg" width="300"/>
  <img src="./images/trouble_switch_2.jpg" width="300"/>
</p>

#### 🔹 AUBO I/O 출력 불안정
<p align="center">
  <img src="./images/trouble_voltage_1.jpg" width="300"/>
  <img src="./images/trouble_voltage_2.jpg" width="300"/>
</p>


---

## 📹 프로젝트 시연

### 금속 부품 공정

<p align="center">
  <img src="./images/metal_demo.gif" width="500"/>
</p>

### 플라스틱 부품 공정

<p align="center">
  <img src="./images/plastic_demo.gif" width="500"/>
</p>

---

## 📆 작업 히스토리

1. 아이디어 회의 및 역할 분담  
2. 공정 설계 → 시뮬레이션  
3. EPLAN 회로 설계  
4. PLC 래더 로직 구현  
5. AUBO 로봇 티칭 및 테스트  
6. HMI 화면 구성  
7. 통합 테스트 및 디버깅  

> 전체 프로젝트는 약 3주 동안 진행되었습니다.

---


## 📁 관련 자료

- [`📄 프로젝트 결과 PDF`](./프로젝트명_콘스탄틴.pdf)
- 전체 영상: 별도 드라이브 또는 링크 제공 예정 (GIF 일부 포함)

---

## 🔚 마무리

> 이 프로젝트를 통해 협동로봇의 실무 적용 가능성과 자동화 설계 전 과정을 체험할 수 있었습니다.  
> 로봇 제어, 센서 회로, 전장 설계, 티칭, HMI까지 연계된 경험은 현장 중심의 성장 기회였습니다.

---

