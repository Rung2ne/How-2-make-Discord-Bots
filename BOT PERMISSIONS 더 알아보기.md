# 주요 Bot Permissions

Discord 봇의 권한은 서버 내에서 봇이 수행할 수 있는 작업을 정의합니다. 아래는 권한 목록과 간단한 설명입니다.

---

## 📜 General Permissions

| **Permission**                  | **Description**                                                                                     |
|----------------------------------|-----------------------------------------------------------------------------------------------------|
| **Administrator**               | 서버 내 모든 권한을 무제한적으로 부여합니다.                                                        |
| **View Audit Log**              | 서버 활동 로그를 조회할 수 있습니다.                                                                |
| **Manage Server**               | 서버 설정을 변경하거나 관리할 수 있습니다.                                                          |
| **Manage Roles**                | 서버 내 역할(권한 포함)을 생성, 수정 및 삭제할 수 있습니다.                                           |
| **Manage Channels**             | 채널 생성, 수정 및 삭제 권한을 제공합니다.                                                          |
| **Kick Members**                | 멤버를 서버에서 추방할 수 있습니다.                                                                 |
| **Ban Members**                 | 멤버를 서버에서 차단할 수 있습니다.                                                                 |
| **Create Instant Invite**       | 서버 초대 링크를 생성할 수 있습니다.                                                                |
| **Change Nickname**             | 자신의 닉네임을 변경할 수 있습니다.                                                                 |
| **Manage Nicknames**            | 다른 사용자의 닉네임을 변경할 수 있습니다.                                                          |
| **Manage Expressions**          | 서버의 커스텀 이모지 및 스티커를 관리할 수 있습니다.                                                |
| **Create Expressions**          | 새로운 이모지나 스티커를 생성할 수 있습니다.                                                        |
| **Manage Webhooks**             | 웹훅을 생성, 수정 및 삭제할 수 있습니다.                                                            |
| **View Channels**               | 서버의 텍스트 및 음성 채널을 조회할 수 있습니다.                                                    |
| **Manage Events**               | 서버 이벤트를 관리할 수 있습니다.                                                                   |
| **Create Events**               | 새로운 서버 이벤트를 생성할 수 있습니다.                                                            |
| **Moderate Members**            | 멤버를 음소거하거나, 제한할 수 있습니다.                                                            |
| **View Server Insights**        | 서버 통계를 조회할 수 있습니다.                                                                    |
| **View Server Subscription Insights** | 서버 구독 정보를 조회할 수 있습니다.                                                              |

---

## ✉️ Text Permissions

| **Permission**                  | **Description**                                                                                     |
|----------------------------------|-----------------------------------------------------------------------------------------------------|
| **Send Messages**               | 텍스트 채널에서 메시지를 보낼 수 있습니다.                                                           |
| **Create Public Threads**       | 공개 스레드를 생성할 수 있습니다.                                                                   |
| **Create Private Threads**      | 비공개 스레드를 생성할 수 있습니다.                                                                 |
| **Send Messages in Threads**    | 스레드 내에서 메시지를 보낼 수 있습니다.                                                             |
| **Send TTS Messages**           | TTS(텍스트 음성 변환) 메시지를 보낼 수 있습니다.                                                     |
| **Manage Messages**             | 모든 메시지를 삭제하거나 관리할 수 있습니다.                                                        |
| **Manage Threads**              | 스레드를 수정하거나 삭제할 수 있습니다.                                                             |
| **Embed Links**                 | 링크 미리보기를 포함하는 메시지를 보낼 수 있습니다.                                                  |
| **Attach Files**                | 파일을 업로드할 수 있습니다.                                                                        |
| **Read Message History**        | 이전에 보낸 메시지 기록을 읽을 수 있습니다.                                                         |
| **Mention Everyone**            | `@everyone` 또는 `@here` 멘션을 사용할 수 있습니다.                                                 |
| **Use External Emojis**         | 서버 외부의 이모지를 사용할 수 있습니다.                                                            |
| **Use External Stickers**       | 서버 외부의 스티커를 사용할 수 있습니다.                                                            |
| **Add Reactions**               | 메시지에 반응(이모지)을 추가할 수 있습니다.                                                        |
| **Use Slash Commands**          | 슬래시 명령어를 사용할 수 있습니다.                                                                |
| **Use Embedded Activities**     | 내장된 Discord 활동(예: 게임 등)을 사용할 수 있습니다.                                              |
| **Use External Apps**           | 외부 애플리케이션을 연동하여 사용할 수 있습니다.                                                    |
| **Create Polls**                | 투표를 생성할 수 있습니다.                                                                          |

---

## 🔊 Voice Permissions

| **Permission**                  | **Description**                                                                                     |
|----------------------------------|-----------------------------------------------------------------------------------------------------|
| **Connect**                     | 음성 채널에 연결할 수 있습니다.                                                                     |
| **Speak**                       | 음성 채널에서 대화할 수 있습니다.                                                                   |
| **Video**                       | 음성 채널에서 비디오를 사용할 수 있습니다.                                                         |
| **Mute Members**                | 다른 멤버의 음성을 음소거할 수 있습니다.                                                            |
| **Deafen Members**              | 다른 멤버의 소리를 듣지 못하게 설정할 수 있습니다.                                                  |
| **Move Members**                | 음성 채널의 멤버를 다른 채널로 이동시킬 수 있습니다.                                                |
| **Use Voice Activity**          | 음성 활성화를 기반으로 말할 수 있습니다(푸시 투 토크 불필요).                                       |
| **Priority Speaker**            | 우선 발언자로 설정되어 다른 사용자의 볼륨이 감소합니다.                                              |
| **Request To Speak**            | 음성 채널에서 발언 요청을 할 수 있습니다.                                                           |
| **Use Embedded Activities**     | 음성 채널에서 내장된 Discord 활동을 사용할 수 있습니다.                                             |
| **Use Soundboard**              | 음성 채널에서 사운드보드 기능을 사용할 수 있습니다.                                                 |
| **Use External Sounds**         | 외부 사운드를 사용할 수 있습니다.                                                                   |

---

**참고:** Discord 개발자 포털에서 필요한 권한을 선택하면 자동으로 계산된 URL을 제공합니다.
