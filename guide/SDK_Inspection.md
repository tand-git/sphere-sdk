# Sphere SDK 연동 검증 가이드

## SDK 연동 검증하기

> SDK 기본 연동이 완료되었다면 SDK 로그 확인 및 Sphere Analytics 콘솔 SDK 검증 화면에서 연동 검증이 가능합니다.

### Sphere Analytics 콘솔을 통한 검증

[Notion 연동검증가이드](https://lightning-individual-9c1.notion.site/0ad122054a0d44e59166a90a3c48e8e2)를 참조하여,
Sphere Analtyics 콘솔에서 로그인 후 [SDK 연동 및 검증](https://analytics.tand.kr/account/inspector) 화면에서 가장 최근에 수집된 이벤트 및 세션 정보를 확인할 수 있습니다.

### SDK 로그를 통한 검증

SDK 로그를 확인하기 위해서는 아래 해당하는 플랫폼의 SDK 연동 가이드 내용에 따라 SDK 로그 출력을 활성화합니다.

* [Web SDK 연동 가이드 - 로그 출력](https://github.com/tand-git/web-sdk#로그-출력)
* [Android SDK 연동 가이드 - 로그 출력](https://github.com/tand-git/android-sdk#로그-출력)
* [iOS SDK 연동 가이드 - 로그 출력](https://github.com/tand-git/ios-sdk#로그-출력)


로그가 활성화 되었다면 다음과 같이 정상적으로 로그가 출력이 됩니다.  
만약 정상적으로 연동이 되지 않은 경우 로그가 출력이 되지 않거나 에러 로그를 출력합니다.

(1) 앱 실행 시

```text
Sphere Android SDK version 1.x.x
```

(2) 앱 종료 시

```text
Finished to upload events.
```

(3) 이벤트 기록 시

```text
Log event. Event name: xxxxx
```

(4) 사용자 속성 기록 시

```text
Set user property. [속성명] : [속성값]
```


