# OAuth2 SCOPES 더 알아보기

[디스코드 OAuth2 문서](https://discord.com/developers/docs/topics/oauth2)

> 일부 기능은 사용자의 개인 정보 등 민감한 데이터를 다룰 수 있기 때문에, 권한 남용을 막기 위해 디스코드의 승인이 필요함.

> 아주 많이 대충 적어놨기 때문에 간단히 읽어보시고 더 궁금한게 있으면 스스로 인터넷에 찾아보시길

> 저기 적힌 말들은 다 알거라 가정하고 썼으니까 해석 따위는 기대하지 마시길

## activities
> ### activities.read:
> 사용자의 현재 활동 상태 읽기
>
> 지금은 사용 불가라고 합니다.
>> #### 활동 상태?
>> ![image](https://github.com/user-attachments/assets/175eeaab-4328-4d73-a276-ef0591bbacdb)
>>
>> 저렇게 게임 하는 중, Spotify 듣는 중, Twitch 방송 중 등을 말한다.
>
> ### activities.write:
> 봇이 사용자의 활동 상태를 정할 수 있게 해줌.
> 
> Discord 승인이 필요한 기능
>
> 얘도 지금은 사용 불가라고 합니다.
>
> ~~근데 왜 있는거야~~

## applications
> ### applications.builds.read:
> 앱이 사용자 애플리케이션의 빌드 데이터를 읽을 수 있게 해줌.
> ### applications.builds.upload:
> 앱이 사용자 애플리케이션용 빌드를 업로드하고 업데이트하도록 허용
>
> Discord의 승인이 필요한 기능
> ### applications.commands:
> 슬래시 명령어를 쓸 수 있게 해줌.
> 슬래시 명령어를 쓰는 봇은 필수인 SCOPE임.
> ### applications.commands.update:
> 앱이 Bearer 토큰을 사용하여 명령을 업데이트하도록 허용 - 클라이언트 자격 증명 인증만 가능해서 주로 서버 측에서 쓴다고 적혀있긴 한데, 무슨 기능인지는 잘 모르겠다.
>
> ~~어차피 우리같은 사람들은 쓸 일이 없는 기능이니 넘어가자~~
> ### applications.commands.permissions.update
> /ban 명령어는 관리자만 쓸 수 있게 해주는 등 명령어를 특정 역할만 사용할 수 있게 나눌 수 있음.
> ### applications.entitlements:
> 이 권한은 사용자의 애플리케이션에 대한 권한(예: 사용자가 구매한 콘텐츠나 혜택)을 읽을 수 있게 해준다고 적혀있다.
>
> 무슨 기능인지는 모르겠지만 우리는 아마 구매와 관련된 기능은 필요 없을것이니 그냥 넘어가자.
> ### applications.store.update:
> 앱이 사용자 애플리케이션의 스토어 데이터(SKU, 스토어 등록정보, 업적 등)를 읽고 업데이트할 수 있습니다.
>
> 도대체 스토어는 무엇일까?

## bot
> ### bot:
> 뭔지 알 필요 없음.
>
> 그냥 필수임.

## connections
> ### connections:
> /users/@me/connections가 연결된 타사 계정을 반환하도록 허용해줌

## dm
> ### dm_channels.read:
> 앱이 사용자의 DM 볼 수 있도록 허용해줌
>
> 사용자의 개인 DM을 볼 수 있게 해준다는거 자체가 당연히 디스코드의 승인이 있어야함.
> 
> ### gdm.join:
> 앱에서 사용자를 그룹 dm에 가입 시킬 수 있게 함.

## email
> ### email:
> 사용자의 이메일 정보를 조회할 수 있음
>
> ~~디스코드 승인 필요가 없는 것을 보니 이메일은 그닥 안 중요하나보다~~

## guilds
> ### guilds:
> /users/@me/guilds가 사용자의 모든 길드에 대한 기본 정보를 반환하도록 허용
> ### guilds.join:
> 사용자를 길드에 가입시키는 데 /guilds/{guild.id}/members/{user.id}를 사용할 수 있습니다 .
> ### guilds.members.read:
> /users/@me/guilds/{guild.id}/member 가 길드에서 사용자의 회원 정보를 반환하도록 허용

## identify
> ### identify:
> 사용자의 기본 정보(아이디, 사용자명, 아바타 등)에 대한 접근 권한을 제공함.

## messages
> ### messages.read:
> 로컬 rpc 서버 API 액세스의 경우 모든 클라이언트 채널에서 메시지를 읽을 수 있습니다(그렇지 않으면 앱이 만든 채널/길드로 제한됨).

## relationships
> ### relationships.read:
> 앱이 사용자의 친구 및 암시적 관계를 알 수 있도록 허용
>
> 디코 승인 필
>
> ~~뭔가 무서운 기능이다.~~

## role
> ### role_connections.write:
> 앱이 앱에 대한 사용자 연결 (유튜브, 트위치 등) 및 메타데이터(ID, 사용자 이름 등)를 업데이트할 수 있습니다.

## rpc
> ### rpc:
> 로컬 rpc 서버 엑세스를 통해 사용자의 로컬 Discord 클라이언트를 제어할 수 있습니다.
>
> 클라이언트 제어..? ㄷㄷㄷ
> 
> 디코 승인 필
> ### rpc.activities.write:
> 로컬 rpc 서버로 사용자 활동을 업데이트할 수 있음. (게임 중, 음악 듣는 중 등)
>
> Discord 승인이 필요합니다.
>
> ### rpc.notifications.read:
> 로컬 rpc 서버를 통해 사용자에게 푸시된 알림을 받을 수 있습니다
>
> 사용자의 알림을 접근하는 무서운;;;
>
> 당연히 디코 승인이 필요함
> 
> ### rpc.voice.read:
> 로컬 rpc 서버를 통해 사용자의 음성 설정을 읽고 음성 채널 접속, 음소거 등 음성 이벤트를 감지할 수 있음.
> 디스코드 승인 필
>
> ### rpc.voice.write:
> 로컬 rpc 서버를 통해 사용자의 음성 채팅 볼륨, 음소거 상태 등 음성 설정을 업데이트할 수 있음.
> 디코 승인 필

## voice
> ### voice:
> 앱이 음성방에 연결하고 음성방 멤버를 볼 수 있게 허용함.
>
> Discord 승인이 필요합니다.

## 웹후크
> ### webhook.incoming:
> OAuth2 인증 후 웹훅을 생성하고 이를 통해 Discord와 외부 시스템 간의 자동화된 메시지 전송을 가능하게 하는 권한임.
>
> 봇이 웹후크를 생성할 수 있음.
>
> 디스코드의 승인이 필요함.
