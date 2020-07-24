# **OUNCE 기술서**

## 목차

1. [프로젝트 소개](#프로젝트-소개)

2. [개발 담당 부분](#개발-담당-부분)

   2-1. [스플래시 & 로그인](#스플래시-&-로그인)

   2-2. [회원가입](#회원가입)

   2-3. [프로필 등록](#프로필-등록)

   2-4. [메인 화면](#메인-화면)

   2-5. [기록하기](#기록하기)

3. [후기 및 발전](#후기-및-발전)

---

## 프로젝트 소개

- 한 줄 소개 : 고양이 집사들을 위한 똑똑한 기록장

- 프로젝트 기간 : 2020.06.28 ~ 2020.07.18

- 팀 구성 (총 16명)

  - PM : 이예인

  - TI :최혜리, 최현정

  - Designer : 안유경, 안아경, 권리원

  - Android Developer : **강민구(본인)**, 이현우, 박주예

  - iOS Developer : 오준현, 박주연, 이윤진, 김호세

  - Server : 정효원, 최정균, 손예지

- [Android Github](https://github.com/We-are-Ounce/OUNCE_Android)

&nbsp;&nbsp;26TH SOPT APP JAM 프로젝트 중 하나인 OUNCE에 안드로이드 개발자로서 참여했습니다.\
OUNCE는 기존 고양이를 키우는 일명 ‘집사’들을 위한 캣푸드 메모 어플입니다.\
입맛이 까다로운 고양이들을 위해 집사들은 맛있게 잘 먹으면서도 건강한 제품을 찾게 됩니다.\
이 과정에서 구매한 캣푸드를 고양이가 잘 먹는지 안 먹는지를 기록하게 되는데, 이 부분이 아직도 메모장이나 직접 수기로 작성하는 한계가 있습니다.\
기록한 정보의 양이 많아질수록 메모장의 기능만으로는 한계가 오게 되며 (정렬, 가시성 등등) 이러한 고민에서 시작된 것이 바로 ‘ounce’입니다.

&nbsp;&nbsp;OUNCE는 먹여본 캣푸드를 빠르게 검색하여 한 페이지에서 간단하게 기록할 수 있고, 최신 순, 기호도 순, 총점 순으로 정렬하여 내가 기록한 캣푸드를 보다 직관적으로 보여줄 수 있으며, 다른 고양이를 팔로우하여 서로의 기록을 공유할 수 있습니다.\
또한 ‘기호성’을 기준으로 입맛이 비슷한 고양이들을 추천해 줄 수 있는 기능으로 인해 다른 고양이들과 소셜 네트워크를 넓힐 수 있습니다.

&nbsp;&nbsp;저는 이 프로젝트에 Android 리드 개발자로 참여해 3주 동안 팀원들과 협업하며 앱 개발을 했고, 같은 파트원들을 이끌어주는 리더십, GitFlow를 이용한 프로젝트 협업 등을 배웠으며 개인적인 개발 성장 또한 이루어낼 수 있었습니다.

---

## 개발 담당 부분

&nbsp;&nbsp;OUNCE 앱을 만들 때 담당한 부분으로는 로그인, 회원가입, 프로필 등록, 메인 화면, 기록하기 기능, Splash화면을 맡아서 담당해서 개발했습니다.\
리드 개발자로서 코드리뷰를 진행하고, 전체적인 Git관리도 했습니다. 다른 팀원들보다 많은 부분을 맡아 개발했으며, 이 과정에서 많은 삽질이 있었지만 담당했던 뷰와 기능은 전부 완성시켰고, 다른 팀원들의 부분까지 도와줄 수 있어서 3주 동안 진행했던 프로젝트에서 본인의 역할에 충실했다고 생각합니다.

> #### **눈으로 보이는 디자인에 신경 쓰다.**

&nbsp;&nbsp;이번 프로젝트에서 가장 신경 썼던 부분은 실제 사용자가 눈으로 보는 화면이었습니다.\
개발 코드 내부적으로 최적화 시키고, 여러 디자인 패턴들을 사용해 독립성, 확장성을 넓히는 방향의 개발도 중요하지만 실제 사용자 눈에 보이는 화면이 모든 것을 보여주기 때문에 이 부분에 있어서 더 신경을 썼습니다.\
디자이너가 만든 UI/UX를 최대한 충실히 따르기 위해 노력했으며 회원가입 및 프로필 등록 단계에서 ViewPager를 커스텀 해 다음 단계로 넘어갈 때마다 페이지가 자연스럽게 전환되는 효과를 만들었습니다.\
그리고 사용자가 입력하는 정보에 대해서 밑줄 색 변경, 알림 문구 등 작성한 방식, 길이에 따라서 실시간으로 적용되게 만들었으며, 메인 화면 부분도 최대한 iOS어플 같은 느낌을 살리기 위해 노력했습니다.

<p align="center"><img src="https://user-images.githubusercontent.com/55642709/88371652-6d115c00-cdcf-11ea-8466-6c29ab8d9e03.png">
<img src="https://user-images.githubusercontent.com/55642709/88371717-8b775780-cdcf-11ea-9952-8ab72d90b18d.png">
<img src="https://user-images.githubusercontent.com/55642709/88371767-9f22be00-cdcf-11ea-944d-0b0b7384e25f.png"></p>

---

### 스플래시 & 로그인

> #### **Lottie 사용으로 깔끔한 스플래시 화면**

Splash 화면은 Lottie를 사용했습니다.\
gif를 사용하면 아무래도 화면에 따라서 깨져서 보이기 때문에 좀 더 깔끔함과 부드러움을 가지고 있는 Lottie 파일을 적용했습니다.\
그리고 풀 스크린 효과를 통해 Splash에 집중할 수 있도록 구성했고, 마지막으로 Thread를 이용해 3초간 딜레이를 건 다음 로그인 화면으로 이동하게 됩니다.

```
class SplashActivity : AppCompatActivity() {

    val handler = Handler(Looper.getMainLooper())

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_splash)

        window.decorView.systemUiVisibility = (View.SYSTEM_UI_FLAG_IMMERSIVE
                // Set the content to appear under the system bars so that the
                // content doesn't resize when the system bars hide and show.
                or View.SYSTEM_UI_FLAG_LAYOUT_STABLE
                or View.SYSTEM_UI_FLAG_LAYOUT_HIDE_NAVIGATION
                or View.SYSTEM_UI_FLAG_LAYOUT_FULLSCREEN
                // Hide the nav bar and status bar
                or View.SYSTEM_UI_FLAG_HIDE_NAVIGATION
                or View.SYSTEM_UI_FLAG_FULLSCREEN)


        img_splash.setAnimation("splash.json")
        img_splash.playAnimation()


        val thread = Thread2()
        thread.start()
    }

    ...

}
```

<p align="center"><img src="https://user-images.githubusercontent.com/55642709/88373022-05104500-cdd2-11ea-85c2-dcdc078afb10.gif" width="50%"></p>
