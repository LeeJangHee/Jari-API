# 로그인

## 개요

요청된 URL 매개 변수를 기반으로 로그인 정보를 조회합니다.



## 사용 방법

### 회원가입

{% api-method method="post" host="http://wkdgml96.iptime.org:8080" path="/users/Register.php" %}
{% api-method-summary %}
Sign Up API
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="id" type="string" required=false %}
 String ID \(필수\)
{% endapi-method-parameter %}

{% api-method-parameter name="password" type="string" required=false %}
 String Password \(필수\)
{% endapi-method-parameter %}

{% api-method-parameter name="name" type="string" required=false %}
 String Name \(필수\)
{% endapi-method-parameter %}

{% api-method-parameter name="phone" type="string" required=false %}
 String Phone \(필수\)
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    // 성공
    "success": true
}

{
    // 실패
    "success": false
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=302 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



### 아이디 중복검사

{% api-method method="post" host="http://wkdgml96.iptime.org:8080" path="/users/Validate.php" %}
{% api-method-summary %}
ID Validate API
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="id" type="string" required=false %}
 String ID \(필수\)
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    // 성공
    "success": true
}

{
    // 실패
    "success": false,
    "id": "wkdgml96"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



### 로그인

{% api-method method="post" host="http://wkdgml96.iptime.org:8080" path="/users/Login.php" %}
{% api-method-summary %}
Login API
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="id" type="string" required=false %}
 String ID \(필수\)
{% endapi-method-parameter %}

{% api-method-parameter name="password" type="string" required=false %}
 String Password \(필수\)
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    // 성공
    "success": true,
    "id": "wkdgml96",
    "password": "123123",
    "name": "janghee2",
    "phone": "38482784"
}

{
    // 실패
    "success": false
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

