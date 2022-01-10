# 발견 문제점
## 1.'조회' /board/view.do에서 에러 발생

> **원인** : view.jsp에서 DTO의 property를 잘못 기재

```java
//수정
${list[0].regdate} ==> ${list[0].regDate}
```
## 2. 수정 시 내용이 삭제되는 증상 발생

>**원인** : update.jsp에서 parametername에 오타

```html
