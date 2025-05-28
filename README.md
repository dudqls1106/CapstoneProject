# CapstoneProject

# MooDiary

<img width="509" alt="pi" src="https://github.com/user-attachments/assets/ad70e5b5-ef3f-4a8c-9c52-d34936b19ff4">

<br>

## 프로젝트 소개

- MooDiary는 사용자의 일기 데이터를 기반으로 감정을 분석하고, 이를 시각화하여 제공하는 온디바이스 AI 기반 일기 애플리케이션입니다.
- 사용자의 편의를 위해 음성 인식 모델을 활용하여 텍스트 타이핑 및 음성 일기 작성 모두를 지원합니다.
- 사용자는 일기를 작성하며 하루를 되돌아보고, 감정 상태를 시각적으로 확인할 수 있으며, 앱이 제공하는 피드백을 통해 더 나은 하루를 설계할 수 있습니다.

<br>

## 팀원 구성

<div align="center">

| **서연수** | **성시우** | **박영빈** | **유두연** |
| :------: |  :------: | :------: | :------: |
| [<img src="https://github.com/user-attachments/assets/b8ee6c21-e044-4dcf-ade4-7ea26aa8c78c" height=150 width=150> <br/> @brynn00](https://github.com/brynn00) | [<img src="https://github.com/user-attachments/assets/05a676d3-31ae-4dc5-ba33-2bb342d952cf" height=150 width=150> <br/> @sung0368](https://github.com/sung0368) | [<img src="https://github.com/user-attachments/assets/d9ec4cf1-2319-4320-bf95-b074ad6d5bd7" height=150 width=150> <br/> @dudqls1106](https://github.com/dudqls1106) | [<img src="https://github.com/user-attachments/assets/57142a10-8c2b-43e5-b308-928823a941c4" height=150 width=150> <br/> @duyeonyoo99](https://github.com/duyeonyoo99) |

</div>

<br>

## 1. 개발 환경

- Front-end : Android XML, Java
- Back-end : Java, SQLite, Llama v3, Android STT, Google Drive API
- 버전 및 이슈관리 : Github, Github Issues, Github Project
- 협업 툴 : Discord, Notion, Slack, Figma

---



## 2. 채택한 개발 기술

### Android(Java) 기반 네이티브 앱 개발

### SQLite

- 일기 데이터, 통계 및 피드백 등의 로컬 저장소
 
### Google Drive API

- 데이터의 선택적 클라우드 백업 및 복원 기능 제공

### Llama v3

- 온디바이스에 최적화 된 LLM 기반 로컬 AI 추론 기술 제공

### Android STT

- 온디바이스 음성 인식 기능 구현으로 인터넷 연결 없이 음성 일기 작성 제공

--- 


## 3. 프로젝트 구조

```
├── .cxx
├── .gradle
├── .idea
├── gradle
├── .gitignore
├── .gitmodules
├── build.gradle
├── gradle.properties
├── gradlew
├── gradlew.bat
├── local.properties
├── settings.gradle
│
└── app
     ├── .cxx
     ├── build
     ├── java-llama.cpp
          ├── .github
          ├── models
          ├── src
          ├── target
          ├── .clang-format
          ├── .clang-tidy
          ├── .gitignore
          ├── CMakeLists.txt
          ├── LICENSE.md
          ├── pom.xml
          └── README.md
      
     └── src
          └── main
                ├── AndroidManifest.xml
                ├── java
                      ├── de.kherud.llama
                      ├── App
                      ├── AppLifecycleObserver
                      ├── CalendarActivity
                      ├── CalendarAdapter
                      ├── CalendarDay
                      ├── ColorBottomSheet
                      ├── ColorUtils
                      ├── DiaryAdapter
                      ├── DiaryDraftManager
                      ├── DiaryEntry
                      ├── DriveBackupManager
                      ├── HomeActivity
                      ├── HomeSearchActivity
                      ├── MiniCalendarAdapter
                      ├── MiniCalendarAdapterAtWrite
                      ├── MiniCalendarAtWriteDiary
                      ├── MiniCalendarDialog
                      ├── ModelManager
                      ├── MyDatabaseHelper
                      ├── SettingsActivity
                      ├── SpeechRecognizerHelper
                      ├── StatisticsActivity
                      ├── VoiceRecordActivity
                      ├── WriteDiaryHomeActivity
                      └── WritingButtonActivity

                └── res
                      ├── drawable
                              ├── bg_calendar_bubble.xml
                              ├── bg_card.xml
                              ├── bg_card2.xml
                              ├── bg_circle_green.xml
                              ├── bg_diary_card.xml
                              ├── bg_half_circle.xml
                              ├── bg_info_bubble.xml
                              ├── bg_popup.xml
                              ├── blue_button.xml
                              ├── dots_horizontal.xml
                              ├── green_button.xml
                              ├── handle_background.xml
                              ├── ic_add.xml
                              ├── ic_arrow_left.xml
                              ├── ic_arrow_right.xml
                              ├── ic_calendar.xml
                              ├── ic_calendar2.xml
                              ├── ic_calendar3.xml
                              ├── ic_chart.xml
                              ├── ic_close.xml
                              ├── ic_close2.xml
                              ├── ic_emotion_angry.xml
                              ├── ic_emotion_anxious.xml
                              ├── ic_emotion_confused.xml
                              ├── ic_emotion_group.png
                              ├── ic_emotion_happy.xml
                              ├── ic_emotion_hurt.xml
                              ├── ic_emotion_none.xml
                              ├── ic_emotion_sad.xml
                              ├── ic_heart.xml
                              ├── ic_info.xml
                              ├── ic_launcher_background.xml
                              ├── ic_launcher_foreground.xml
                              ├── ic_list.xml
                              ├── ic_logo.xml
                              ├── ic_microphone.xml
                              ├── ic_more.xml
                              ├── ic_palette.xml
                              ├── ic_pen.xml
                              ├── ic_photo.xml
                              ├── ic_recordmic.xml
                              ├── ic_search.xml
                              ├── ic_settings.xml
                              ├── ic_small_calendar.xml
                              ├── ic_status_done.xml
                              ├── ic_status_in_progress.xml
                              ├── ic_toggle_day_selected.xml
                              ├── ic_toggle_week_selected.xml
                              ├── ic_user.xml
                              ├── ic_wave_gray.xml
                              ├── ic_wave_green.xml
                              ├── main_button_selector.xml
                              ├── pencil_f.xml
                              ├── popup_background.xml
                              ├── purple_button.xml
                              ├── red_button.xml
                              ├── searchview_background.xml
                              ├── trash_f.xml
                              ├── white_button.xml
                              └── yellow_button.xml

                      └── layout
                              ├── activity_calendar.xml
                              ├── activity_calendar_item.xml
                              ├── activity_home.xml
                              ├── activity_home_popup.xml
                              ├── activity_home_search.xml
                              ├── activity_mini_calendar.xml
                              ├── activity_mini_calendar_item.xml
                              ├── activity_settings.xml
                              ├── activity_statistics.xml
                              ├── activity_voice_record.xml
                              ├── activity_writediary_home.xml
                              ├── activity_writingbutton.xml
                              ├── bottom_sheet_color.xml
                              ├── diary_item_popup.xml
                              └── item_diary_entry.xml

      
```

--- 

## 4. 역할 분담

### 🍊서연수

- **UI 설계 및 구현**
- **Google Cloud 연동**
- **AI 연결**

<br>
    
### 👻성시우

- **DB 설계 및 구축**
- **UI 구현**
- **AI 테스팅**


<br>

### 🐬박영빈

- **UI 개발 및 동적 구현**
- **DB 설계**
- **AI 모델 연결**


<br>

### 😎유두연

- **AI 테스팅 및 모듈 개발**
- **DB 설계**
    
--- 

## 5. 개발 기간 및 작업 관리

### 개발 기간

- 전체 개발 기간 : 2025-03-04 ~ 2025-05-30

<br>

### 작업 관리

- GitHub Projects와 Issues를 사용하여 진행 상황을 공유했습니다.
- 주간회의를 진행하며 작업 순서와 방향성에 대한 고민을 나누고 GitHub Wiki에 회의 내용을 기록했습니다.

--- 

## 6. 페이지별 기능

### [메인 화면 / 일기 화면]
- 해시태그 및 내용으로 작성한 일기를 확인합니다.
- 일기 확인을 통해 감정 분석의 결과를 확인할 수 있습니다.

<br>

| 메인 화면 |
|----------|
|<img src="https://github.com/user-attachments/assets/1ee0c4ef-2d30-445f-9a65-b3a7e261b855">|

<br>

### [감정분석 / 통계 및 피드백]
- 작성된 일기는 Llama를 통해 분석됩니다.
- 6가지 감정으로 통계를 제공하고, 그에 맞는 피드백을 함께 제공합니다.

<br>

| 통계 및 피드백 화면 |
|----------|
|<img src="https://github.com/user-attachments/assets/9e2bbef1-eba4-4d41-bd23-bfad81c88127">|

<br>

### [일기 작성]
- 음성 및 텍스트 타이핑 원하는 방식으로 일기를 작성할 수 있습니다.
- 하루를 대표하는 사진 1장을 입력할 수 있습니다.
- 일기의 분위기에 맞춰 원하는 배경색을 선택할 수 있습니다.

<br>

| 일기 작성 화면 |
|----------|
|<img src="https://github.com/user-attachments/assets/2d359999-63c0-4a60-b8a3-e0ba6ea5ba2a">|

<br>

### [캘린더]
- 캘린더에서 감정을 한 눈에 확인할 수 있습니다.
- 원하는 날짜를 선택하면, 그 날의 하루를 되돌아 볼 수 있습니다.

<br>

| 캘린더 화면 |
|----------|
|<img src="https://github.com/user-attachments/assets/b5343058-8db4-447b-899a-db8854326fef">|

<br>

### [Google Drive에 백업]
- 온디바이스의 이점을 살리고 사용자의 프라이버시 보장을 위해, 백업을 선택적으로 제공합니다.
- 네트워크 연결 후 사용자가 동기화를 활성화한다면, Google로 로그인 후 Google Drive에 백업합니다.

<br>

| 백업 화면 |
|----------|
|<img src="https://github.com/user-attachments/assets/ed9289ae-bd84-4eb4-bf9d-322f8fc39a1e">|

--- 

## 7. 프로젝트 후기

### 🍊 서연수

깃헙을 통한 협업에 익숙해지는 것, 서로 감정 상하지 않고 무사히 마무리하는 것이 1차적인 목표였어서 항상 이 부분을 명심하면서 작업했습니다.
각자 페이지를 작업하고 합치는 과정에서 마주친 버그들이 몇 있었는데, 시간에 쫓기느라 해결하기에 급급해서 제대로 트러블슈팅 과정을 기록하지 못한 게 살짝 아쉬운 부분으로 남습니다. 그래도 2022년 한 해 동안 가장 치열하게 살았던 한 달인 것 같습니다. 조원들 모두에게 고생했다고 전하고 싶습니다🧡

<br>

### 👻 성시우

여러모로 많은 것들을 배울 수 있었던 한 달이었습니다. 혼자서는 할 수 없었던 일이라는 것을 너무 잘 알기에 팀원들에게 정말 감사하다는 말 전하고 싶습니다. 개인적으로 아쉬웠던 부분은 기한 내에 기능을 구현하는 데에만 집중하면서 트러블 슈팅이나 새로 배웠던 것들을 체계적으로 기록하지 못했다는 점입니다. 이렇게 느낀 바가 있으니 이후의 제가 잘 정리하면서 개발할 거라 믿습니다… 하하 다들 수고하셨습니다!!!!

<br>

### 🐬 박영빈

팀 프로젝트 시작에 앞서 초기 설정을 진행하며 체계적인 설계의 중요성을 느꼈습니다. 앞으로는 점점 더 체계적이고 효율적으로 프로젝트를 진행할 수 있도록 발전하고 싶습니다.
정규 수업 직후에 프로젝트를 진행하면서 배운 내용을 직접 구현하는 과정이 어색했지만 어떤 부분이 부족한지 알 수 있는 기회였습니다. 스스로 최대한 노력해보고 팀원들과 함께 해결해 나가면서 협업의 장점을 체감할 수 있었습니다. 하지만 빠르게 작업을 진행하면서 팀원들과 함께 해결한 이슈가 어떤 이슈이며 어떻게 해결했는지에 대해 자세히 작성하지 못한 것이 아쉽습니다.
’멋쟁이 사자처럼’이라는 같은 목표를 가진 집단에서 프로젝트에 함께할 수 있는 소중한 경험이었습니다. 함께 고생한 조원들 모두 고생하셨습니다! 앞으로도 화이팅해서 함께 목표를 이뤄가고 싶습니다.

<br>

### 😎 유두연

컨벤션을 정하는 것부터 Readme 파일 작성까지 전 과정을 진행하려니 처음 생각보다 많은 에너지를 썼어요. 좋은 의미로 많이 썼다기보다, 제 능력을 십분 발휘하지 못해서 아쉬움이 남는 쪽입니다. 개발한다고 개발만 해서는 안 된다는 것을 몸소 느껴보는 기간이었던 것 같습니다. 이번 기회로 프로젝트를 진행하면서, 제가 잘하는 점과 부족한 점을 확실하게 알고 가는 건 정말 좋습니다. 기술적인 부분에 있어서는 리액트의 컴포넌트화가 주는 장점을 알았습니다. 조금 느린 개발이 되었을지라도 코드 가독성 부분에 있어서 좋았고, 오류가 발생해도 전체가 아닌 오류가 난 컴포넌트와 근접한 컴포넌트만 살펴보면 수정할 수 있는 부분이 너무 편했습니다. 모두 고생 참 많으셨고 리팩토링을 통해 더 나은 프로젝트 완성까지 화이팅입니다.
