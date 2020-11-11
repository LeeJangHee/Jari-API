# 회원 정보 수정

##  개요

 요청된 URL 매개 변수를 기반으로 회원 정보를 조회합니다.

##  사용 방법

###  회원 정보 조회 전 비밀번호 확인

{% api-method method="post" host="http://wkdgml96.iptime.org:8080" path="/users/ChangeValidate.php" %}
{% api-method-summary %}
 User Info Validate API
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="id" type="string" required=false %}
 String 사용자 아이디 \(필수\)
{% endapi-method-parameter %}

{% api-method-parameter name="password" type="string" required=false %}
 String 사용자 비밀번호 \(필수\)
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    // 회원정보 비밀번호 확인 성공
    "success": true,
    "id": "wkdgml96",
    "password": "123123"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



###  회원 정보 비밀번호 변경

{% api-method method="post" host="http://wkdgml96.iptime.org:8080" path="/users/update/password.php" %}
{% api-method-summary %}
 User Info Change Password API
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="id" type="string" required=false %}
 String 사용자 아이디
{% endapi-method-parameter %}

{% api-method-parameter name="password" type="string" required=false %}
 String 변경할 비밀번호
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    // 변경할 비밀번호가 다를 때
    // 성공
    "success": true
}

{
    // 변경할 비밀번호가 같을 때
    // 실
    "success": false
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



###  회원 정보 이름 변경

{% api-method method="post" host="http://wkdgml96.iptime.org:8080" path="/users/update/name.php" %}
{% api-method-summary %}
 User Info Change Name API
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="id" type="string" required=false %}
 String 사용자 아이디 \(필수\)
{% endapi-method-parameter %}

{% api-method-parameter name="name" type="string" required=false %}
 String 변경할 이름 \(필수\)
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    // 변경할 이름이 다를 때
    // 성공
    "success": true
}

{
    // 변경할 이름이 같을 때
    // 실패
    "success": false
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



###  회원 정보 전화번호 변경

{% api-method method="post" host="http://wkdgml96.iptime.org:8080" path="/users/update/phone.php" %}
{% api-method-summary %}
 User Info Change Phone API
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="id" type="string" required=false %}
 String 사용자 아이디 \(필수\)
{% endapi-method-parameter %}

{% api-method-parameter name="phone" type="string" required=false %}
 String 변경할 전화번호 \(필수\)
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    // 변경할 전화번호가 다를 때
    // 성공
    "success": true
}

{
    // 변경할 전화번호가 같을 때
    // 실패
    "success": false
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

