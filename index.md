---
layout: default
title: 리도 개인정보처리방침 / Rido Privacy Policy
---

<div align="right">
<a href="#english">English</a>
</div>

# 리도 개인정보처리방침

**시행일: 2026년 8월 22일**

리도(이하 "앱")는 사용자가 올린 사진을 바탕으로 배달·쇼핑 후기 초안을 만들어 주는 앱입니다. 이 방침은 앱이 어떤 정보를 다루고, 어디로 보내고, 얼마나 두는지를 적은 것입니다.

---

## 1. 앱이 수집하지 않는 것

먼저 수집하지 **않는** 것을 밝힙니다.

- 회원가입이 없습니다. 이름, 이메일, 전화번호, 생년월일을 받지 않습니다.
- 로그인이 없습니다. 계정을 만들지 않습니다.
- 사용자가 만든 후기 글을 개발자가 볼 수 있는 곳으로 보내지 않습니다.
- 연락처, 통화기록, 문자메시지에 접근하지 않습니다.

---

## 2. 앱이 다루는 정보

### 2-1. 사진

| 항목 | 내용 |
|---|---|
| 무엇 | 사용자가 직접 고르거나 찍은 사진, 그 사진의 촬영 시각(EXIF) |
| 왜 | 후기 초안을 만들기 위해 |
| 어디로 | Google Gemini API로 전송 |
| 얼마나 | 앱은 전송한 사진을 서버에 보관하지 않음 |

**앱은 사진 접근 권한을 요청하지 않습니다.** 안드로이드의 시스템 사진 선택 도구를
쓰기 때문에, 사용자가 그 화면에서 고른 사진만 앱으로 넘어옵니다. 나머지 사진은
앱이 볼 수 없습니다.

시스템 선택 도구는 사진의 위치 태그를 지우고 넘겨주는 것이 기본입니다. 그래서
앱은 대개 사진의 좌표를 알지 못하고, 장소는 사용자가 직접 적거나 지도 검색으로
고릅니다. 좌표가 남아 있는 사진이라면 그 좌표만 지명 변환 서비스로 보냅니다.

### 2-2. 사용자가 직접 입력한 내용

만족도 선택, 좋았던 점, 아쉬웠던 점, 장소 이름. 후기 문장을 만드는 데만 쓰이며, 만들어진 글과 함께 **기기 안에만** 저장됩니다.

### 2-3. 기기에만 저장되고 밖으로 나가지 않는 것

- 저장한 후기 글과 그 사진 사본
- 남은 생성 횟수와 하루 무료 사용 횟수
- 앱 설정

이 값들은 기기의 앱 저장 공간에 있고, **앱을 지우면 함께 지워집니다.** 개발자를 포함해 아무도 외부에서 볼 수 없습니다.

친구 초대를 쓰는 경우에만 예외가 하나 있습니다. 초대 코드와 아직 받아 가지 않은 보상 수는 아래 3-4에 적은 서버에도 함께 있습니다.

---

## 3. 정보를 넘기는 곳

### 3-1. Google (Gemini API)

- **넘기는 것**: 사용자가 고른 사진, 사용자가 적은 내용, 장소 이름
- **왜**: 후기 문장을 만들기 위해
- **처리 방침**: Google의 [Gemini API 약관](https://ai.google.dev/gemini-api/terms)과 [Google 개인정보처리방침](https://policies.google.com/privacy)을 따릅니다.

앱은 Gemini API의 **유료 등급**을 사용합니다. 이는 다음을 뜻합니다.

- 전송된 사진과 입력 내용은 **Google의 모델 개선에 사용되지 않습니다.**
- 사람이 내용을 읽고 검토하지 않습니다.
- 다만 Google은 금지된 사용을 탐지하고 서비스 안전을 지키기 위해, 그리고 법적 의무 이행을 위해 요청과 응답을 **제한된 기간 동안** 보관합니다.

무료 등급에서는 전송 내용이 모델 개선에 쓰이고 사람이 검토할 수 있으나, 앱은 그 등급을 쓰지 않습니다.

### 3-2. 위치를 지명으로 바꾸는 서비스

사용자가 지도에서 장소를 검색할 때, 그리고 사진에 좌표가 남아 있는 드문 경우에만
그 좌표나 검색어만 보냅니다. 사진이나 후기 내용은 보내지 않습니다.

- OpenStreetMap Nominatim ([방침](https://osmfoundation.org/wiki/Privacy_Policy))
- 카카오 로컬 API ([방침](https://www.kakao.com/policy/privacy))

### 3-3. Google AdMob (광고)

앱은 광고를 보여 줍니다. AdMob은 광고 식별자(AAID) 등을 이용해 맞춤 광고를 제공할 수 있습니다.

광고가 나오는 곳은 두 군데입니다.

- 후기를 만드는 동안과 결과를 보는 화면
- 사용자가 **직접 버튼을 눌러** 광고를 보고 생성 횟수를 받는 경우

참고 링크와 설정 방법입니다.

- [Google 광고 정책](https://policies.google.com/technologies/ads)
- 맞춤 광고는 **기기 설정 → Google → 광고**에서 끌 수 있습니다.

### 3-4. 친구 초대 서버

**친구 초대 기능을 쓸 때만 동작합니다.** 초대한 사람에게 생성 횟수를 주려면 그 사람의 **다른 기기에 있는 값을 올려야** 하는데, 기기 안에만 저장하는 구조로는 방법이 없습니다. 그래서 이 기능 하나만 앱 밖의 서버를 씁니다.

| 항목 | 내용 |
|---|---|
| 무엇 | 앱이 만든 무작위 값 1개, 초대 코드 6자리, 아직 받아 가지 않은 보상 수 |
| 어디로 | Supabase — 개발자가 운영하는 데이터베이스 |
| 왜 | 초대한 사람과 초대받은 사람에게 생성 횟수를 주기 위해 |
| 언제 | 앱을 열 때, 그리고 초대 코드를 입력할 때 |

**보내지 않는 것**: 사진, 만들어진 후기 글, 입력한 내용, 이름·이메일·전화번호, 광고 ID, 기기 식별자(ANDROID_ID 등).

무작위 값은 **앱이 스스로 만들어 낸 숫자**입니다. 기기에서 읽어 온 값이 아니라서 다른 앱이나 서비스의 기록과 이어 붙일 수 없고, 앱을 지우면 끊어집니다.

---

## 4. 사진 속 개인정보를 다루는 방식

주문 화면이나 영수증에는 주소, 전화번호, 카드번호, 주문번호가 함께 찍히는 일이 많습니다.

앱은 후기 문장을 만들 때 **그런 정보를 옮겨 적지 않도록** 모델에 지시하고 있습니다. 다만 이는 완벽하지 않습니다. 만들어진 글은 붙여넣기 전에 반드시 확인해 주시고, 가능하면 **사진을 올리기 전에 개인정보 부분을 가려 주세요.**

---

## 5. 보관 기간

| 대상 | 기간 |
|---|---|
| 기기에 저장된 후기와 사진 | 사용자가 지울 때까지. 최근 100편을 넘으면 오래된 것부터 자동 삭제 |
| 앱 설정과 생성 횟수 | 앱을 삭제할 때까지 |
| 초대 서버의 코드와 보상 기록 | 삭제를 요청하실 때까지 |
| Google·지도 서비스로 전송된 내용 | 각 사업자의 방침에 따름 |

---

## 6. 사용자의 권리

- **저장한 후기 삭제**: 앱의 보관함에서 개별 삭제
- **전체 삭제**: 앱을 삭제하면 기기에 저장된 모든 정보가 함께 지워집니다
- **사진 접근**: 앱이 요청하는 사진 권한이 없어 철회할 것도 없습니다.
  사진은 고를 때마다 시스템 선택 화면에서 그때 고른 것만 넘어갑니다
- **맞춤 광고 끄기**: 안드로이드 설정 → Google → 광고
- **초대 기록 삭제**: 설정 → 친구 초대에 보이는 **내 초대 코드**를 아래 문의 주소로 보내 주시면 해당 기록을 지웁니다

앱을 지우면 기기 안의 정보는 전부 사라집니다. 다만 **친구 초대를 쓰셨다면 초대 코드와 보상 기록은 서버에 남습니다** — 앱이 지워진 것을 서버가 알 방법이 없기 때문입니다. 위 방법으로 요청해 주시면 지웁니다.

그 밖에는 회원가입이 없어 개발자가 보관하는 개인정보가 없으므로, 별도의 열람·정정 요청 절차를 두지 않습니다.

---

## 7. 만 14세 미만 아동

앱은 만 14세 미만 아동을 대상으로 하지 않으며, 아동의 개인정보를 알면서 수집하지 않습니다.

---

## 8. 방침 변경

내용이 바뀌면 앱 안의 설정 화면과 이 문서에서 알립니다. 중요한 변경은 시행 7일 전에 알립니다.

---

## 9. 문의

- 이메일: wnsgud875@gmail.com

---

---

# Rido Privacy Policy {#english}

**Effective: August 22, 2026**

Rido ("the app") writes review drafts for delivery orders and shopping from photos you
choose. This policy sets out what the app handles, where it goes, and how long it stays.

---

## 1. What the app does not collect

First, what it does **not** take.

- There is no sign-up. No name, email, phone number, or date of birth.
- There is no login. No account is created.
- The reviews you write are never sent anywhere the developer can see them.
- The app does not touch your contacts, call log, or messages.

---

## 2. What the app handles

### 2-1. Photos

| | |
|---|---|
| What | Photos you pick or take, and the time they were taken (EXIF) |
| Why | To write the review draft |
| Where | Sent to the Google Gemini API |
| How long | The app does not keep them on any server |

**The app does not ask for photo permission.** It uses Android's system photo picker, so
only the photos you select on that screen come through. The app cannot see the rest.

The system picker strips location tags by default. So the app usually does not know where
a photo was taken, and you either type the place yourself or search the map. In the rare
case a photo still carries coordinates, only those coordinates go to a place-name service.

### 2-2. What you type

Your rating, what you liked, what disappointed you, and the place name. These are used
only to write the review, and are stored **on your device only** along with the result.

### 2-3. What stays on your device and never leaves

- Saved reviews and copies of their photos
- Remaining writes and your daily free count
- App settings

These live in the app's storage on your device and **are deleted when you uninstall the
app.** Nobody, including the developer, can see them from outside.

There is one exception, and only if you use the invite feature: your invite code and any
uncollected reward also live on the server described in 3-4 below.

---

## 3. Who the app sends things to

### 3-1. Google (Gemini API)

- **Sent**: the photos you picked, what you wrote, the place name
- **Why**: to write the review
- **Their terms**: Google's [Gemini API terms](https://ai.google.dev/gemini-api/terms)
  and [Google Privacy Policy](https://policies.google.com/privacy)

The app uses the **paid tier** of the Gemini API. That means:

- What you send is **not used to improve Google's models.**
- No human reviews the content.
- Google does retain requests and responses for a **limited period** to detect prohibited
  use, keep the service safe, and meet legal obligations.

On the free tier, what you send would be used for model improvement and could be reviewed
by a person. The app does not use that tier.

### 3-2. Place-name services

Only when you search for a place on the map, and in the rare case a photo still carries
coordinates. Only the coordinates or the search term go out. Never your photos or your
review.

- OpenStreetMap Nominatim ([policy](https://osmfoundation.org/wiki/Privacy_Policy))
- Kakao Local API ([policy](https://www.kakao.com/policy/privacy))

### 3-3. Google AdMob (ads)

The app shows ads. AdMob may use an advertising identifier (AAID) and similar signals to
serve personalized ads.

Ads appear in two places:

- While the review is being written, and on the result screen
- When you **tap a button yourself** to watch an ad in exchange for more writes

References and how to turn it off:

- [Google advertising policies](https://policies.google.com/technologies/ads)
- Personalized ads can be turned off in **device Settings → Google → Ads**.

### 3-4. Invite server

**Only active if you use the invite feature.** To give someone credits for inviting a friend, we have to change a value on *their* device — and there is no way to do that from data kept only on your phone. This one feature is why the app talks to a server at all.

| | |
|---|---|
| What | One random value the app generates, a 6-character invite code, and any reward not yet collected |
| Where | Supabase — a database the developer runs |
| Why | To credit both the person who invited and the person who joined |
| When | When you open the app, and when you enter an invite code |

**Not sent**: photos, generated reviews, anything you typed, your name, email, phone number, advertising ID, or device identifiers such as ANDROID_ID.

The random value is **made up by the app itself**. It is not read from the device, so it cannot be linked to records held by other apps or services, and it is gone once you uninstall.

---

## 4. Personal details inside your photos

Order screens and receipts often carry an address, phone number, card number, or order
number in the same frame.

The app instructs the model **not to copy those into the review.** This is not perfect.
Please read the result before you paste it anywhere, and where you can, **cover the
personal parts before adding the photo.**

---

## 5. Retention

| What | How long |
|---|---|
| Reviews and photos on your device | Until you delete them. Past 100 reviews, the oldest are removed automatically |
| Settings and remaining writes | Until you uninstall the app |
| Invite code and reward record on the server | Until you ask us to delete it |
| What was sent to Google and map services | Per each provider's own policy |

---

## 6. Your rights

- **Delete a saved review**: remove it individually from the app's library
- **Delete everything**: uninstalling the app removes everything stored on your device
- **Photo access**: the app requests no photo permission, so there is nothing to revoke.
  Each time, only what you pick on the system picker is handed over
- **Turn off personalized ads**: Android Settings → Google → Ads
- **Delete your invite record**: send the **invite code** shown under Settings → Invite
  friends to the contact address below, and we will delete that record

Uninstalling removes everything held on your device. However, **if you used the invite
feature, your invite code and reward record stay on the server** — the server has no way
to know the app was removed. Ask us using the method above and we will delete it.

Otherwise there is no sign-up, so the developer holds no personal data about you, and
there is no separate procedure for access or correction requests.

---

## 7. Children under 14

The app is not directed at children under 14 and does not knowingly collect their
personal information.

---

## 8. Changes to this policy

If this changes, it will be announced in the app's settings screen and in this document.
Significant changes are announced 7 days before they take effect.

---

## 9. Contact

- Email: wnsgud875@gmail.com

---
