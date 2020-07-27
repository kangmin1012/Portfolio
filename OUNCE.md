# **OUNCE 기술서**

## 목차

1. [프로젝트 소개](#1-프로젝트-소개)

2. [개발 담당 부분](#2-개발-담당-부분)

   2-1. [스플래시 & 로그인](#2-1-스플래시--로그인)

   2-2. [회원가입](#2-2-회원가입)

   2-3. [프로필 등록](#2-3-프로필-등록)

   2-4. [메인 화면](#2-4-메인-화면)

   2-5. [다른 고양이 프로필](#2-5-다른-고양이-프로필)

   2-6. [리뷰 수정,삭제](#2-6-리뷰-수정삭제)

3. [후기 및 발전](#3-후기-및-발전)

---

## 1. 프로젝트 소개

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

## 2. 개발 담당 부분

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

### 2-1. 스플래시 & 로그인

> #### **Lottie 사용으로 깔끔한 스플래시 화면**

&nbsp;&nbsp;Splash 화면은 Lottie를 사용했습니다.\
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

<p align="center"><img src="https://user-images.githubusercontent.com/55642709/88373022-05104500-cdd2-11ea-85c2-dcdc078afb10.gif" width="30%"></p>

> #### **아이디 비밀번호 입력에 따른 버튼 활성화 및 알림 문구**

&nbsp;&nbsp;로그인 화면에서 가장 신경 쓴 것은 사용자가 아이디 비밀번호를 입력하는 것에 따라서 로그인 버튼을 활성화 시키는 부분이었습니다.\
아이디 패스워드 EditTextView에 텍스트의 변화를 감지하는 리스너를 달고, 두 곳 다 빈칸이 아니라면 로그인 버튼을 활성화 시켰습니다.\
여기서 텍스트 변화를 감지하는 리스너는 코틀린의 확장함수를 통해 구현했고, 회원가입, 프로필 등록 화면에서도 계속해서 사용했습니다.

_textCheckListener 확장 함수_

```
fun EditText.textCheckListener(textCheck: (CharSequence?) -> Unit) {
    this.addTextChangedListener(object : TextWatcher {
        override fun afterTextChanged(s: Editable?) {
        }

        override fun beforeTextChanged(
            s: CharSequence?,
            start: Int,
            count: Int,
            after: Int
        ) = Unit

        override fun onTextChanged(
            s: CharSequence?,
            start: Int,
            before: Int,
            count: Int
        ) {
            textCheck(s)
        }
    })
}
```

_로그인 버튼 활성화 및 잘못 입력했을 때 반응_

<p align="center"><img src="https://user-images.githubusercontent.com/55642709/88380182-07c56700-cddf-11ea-92dd-ec51af66a3d3.PNG" width="30%">
<img src="https://user-images.githubusercontent.com/55642709/88380234-23c90880-cddf-11ea-8d76-e57df639e5ab.PNG" width="30%"></p>

> #### **Ted Park님의 EditText 커스텀을 이용한 글씨 감지**

&nbsp;&nbsp;EditText는 기존 안드로이드에서 제공해주는 뷰가 아니라 Ted Park님께서 커스텀 하신 EditText를 참고하여 사용하였습니다.\
그 이유는 뷰에 글씨가 감지 되었을 때 우측에 x표시가 뜨고, 그 버튼을 누르면 전체 내용이 지워지는 기능이 필요한데 해당 코드가 이에 부합하다고 생각했기 때문입니다.

- [_ClearEditText.kt_](https://github.com/We-are-Ounce/OUNCE_Android/blob/master/app/src/main/java/com/sopt/ounce/util/ClearEditText.kt)

---

### 2-2. 회원가입

> #### **뷰페이저를 커스텀하여 애니메이션 대체**

&nbsp;&nbsp;회원가입과 프로필 화면은 둘 다 단계별로 사용자에게 정보를 입력받습니다.  
단계별로 입력을 받기 때문에 다음 단계로 넘어갈 때 화면의 자연스러움을 주기 위해서 애니메이션을 먼저 떠올렸습니다.  
각각의 단계를 프래그먼트로 만들어 애니메이션을 적용시켜 줄 수도 있었으나, 뷰페이저가 떠오르게 되었고, 좀 더 자연스러운 애니메이션을 제공해준다고 생각하여 뷰페이저를 사용하게 되었습니다.

&nbsp;&nbsp;정보 입력 시 다음 단계로 넘어갈 때의 조건은 다음과 같습니다.

- 모든 항목을 입력 전 까지는 이동 할 수 없다.
- 뷰페이저가 스와이프 돼서는 안된다.
- 인디케이터를 눌러도 이동 되면 안된다.

해당 조건을 만족시키기 위해서 뷰페이저를 직접 커스텀하였고, 애니메이션 이동 속도가 너무 빨라서 페이지가 변경되는 애니메이션 속도를 조절하였습니다.

- [_스와이프 되지 않는 뷰페이저_](https://github.com/We-are-Ounce/OUNCE_Android/blob/master/app/src/main/java/com/sopt/ounce/util/NoSwipeViewPager.kt)

- [_뷰페이저 이동속도 조절하는 코드_](https://github.com/We-are-Ounce/OUNCE_Android/blob/master/app/src/main/java/com/sopt/ounce/util/FixedSpeedScroller.kt)

각 단계별로 모든 항목을 입력 할 때 까지 다음으로 이동할 수 없기 때문에, 로그인 버튼과 마찬가지로  
EditText에 checkListener를 추가해 전부 다 작성했는지 판단하여 버튼을 활성화 하도록 만들었습니다.  
이 때 '다음' 버튼은 activity 상에 존재하고 있고, EditText는 프래그먼트에 존재하기 때문에  
프래그먼트에서 액티비티에 접근하여 '다음'버튼을 활성화 시켰습니다.

_프래그먼트 내 액티비티 접근 함수_

```
 private fun checkCode() {
        if (mCode == v.edt_email_number.text.toString().toInt()) {
            v.txt_email_failcheck.text = "인증이 완료되었습니다."
            v.txt_email_failcheck.visibility = View.VISIBLE
            "UserInfoCheck".showLog(mEmail)
            UserInfoObject.email = mEmail
            "UserInfoCheck".showLog("${UserInfoObject.email}")
            mActivity.buttonEnable(true)
        }

        ...
 }
```

_액티비티에 있는 buttonEnable() 함수_

```
//확인 버튼 클릭 활성화
@Suppress("DEPRECATION")
fun buttonEnable(enable: Boolean) {
    if (enable) {
        btn_signup_ok.apply {
            isEnabled = true
            setTextColor(resources.getColor(R.color.white))
        }
    } else {
        btn_signup_ok.apply {
            isEnabled = false
            setTextColor(resources.getColor(R.color.greyish_two))
        }
    }

}
```

<p align="center"><img src="https://user-images.githubusercontent.com/55642709/88384043-a43f3780-cde6-11ea-8dad-2dcc49970435.gif" width="30%"></p>

> #### **6자리 난수를 이용한 이메일 인증**

&nbsp;&nbsp;회원가입에서 이메일을 인증하는 부분이 있습니다.  
6자리 난수를 생성해 이메일 주소와 함께 서버에 보내면, 서버에서 해당 이메일로 난수를 그대로 보내줍니다.  
그러면 사용자는 메일을 보고 6자리 숫자를 입력하는데,  
내부적으로 해당 6자리 숫자를 가지고 있다가 사용자가 입력하는 숫자와 대입해 같을 경우  
다음 단계로 넘어갈 수 있게 활성화 시켰습니다.

_서버통신으로 이메일에 인증코드를 보내는 함수_

```
    // 이메일에 인증번호를 보내는 버튼 누를 때 호출
    private fun checkEmail() {
        mEmail = v.edt_email.text.toString()

        //6자리 난수 생성
        mCode = (100000..999999).random()
        v.txt_email_failsend.text = "인증번호를 발송했습니다."
        v.txt_email_failsend.visibility = View.VISIBLE

        val request = EmailCheckServiceImpl
        request.service.postEmail(
            RequestEmailData(
                v.edt_email.text.toString(),
                "OUNCE 회원가입 인증해주세요.",
                "인증번호를 입력해주세요 : $mCode"
            )
        ).customEnqueue(
            onSuccess = {
                "MailSuccess".showLog("${it.message}")

            }
        )

    }
```

_사용자가 인증번호를 입력해서 맞는지 비교하는 함수_

```
    // 이메일에서 받은 인증코드를 입력하는 버튼 누를 때 호출
    private fun checkCode() {
        if (mCode == v.edt_email_number.text.toString().toInt()) {
            v.txt_email_failcheck.text = "인증이 완료되었습니다."
            v.txt_email_failcheck.visibility = View.VISIBLE
            "UserInfoCheck".showLog(mEmail)
            UserInfoObject.email = mEmail
            "UserInfoCheck".showLog("${UserInfoObject.email}")
            mActivity.buttonEnable(true)
        }
        else {
            v.edt_email_number.background.setColorFilter(
                resources.getColor(R.color.dark_peach),
                PorterDuff.Mode.SRC_IN
            )
            v.txt_email_failcheck.text = "인증번호가 틀렸습니다."
            v.txt_email_failcheck.visibility = View.VISIBLE
        }
    }
```

_Retrofit2 서버통신 확장 함수_

```
fun <ResponseType> Call<ResponseType>.customEnqueue(
    onFaile: () -> Unit = { "OunceServerStatus".showLog("통신 실패") },
    onSuccess: (ResponseType) -> Unit,
    onError: (Response<ResponseType>) -> Unit = {}
) {
    this.enqueue(object : Callback<ResponseType> {
        override fun onFailure(call: Call<ResponseType>, t: Throwable) {
            "OunceServerStatus".showLog("ServerFail : ${t.message}")
            onFaile()
        }

        override fun onResponse(call: Call<ResponseType>, response: Response<ResponseType>) {
            response.takeIf { it.isSuccessful }
                ?.body()
                ?.let{
                    onSuccess(it)
                } ?: onError(response)
        }
    })
}
```

### 2-3. 프로필 등록

#### **프로필 이미지 서버 업로드 MultipartBody.Part 이용**

&nbsp;&nbsp;앱에서 회원가입을 하게 되면 본인이 키우고 있는 고양이 프로필을 등록 하게 됩니다.  
고양이의 정보를 입력 받는 것은 크게 어렵지 않았으나, 가장 큰 문제는 이미지를 서버에 업로드 하는 일이었습니다.  
지금까지 서버에서 주는 url을 `Glide`로 이용해 처리하기만 했는데  
이번에는 내 로컬에 있는 이미지를 가져와 서버에 업로드해야 했기 때문에 새로운 시도였습니다.  
한 번도 해본 적 없는 작업이었기에 구글링을 통해 공부했고, `MultipartBody.Part`를 이용하면 가능하다는 것을 배웠습니다.  
먼저 interface에 `@Multipart` 어노테이션을 지정해주고, 이미지는 `MultipartBody.Part` 타입으로, 나머지 고양이 정보는 `HashMap` 타입으로 request를 보냈습니다.

_Multipart를 이용한 서버 통신 인터페이스_

```
@Multipart
@POST("profile/register")
fun postCatProfile(
    @Header("token") token: String,
    @Part profileImg: MultipartBody.Part,
    @PartMap body: HashMap<String, RequestBody>
): Call<ResponseCatProfileData>
```

기존과는 다른 서버 통신이었기 때문에 request에 들어가는 String 값들을 **MIME Type**으로 변형 시켰고,  
이미지 또한 `MultipartBody.Part` 타입으로 변환시켜 주었습니다.

_Multpart로 고양이 프로필 등록을 서버에 요청하는 함수_

```
private fun settingDataMultiForm() {
    val PARSE_STRING = "text/plain"
    val pictureRb = settingImgMultiPart()
    val accessToken = EasySharedPreference.Companion.getString("accessToken", "")
    val name = RequestBody.create(MediaType.parse(PARSE_STRING), CatInfoData.profileName)
    val weight = RequestBody.create(MediaType.parse(PARSE_STRING), CatInfoData.profileWeight)
    val gender = RequestBody.create(MediaType.parse(PARSE_STRING), CatInfoData.profileGender)
    val neutral = RequestBody.create(MediaType.parse(PARSE_STRING), CatInfoData.profileNeutral)
    val age = RequestBody.create(MediaType.parse(PARSE_STRING), CatInfoData.profileAge)
    val info = RequestBody.create(MediaType.parse(PARSE_STRING), CatInfoData.profileInfo)

    mOunce.SERVICE.postCatProfile(
        token = accessToken,
        profileImg = pictureRb,
        body = hashMapOf<String, RequestBody>(
            "profileName" to name,
            "profileWeight" to weight,
            "profileGender" to gender,
            "profileNeutral" to neutral,
            "profileAge" to age,
            "profileInfo" to info
        )
    ).customEnqueue(
        onSuccess = {
            "OunceCatRegisterSuccess".showLog("CatRegisterOk")
            val intent = Intent(this,CatRegisterFinishActivity::class.java)
            startActivity(intent)
            finish()
        },
        onError = {
            "ServerError".showLog("고양이 프로필 등록 에러 : ${it.code()}")
            Toast.makeText(this, "Error", Toast.LENGTH_SHORT).show()
        }
    )
}
```

_갤러리에서 가져온 사진을 `MultipartBody.Part`타입으로 변환 하는 함수_

```
private fun settingImgMultiPart(): MultipartBody.Part {
    val options = BitmapFactory.Options()
    val inputStream = contentResolver.openInputStream(CatInfoData.catProfileUri!!)!!
    val bitmap = BitmapFactory.decodeStream(inputStream, null, options)
    val byteArrayOutputStream = ByteArrayOutputStream()
    bitmap!!.compress(Bitmap.CompressFormat.JPEG, 20, byteArrayOutputStream)
    val photoBody =
        RequestBody.create(MediaType.parse("image/jpg"),byteArrayOutputStream.toByteArray())

    return MultipartBody.Part.createFormData(
        "profileImg",
        File(CatInfoData.catProfileUri.toString()).name,
        photoBody)
}
```

프로필 이미지는 갤러리에서 불러 온 후 Crop 기능이 필요했기 때문에 [Cropper](https://github.com/ArthurHub/Android-Image-Cropper) 라이브러리를 이용했습니다.  
갤러리에 접근 시 권한을 설정해줘야 하기 때문에 좀 더 쉽게 권한 설정을 하기 위해서  
[TedPermission](https://github.com/ParkSangGwon/TedPermission) 라이브러리를 사용했습니다.

_CatProfileRegisterFragment.kt_

```
private fun settingPermission() {
    val permis = object : PermissionListener {
        override fun onPermissionGranted() {
            // 갤러리 호출
            callGallery()
        }

        override fun onPermissionDenied(deniedPermissions: MutableList<String>?) {
        }
    }

    TedPermission.with(mContext)
        .setPermissionListener(permis)
        .setRationaleMessage("갤러리 호출을 위해 권한을 설정해 주세요.")
        .setDeniedMessage("갤러리 권한은 기기 시스템 설정에서 변경 할 수 있습니다.")
        .setPermissions(
            android.Manifest.permission.WRITE_EXTERNAL_STORAGE
        ).check()
}
```

```
private fun callGallery() {
    CropImage.activity()
        .setGuidelines(CropImageView.Guidelines.ON)
        .setAspectRatio(4, 3)
        .start(mContext, this)
}

@SuppressLint("Recycle")
@Suppress("DEPRECATION")
override fun onActivityResult(requestCode: Int, resultCode: Int, data: Intent?) {
    super.onActivityResult(requestCode, resultCode, data)

    if (requestCode == CropImage.CROP_IMAGE_ACTIVITY_REQUEST_CODE) {
        val result = CropImage.getActivityResult(data)
        if (resultCode == Activity.RESULT_OK) {
            mSelectedImage = result.uri
            Glide.with(this)
                .load(mSelectedImage).thumbnail(0.1f).into(v.img_cat_profile)


            CatInfoData.catProfileUri = mSelectedImage
            "ShowCatProfileUri".showLog("${CatInfoData.catProfileUri.toString()}")
            checkText()
        }
    }
}
```

### 2-3. 메인 화면

> #### **BottomAppBar 사용과 StickyScrollView**

&nbsp;&nbsp;앱에서 제일 중요하다고 여겨지는 메인 화면 입니다.  
보통은 `BottomNavigationView`를 사용하여 메인 화면을 구성하는데 디자이너들이 원하는 화면을 구성하기 위해 이번에는 `BottomAppBar`를 사용해 보았습니다.  
처음 사용해보는 기능이었기에 많이 헤맸지만, 구글링을 통해 속성값과 특성을 파악하고 마지막에  
디자이너들이 제시한 화면의 요구사항을 충족시킬 수 있었습니다.

<p align="center"><img src="https://user-images.githubusercontent.com/55642709/88534812-d13c5600-d043-11ea-9922-0666dd972e08.PNG" width="30%"></p>

&nbsp;&nbsp; 디자이너들의 또 하나의 요구사항은 아래로 스크롤 시 리뷰가 헤더에 붙어서  
내용들만 스크롤 되게 하는 것이었습니다. 이 부분은 외부 라이브러리인 [StickyScrollView](https://github.com/didikk/sticky-nestedscrollview)를 이용하여 구현하였습니다.

_fragment_home.xml_

```
<me.didik.component.StickyNestedScrollView
        android:id="@+id/sticky_scroll_main"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:fillViewport="true"
        android:overScrollMode="never"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent">

        ...

        <androidx.constraintlayout.widget.ConstraintLayout
            android:id="@+id/layout_main_review_list"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_marginTop="10dp"
            android:background="@color/white"
            android:tag="sticky"
            app:layout_constraintEnd_toEndOf="parent"
            app:layout_constraintStart_toStartOf="parent"
            app:layout_constraintTop_toBottomOf="@id/layout_main_profile">

        ...
```

<p align="center"><img src ="https://user-images.githubusercontent.com/55642709/88535367-b7e7d980-d044-11ea-9d0f-5cd56be8a885.gif" width="30%"></p>

> #### **다른 프로필로 전환**

&nbsp;&nbsp;여러 마리의 고양이를 키우는 집사의 경우도 생각해서 한 계정당 여러 개의 고양이 프로필을 만들 수 있습니다.
현재 프로필의 이름 또는 화살표 아이콘을 클릭 하면 바텀시트로 현재 내 계정의 다른 고양이 프로필을 볼 수 있고,  
다른 프로필을 누르면 해당 프로필로 메인 화면이 구성된다. 맨 하단에는 새로운 고양이 프로필을 등록할 수 있으며  
최대 4마리의 고양이 프로필만 등록 가능하게 구현했습니다.

_HomeFragment.kt_

```
    @Suppress("DEPRECATION")
    @SuppressLint("ClickableViewAccessibility")
    override fun onCreateView(
        inflater: LayoutInflater, container: ViewGroup?,
        savedInstanceState: Bundle?
    ): View? {
        v = inflater.inflate(R.layout.fragment_home, container, false)

        ...

        //바텀시트 프로필 설정
        mBottomsheetProfile.setContentView(R.layout.profile_bottomsheet)

        ...

        //다른프로필 바텀 시트 세팅
        mBottomsheetProfile.rcv_bottom_profile.apply {
            adapter = mProfileAdapter
            layoutManager = LinearLayoutManager(mContext)
        }
        initBottomSheet()


        return v

    }

    override fun onViewCreated(view: View, savedInstanceState: Bundle?) {
        super.onViewCreated(view, savedInstanceState)

        ...

        //고양이 이름 옆 아이콘 클릭 시 다른 고양이 프로필 선택 창 생성
        img_main_profile_dropdown.setOnClickListener {
            showBottomSheet()
        }

        txt_main_profile.setOnClickListener {
            showBottomSheet()
        }

        ...
    }
```

```
private fun initBottomSheet(){
    val accessToken = EasySharedPreference.Companion.getString("accessToken", "")

    // 다른 계정 클릭 시 이벤트
    mProfileAdapter.setOnItemClickListener(object : BottomProfileAdapter.OnItemClickListener {
        @Suppress("DEPRECATION")
        override fun onItemClick(v: View, data: BottomProfileData.Data) {
            EasySharedPreference.Companion.putInt("profileIdx", data.profileIdx)
            val activity = activity as MainActivity
            activity.resetFragment(data.profileIdx)
            mBottomsheetProfile.dismiss()
        }
    })

    //계정추가 버튼 및 판단하는 클릭 리스너
    mBottomsheetProfile.layout_bottomsheet_add_profile.setOnClickListener {
        mOunce.SERVICE.postIsLimit(accessToken).customEnqueue(
            onSuccess = {
                it.data.let { data ->
                    if (data.possibleAddProfile) {
                        val intent = Intent(mContext, CatRegisterActivity::class.java)
                        startActivity(intent)
                    } else {
                        Toast.makeText(
                            mContext,
                            "최대 4개의 계정만 만들 수 있습니다.",
                            Toast.LENGTH_SHORT
                        ).show()
                    }
                }
            },
            onError = {
                "OunceMainBottomProfileServerError".showLog("프로필 추가 생성 오류")
            }
        )
    }
}
```

```
private fun showBottomSheet() {
    val accessToken = EasySharedPreference.Companion.getString("accessToken", "")

    mOunce.SERVICE.getConversionProfile(accessToken,mProfileIdx).customEnqueue(
        onSuccess = {
            "OunceStatus".showLog("프로필 바텀시트 호출 메세지 : ${it.message}")
            "OunceStatus".showLog("프로필 바텀시트 데이터 전달 \n ${it.data}")
            mProfileAdapter.data.clear()
            mProfileAdapter.data.addAll(it.data)
            mProfileAdapter.notifyDataSetChanged()
        },
        onError = {
            "OunceError".showLog("프로필 바텀시트 호출 오류")
        }
    )

    mBottomsheetProfile.show()

}
```

<p align="center"><img src="https://user-images.githubusercontent.com/55642709/88537203-18c4e100-d048-11ea-9a26-b5e4658bdb72.gif" width="30%"></p>

> #### **리뷰필터 역시 바텀 시트로 구성**

&nbsp;&nbsp;리뷰 타이틀바에서 우측 아이콘을 클릭하면 리뷰 필터가 바텀시트로 보여지게 됩니다.  
원하는 필터를 설정하고 선택완료를 누르면 필터가 적용된 리뷰들이 보이게 됩니다.  
서버에서 주재료,제조사 필터는 사용자가 작성한 제품 리뷰 카테고리들만 가져오게 되어 있어서,  
필터의 양이 많아지면 바텀 시트에서 스크롤이 될 수 있습니다.  
여기서 아쉬웠던 점은 바텀시트를 스크롤해서 필터를 설정하고 다시 선택완료를 누르려고  
화면 위로 스크롤 할 때 바텀시트가 닫혀버리는 현상을 잡을 수가 없던 점이었습니다.

<p align="center"><img src="https://user-images.githubusercontent.com/55642709/88538008-963d2100-d049-11ea-98a4-026e1c463312.gif" width="30%"></p>

> #### **스피너를 이용한 리뷰 정렬**
>
> &nbsp;&nbsp; 리뷰 정렬 목록은 스피너로 구성했습니다.  
> 가장 대중적인 방법으로 날짜 순, 총점 순, 기호도 순 문자열을 `<string-array>`태그로 감싸 *strings.xml*에 작성하고,  
> 메인 코드에서 가져와 사용하는 방식으로 스피너를 구현해 보았습니다.

_strings.xml_

```
<resources>
    ...

    <string-array name="main_review_array">
        <item>날짜 순</item>
        <item>총점 순</item>
        <item>기호도 순</item>
    </string-array>
</resources>
```

_HomeFragment.kt_

```
@Suppress("DEPRECATION")
@SuppressLint("ClickableViewAccessibility")
override fun onCreateView(
    inflater: LayoutInflater, container: ViewGroup?,
    savedInstanceState: Bundle?
): View? {

    ...

        // 스피너 설정
    val spinnerAdapter = ArrayAdapter(
        mContext,
        R.layout.main_custom_spinner, mItem
    )

    spinnerAdapter.setDropDownViewResource(R.layout.main_custom_dropdown)
    v.spinner_main.apply {
        adapter = spinnerAdapter
        onItemSelectedListener = object : AdapterView.OnItemSelectedListener {
            override fun onNothingSelected(p0: AdapterView<*>?) {
            }

            override fun onItemSelected(
                parent: AdapterView<*>?,
                view: View?,
                position: Int,
                id: Long
            ) {

                when (parent?.getItemAtPosition(position).toString()) {
                    "날짜 순" -> {
                        mRecyclerAdapter.data.clear()
                        startServerReviewDate()
                    }

                    "총점 순" -> {
                        mRecyclerAdapter.data.clear()
                        startServerReviewRating()
                    }

                    "기호도 순" -> {
                        mRecyclerAdapter.data.clear()
                        startServerReviewPrefer()
                    }

                }
            }
        }
    }

    ...
}

```

<p align="center"><img src="https://user-images.githubusercontent.com/55642709/88538480-6cd0c500-d04a-11ea-9917-0f0f3d649f0a.gif" width="30%"></p>

### 2-5. 다른 고양이 프로필

> #### **팔로잉 팔로워만 다르고 나머지는 동일**

&nbsp;&nbsp;내 계정의 고양이 프로필이 아닌 다른 계정의 고양이 프로필로 접근 시 보여지는 화면은 전체적으로 동일하나 팔로우 기능 부분만 다르게 구성되어 있습니다.  
처음 액티비티에 접근 할 때 내 프로필 계정이 팔로우 했는지를 서버로 부터 값을 받아와서  
화면에 보여지는 팔로우 버튼을 다르게 합니다. 이 과정에서 드로어블을 사용해 좀 더 편하게  
뷰를 변화 시킬 수 있었습니다. 버튼을 누르면 팔로우 또는 팔로우 취소 이벤트를 서버로 전송하게 됩니다.

<p align="center"><img src="https://user-images.githubusercontent.com/55642709/88539976-2af54e00-d04d-11ea-93b2-6b780595a12f.PNG" width="30%"></p>

### 2-6. 리뷰 수정,삭제

> #### **내 리뷰만 수정/삭제 버튼 활성화 다른 사람의 리뷰는 읽기 전용**

&nbsp;&nbsp;기록하기는 다른 파트원의 부분이었습니다. 담당하던 팀원이 기록하기 화면에서 어려움을 겪었기 때문에 중간 부분부터 같이 만들기 시작했습니다.  
팀원이 어려워 하던 부분은 다음과 같았습니다.

- 내가 리뷰한 기록하기 화면에서만 수정/삭제 버튼 활성화

- 수정 버튼을 누르기 전까지는 화면에 변화가 일어나서는 안된다.

먼저 리사이클러 뷰 아이템에 해당 리뷰를 작성한 계정의 인덱스 값이 존재합니다.  
아이템 클릭 시 `SharedPreference`에 저장되어 있는 계정 인덱스 값과 같다면 `intent`를 통해  
*True*값을 전달하고 그렇지 않다면 *False*값을 전달합니다.  
전달되는 값에 따라서 상단 타이틀의 값을 다르게 주고, *True*일 경우에만 수정,삭제 버튼을 활성화 시킵니다.  
수정,삭제 버튼은 `PopupMenu`를 통해 구현했습니다.

_RecordModifyActivity.kt_

```
override fun onCreate(savedInstanceState: Bundle?) {
    super.onCreate(savedInstanceState)
    setContentView(R.layout.activity_record_modify)

    StatusObject.setStatusBar(this)

    val intent = intent
    mReviewIdx = intent.getIntExtra("reviewIdx", 0)

    val isMe = intent.getBooleanExtra("isMy", true)

    if (isMe) {
        //내 리뷰 프로필이면 상단 텍스트 이름 변경
        txt_update_myrecord.text = "나의 기록"
        btn_record_popup.visibility = View.VISIBLE
    } else {
        txt_update_myrecord.text = "제품 리뷰"
    }

    enableChange(false, layout_modify_parent)

    ...

}
```

처음 화면에서는 수정 버튼을 누르기 전까지는 화면에 변화가 일어나서는 안되기 때문에  
모든 뷰들의 enable 속성을 *False*로 설정해 줍니다. 이 때 수정 삭제 버튼이 있는 앱바 부분은  
클릭 이벤트가 활성화 되어야 하므로, 그 부분만을 제외하고 설정해 줍니다.  
초기 화면에서는 수정 완료 버튼을 숨기고, 수정 버튼을 누르게 되면 enable 속성을 *True*로 변경해 주면서 수정 완료 버튼을 화면에 나타냅니다.

```
private fun enableChange(b : Boolean, vg : ViewGroup){
    for(i in 0 until vg.childCount){
        val child = vg.getChildAt(i)
        child.isEnabled = b
        if(child is AppBarLayout){
            continue
        }

        if(child is ViewGroup){
            enableChange(b , child)
        }
    }
}
```

<p align="center"><img src="https://user-images.githubusercontent.com/55642709/88542896-21221980-d052-11ea-92b8-e42495aeb56d.PNG" width="30%"><img src="https://user-images.githubusercontent.com/55642709/88542978-3f881500-d052-11ea-96a5-e06d46d9d7ac.PNG"width="30%"></p>

## 3. 후기 및 발전

> #### **저번 앱잼보다 나아진 개발 실력, 그러나 아직은 아쉬운 마무리**

&nbsp;&nbsp;저번 기수 앱잼 때보다는 확실히 더 나은 실력을 가지게 되었다고 느낀 프로젝트였습니다.  
개발 속도도 많이 향상되었고, 다양한 문제에 직면했을 때 좀 더 수월하게 해결할 수 있는 능력을 갖추게 된 것 같습니다.  
그러나 사소한 문제에 대해서 많은 삽질을 해서 시간을 뺏기는 경험을 하면서 아직까지는  
코드의 전체적인 흐름과 뷰의 특성을 파악하는데 많은 노력이 필요하다는 것을 깨닫기도 했습니다.
이번 프로젝트에서도 저번처럼 리드 개발자의 역할로써 팀원들을 이끌면서 진행했는데,  
내 부분을 만들기에 급급했던 저번과는 달리 이번에는 팀원들의 모르는 부분을 피드백 해주는 것과 동시에 개발하면서 터득한 나만의 팁을 공유하면서 진행할 수 있어서  
확실히 저번보다는 크게 발전했다라는 것을 느낄 수 있었습니다.

> #### **최우수상 그리고 MVP, 하지만 아직 배울 점이 많은 단계**

&nbsp;&nbsp;OUNCE 프로젝트는 최우수상이라는 우수한 성적을 거두었습니다. 그리고 개인적으로는 안드로이드 파트 MVP를 수상하면서 굉장히 성공적인 마무리를 했다고 볼 수 있습니다.  
동시에 아직 좀 더 배워야 할 점이 많다는 것을 깨달았습니다. 이번 프로젝트를 통해 노가다성 코드를 줄이는 `style`의 사용, 외부 라이브러리를 사용할 때 정확한 사용법과 사용하는 이유의 명시, 수명주기를 생각하는 자세 등 개발적인 부분에서 많은 성장을 했습니다.  
Git을 관리하는 법과 협업 프로젝트를 진행할 때의 방법에서도 많은 발전이 있었습니다.  
GitFlow 적용, Project, Issue 관리 등 전보다 Git을 더 잘 활용하는 느낌을 많이 받았습니다.  
이번 프로젝트를 통해 제가 더 공부해야할 부분들을 생각해 보았습니다.

- MVVM 디자인 패턴 적용을 위한 `ViewModel`과 `LiveData` 공부

- 백그라운드 작업을 위한 _코루틴_ 공부

- 이중 클릭 방지, 로딩 창 등 디테일한 세부 사항 구현

OUNCE 프로젝트에서 지난 프로젝트에 대한 아쉬웠던 부분들을 보완하여 좀 더 완성도 높은 앱을 만들 수 있었습니다.  
이 모든 결과는 저 뿐만이 아니라 다른 15명의 팀원들의 노력이 없었다면 이루어낼 수 없었을 것입니다.  
프로젝트가 끝난 지금 어느 정도 안드로이드 개발의 기본을 탄탄하게 가져갔다고 생각합니다.  
이제는 좀 더 심화된 부분까지 다룰 수 있는 멋진 안드로이드 개발자가 되겠습니다.
