# pueding:accounts-naver

```
meteor add pueding:accounts-naver
```

Meteor에서 Naver login 을 지원하기 위한 패키지 입니다.

[https://github.com/acidsound/meteor-accounts-naver](https://github.com/acidsound/meteor-accounts-naver) 패키지를 다음과 같은 이유로 수정하였습니다.

* 회원 프로필 조회 API를 XML 방식에서 JSON으로 변경
* 회원의 unique id만 가져오던 기존 방식에서, profile 전체를 저장하도록 변경(주의! 네이버
'내 애플리케이션'에서 '이메일', '회원이름' 추가권한을 꼭 지정해줘야 합니다. 그렇지 않으면 나머지 값들만 저장이 됩니다.)
  * id - 유니크 값
  * nickname - 사용자 별명
  * name - 사용자 이름
  * email - 사용자 메일 주소
  * gender - 성별
  * age - 사용자 연령대
  * birthday - 사용자 생일
  * profile_image - 사용자 프로필 사진 URL



사용자 프로필 관련 자세한 내용은 [https://developers.naver.com/docs/login/profile/](https://developers.naver.com/docs/login/profile/) 을 참고 부탁드립니다.
