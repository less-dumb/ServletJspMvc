### π Reference
[Inflearn : μ€νλ§ MVC 1νΈ - λ°±μλ μΉ κ°λ° ν΅μ¬ κΈ°μ (κΉμνλ)](https://www.inflearn.com/course/%EC%8A%A4%ED%94%84%EB%A7%81-mvc-1/dashboard)
[MDN Web Docs](https://developer.mozilla.org/en-US/)
[μ€νλ§ κ³΅μ](https://spring.io/)

***
### 1. μΉ μ νλ¦¬μΌμ΄μ μ΄ν΄

#### HTTP μλ

μΉμ μ λΆ HTTP κΈ°λ°μΌλ‘ ν΅μ νκ² λ©λλ€.
μΉ λΈλΌμ°μ μμ URLμ μλ ₯νλ©΄,
μΈν°λ·μ ν΅ν΄ μλ²μ μ κ·Όνκ³ 
μλ²μμ  html μμ±ν΄μ ν΄λΌμ΄μΈνΈμκ² μ λ¬ν΄μ€λλ€.

ν΄λΌμ΄μΈνΈμμ μμ²­, μλ²μμ μλ΅ν  λ
__λͺ¨λ  κ²μ΄ HTTP__ κΈ°λ°μμ λμν©λλ€.

HTTP λ©μμ§μ μ μ‘λλ λ°μ΄ν°μ ννλ λ€μκ³Ό κ°μ΅λλ€.

- HTML, TEXT
- IMAGE, μμ±, μμ, νμΌ
- JSON, XML (API)
κ±°μ λͺ¨λ  ννμ λ°μ΄ν°λ₯Ό μ μ‘νλ κ²μ΄ κ°λ₯ ν©λλ€.
μλ²κ°μ λ°μ΄ν°λ₯Ό μ£Όκ³  λ°μ λλ λλΆλΆ HTTPλ₯Ό μ¬μ©ν©λλ€.
μ§κΈμ htmlκ°μ νμ΄νΌλ―Έλμ΄ λ¬Έμ λΏλ§ μλλΌ κ±°μ λͺ¨λ  κ²μ λ€ μ μ‘ν  μ μλ HTTPμ μλλΌκ³  ν©λλ€. λ°μΌνλ‘ HTTPμ μλλΌκ³  ν  μ μμ΅λλ€.

#### μΉ μλ²(Web Server)
- HTTP κΈ°λ°μΌλ‘ λμν©λλ€.
- μ μ  λ¦¬μμ€μ κΈ°ν λΆκ°κΈ°λ₯μ μ κ³΅ν©λλ€.
  - μ μ (νμΌ) HTML, CSS, JS, μ΄λ―Έμ§, μμ
  - μ) NGINX, APACHE
  
#### μΉ μ νλ¦¬μΌμ΄μ μλ²(WAS - Web Application Server)
- HTTP κΈ°λ°μΌλ‘ λμν©λλ€.
- μΉ μλ²μ κΈ°λ₯λ€μ ν¬ν¨νκ³  μμ΅λλ€. (μ μ  λ¦¬μμ€ μ κ³΅)
- νλ‘κ·Έλ¨ μ½λλ₯Ό μ€νν΄μ μ νλ¦¬μΌμ΄μ λ‘μ§μ μνν©λλ€.
  - λμ  HTML, HTTP API(JSON)
  - μλΈλ¦Ώ, JSP, μ€νλ§ MVC
    - μ) ν°μΊ£() Jetty, Undertow
    
#### μΉ μλ², μΉ μ νλ¦¬μΌμ΄μ μλ²(WAS) μ°¨μ΄
- __μΉ μλ²λ μ μ  λ¦¬μμ€(νμΌ) μ κ³΅, WASλ μ νλ¦¬μΌμ΄μ λ‘μ§κΉμ§ μνν©λλ€.__
- μΉ μλ²λ νλ‘κ·Έλ¨μ μ€ννλ κΈ°λ₯μ ν¬ν¨νκΈ°λ ν©λλ€.
- WASλ μΉ μλ²μ κΈ°λ₯μ μ κ³΅ν©λλ€.(μ©μ΄, κ²½κ³κ° λͺ¨νΈν©λλ€.)
- μλ°λ μλΈλ¦Ώ μ»¨νμ΄λ κΈ°λ₯μ μ κ³΅νλ©΄ WAS
  - μλΈλ¦Ώ μμ΄ μλ°μ½λλ₯Ό μ€ννλ μλ² νλ μμν¬λ μμ΅λλ€.
- __WASλ μ νλ¦¬μΌμ΄μ μ½λλ₯Ό μ€ννλλ° λ νΉνλμ΄ μλ€λ μ°¨μ΄κ° μμ΅λλ€.__


#### μΉ μμ€ν κ΅¬μ± - WAS, DB

WASλ μ μ  λ¦¬μμ€, μ νλ¦¬μΌμ΄μ λ‘μ§ λͺ¨λ μ κ³΅ κ°λ₯νκΈ° λλ¬Έμ WAS, DB λ§μΌλ‘ μμ€ν κ΅¬μ± κ°λ₯ν©λλ€.
νμ§λ§ λ€μκ³Ό κ°μ λ¬Έμ κ° μμ΅λλ€.

- WASκ° λλ¬΄ λ§μ μ­ν μ λ΄λΉν΄μ μλ² κ³ΌλΆνκ° μ°λ €λ©λλ.
- κ°μ₯ λΉμΌ μ νλ¦¬μΌμ΄μ λ‘μ§μ΄ μ μ  λ¦¬μμ€ λλ¬Έμ μνμ΄ μ΄λ €μΈ μ μμ΅λλ€.
- WAS μ₯μ μ μ κ·Ό λΆκ°μ΄κΈ° λλ¬Έμ μ€λ₯ νλ©΄λ λΈμΆμ΄ λΆκ°λ₯ν©λλ€.
![WAS](https://images.velog.io/images/urtimeislimited/post/22b65a67-dc40-4aee-a270-5fb6d90a4f6c/image.png)


κ·Έλμ μΌλ°μ μΌλ‘ λ€μκ³Ό κ°μ΄ μΉ μμ€νμ κ΅¬μ±ν©λλ€.

- μ μ  λ¦¬μμ€λ μΉ μλ²κ° μ²λ¦¬ν©λλ€.
- μΉ μλ²λ μ νλ¦¬μΌμ΄μ λ‘μ§κ°μ λμ μΈ μ²λ¦¬κ° νμν  λ WASμ μμ²­μ μμν©λλ€.
- WASλ μ€μν μ νλ¦¬μΌμ΄μ λ‘μ§λ§μ μ²λ¦¬νλ κ²μ μ λ΄ν©λλ€.
![webWasDb](https://images.velog.io/images/urtimeislimited/post/6f3717eb-e9eb-4abd-aa07-c82c125df53f/image.png)
- λν λ¦¬μμ€λ₯Ό ν¨μ¨μ μΌλ‘ κ΄λ¦¬ν  μ μμ΅λλ€.
  - μ μ  λ¦¬μμ€κ° λ§μ΄ μ¬μ©λλ©΄ Web μλ²λ₯Ό μ¦μ€νλ©΄ λ©λλ€.
  - μ νλ¦¬μΌμ΄μ λ¦¬μμ€κ° λ§μ΄ μ¬μ©λλ©΄ WAS μ¦μ€νλ©΄ λ©λλ€.
![wwd](https://images.velog.io/images/urtimeislimited/post/2c481c52-4d0f-4fde-9c16-fb43060a5633/image.png)

#### μΉ μμ€ν κ΅¬μ±(Web, Was, Db) μ₯μ 
- μ μ  λ¦¬μμ€λ§ μ κ³΅νλ μΉ μλ²λ μ μ£½μ§ μμ΅λλ€.
- μ νλ¦¬μΌμ΄μ λ‘μ§μ΄ λμνλ WAS μλ²λ μ μ£½μ΅λλ€.
- WAS, DB μ₯μ μ WEB μλ²κ° μ€λ₯ νλ©΄μ μ κ³΅νλ κ²μ΄ κ°λ₯ν©λλ€.
![Web, Was, Db](https://images.velog.io/images/urtimeislimited/post/403cc7fd-6457-404c-adc6-c18385c1ba0a/image.png)

#### μλΈλ¦Ώ

![form](https://images.velog.io/images/urtimeislimited/post/732ce5d0-ca07-41ad-bfe1-eee5515723e1/image.png)
html form νκ·Έλ₯Ό μμ±ν΄μ μ μ‘μ λμμν€λ©΄
μΉλΈλΌμ°μ λ λ€μκ³Ό κ°μ HTTP λ©μμ§λ₯Ό μμ±νμ¬ μμ²­ν©λλ€.

![post](https://images.velog.io/images/urtimeislimited/post/7ba9ed63-ea42-4066-a2af-fc06d5b8f84b/image.png)

μΉ μ νλ¦¬μΌμ΄μ μλ²λ₯Ό μ§μ  κ΅¬νν΄μΌ νλ€λ©΄ μλ―Έμλ λΉμ¦λμ€ λ‘μ§ μΈμ ν΄μΌν  μμμ΄ κ΅μ₯ν λ³΅μ‘νκ³  λ§μμ§λλ€.

![was](https://images.velog.io/images/urtimeislimited/post/bf116eda-4a45-4f5e-bb5d-d4d8f6381d44/image.png)

μ΄ λ μλΈλ¦Ώμ΄ λ±μ₯ν©λλ€. 
μλΈλ¦Ώμ μ§μνλ WASλ₯Ό μ¬μ©νλ©΄ μλΈλ¦Ώμ WASκ° μνν΄μΌ νλ μλ―Έμλ λΉμ¦λμ€ λ‘μ§μ μ μΈν λͺ¨λ  μμμ μ λΆ μλνν΄μ€λλ€.
![servlet](https://images.velog.io/images/urtimeislimited/post/5dba3a80-8ff6-482f-9683-1de8b8180c18/image.png)

μλΈλ¦Ώμ νΉμ§μ λ€μκ³Ό κ°μ΅λλ€.

```
@WebServlet(name = "helloServlet", urlPatterns = "/hello")
public class HelloServlet extends HttpServlet {
 @Override
 protected void service(HttpServletRequest request, HttpServletResponse response){
 //μ νλ¦¬μΌμ΄μ λ‘μ§
 }
}
```
- urlPatterns(/hello)μ URLμ΄ νΈμΆλλ©΄ μλΈλ¦Ώ μ½λκ° μ€νλ©λλ€.
- HTTP μμ²­ λ©μμ§ μ λ³΄λ₯Ό νΈλ¦¬νκ² μ¬μ©ν  μ μλ HttpServletRequest
- HTTP μλ΅ λ©μμ§ μ λ³΄λ₯Ό νΈλ¦¬νκ² μ κ³΅ν  μ μλ HttpServletResponse
- μλΈλ¦Ώμ ν΅ν΄ κ°λ°μλ HTTP μ€νμ λ§€μ° νΈλ¦¬νκ² μ¬μ©ν  μ μμ΅λλ€.
  - ν¨κ³Όμ μΌλ‘ μ¬μ©νλ €λ©΄ HTTP μ€νμ μ΄λμ λ μΈμ§νκ³  μμ΄μΌ νλ€κ³  ν©λλ€.

#### μλΈλ¦Ώ - HTTP μμ²­, μλ΅νλ¦
μλΈλ¦Ώμ ν΅ν HTTP μμ²­, μλ΅νλ¦μ λ€μκ³Ό κ°μ΅λλ€.
![servletRequesetResponse](https://images.velog.io/images/urtimeislimited/post/4b89f591-6e0a-4c4d-805a-65338e700c49/image.png)
1. μΉ λΈλΌμ°μ κ° localhost:8080/parameterλ₯Ό μλ ₯ν©λλ€.
2. HTTP μμ²­ λ©μμ§λ₯Ό κΈ°λ°μΌλ‘ request, response κ°μ²΄λ₯Ό μμ±ν©λλ€.
3. μμ±ν κ°μ²΄λ₯Ό μλΈλ¦Ώ μ»¨νμ΄λλ‘ μ λ¬νμ¬ helloServletμ μ€νν©λλ€.
4. helloServletμ μ’λ£ν΄μ responseκ°μ²΄ λ΄λΆμ returnκ°μ λ°ννλ©΄ responseκ°μ²΄ λ΄μ©μ κΈ°λ°μΌλ‘ μλ΅ν  HTTP μλ΅ λ©μμ§λ₯Ό μμ±νμ¬ μ λ¬ν©λλ€.



 HTTP μμ²­μ
- WASλ Request, Response κ°μ²΄λ₯Ό μλ‘ λ§λ€μ΄μ μλΈλ¦Ώ κ°μ²΄ νΈμΆν©λλ€.
- κ°λ°μλ Request κ°μ²΄μμ HTTP μμ²­ μ λ³΄λ₯Ό νΈλ¦¬νκ² κΊΌλ΄μ μ¬μ©ν©λλ€.
- κ°λ°μλ Response κ°μ²΄μ HTTP μλ΅ μ λ³΄λ₯Ό νΈλ¦¬νκ² μλ ₯ν  μ μμ΅λλ€.
- WASλ Response κ°μ²΄μ λ΄κ²¨μλ λ΄μ©μΌλ‘ HTTP μλ΅ μ λ³΄λ₯Ό μμ±νμ¬ μΉ λΈλΌμ°μ μκ² μ λ¬ν©λλ€.

#### μλΈλ¦Ώ μ»¨νμ΄λ

- ν°μΊ£μ²λΌ μλΈλ¦Ώμ μ§μνλ WASλ₯Ό μλΈλ¦Ώ μ»¨νμ΄λλΌκ³  ν©λλ€.
- μλΈλ¦Ώ μ»¨νμ΄λλ μλΈλ¦Ώ κ°μ²΄λ₯Ό μμ±, μ΄κΈ°ν, νΈμΆ, μ’λ£νλ μλͺμ£ΌκΈ°λ₯Ό κ΄λ¦¬ν©λλ€.
- μλΈλ¦Ώ κ°μ²΄λ __μ±κΈν€(λ¨μΌ κ°μ²΄ κ³΅μ , μ¬μ¬μ©)μΌλ‘ κ΄λ¦¬__ν©λλ€.
- μλ‘ λ€λ₯Έ κ³ κ°μ μμ²­ λ°μ΄ν°κ° μ¬ λ λ§λ€ κ³μ κ°μ²΄λ₯Ό μμ±νλ κ²μ λΉν¨μ¨μ μ΄κΈ° λλ¬Έμ
- μ΅μ΄ λ‘λ© μμ μ μλΈλ¦Ώ κ°μ²΄λ₯Ό λ―Έλ¦¬ λ§λ€μ΄λκ³  μ¬νμ©ν©λλ€.
- λͺ¨λ  κ³ κ° μμ²­μ λμΌν μλΈλ¦Ώ κ°μ²΄ μΈμ€ν΄μ€μ μ κ·Όνλλ‘ ν©λλ€.
- __κ³΅μ  λ³μ μ¬μ©μ μ£Όμν΄μΌ ν©λλ€.__
  - μ¬λ¬ ν΄λΌμ΄μΈνΈκ° νλμ κ°μ κ°μ²΄ μΈμ€ν΄μ€λ₯Ό κ³΅μ νκΈ° λλ¬Έμ μ±κΈν€ κ°μ²΄λ μνλ₯Ό μ μ§(stateful)νκ² μ€κ³νλ©΄ μλκ³ , λ¬΄μν(stateless)λ‘ μ€κ³ν΄μΌ ν©λλ€.
    - νΉμ  ν΄λΌμ΄μΈνΈμ μμ‘΄μ μΈ νλκ° μμΌλ©΄ μλ©λλ€.
    - νΉμ  ν΄λΌμ΄μΈνΈκ° κ°μ λ³κ²½ν  μ μλ νλκ° μμΌλ©΄ μλ©λλ€.
    - κ°κΈμ  μ½κΈ°λ§ κ°λ₯ν΄μΌ ν©λλ€.
    - νλ λμ  μλ°μμ κ³΅μ λμ§ μλ μ§μ­λ³μ, νλΌλ―Έν°, ThreadLocal λ±μ μ¬μ©ν΄μΌ ν©λλ€.
- μλΈλ¦Ώ μ»¨νμ΄λ μ’λ£μ ν¨κ» μ’λ£λ©λλ€.
- JSPλ μλΈλ¦ΏμΌλ‘ λ³ν λμ΄μ μ¬μ©νκ² λ©λλ€.
- __λμ μμ²­μ μν λ©ν° μ°λ λ μ²λ¦¬λ₯Ό μ§μν©λλ€.__
  - WASμ μμ£Ό ν° νΉμ§μΌλ‘μ¨ λΈλΌμ°μ μμ λ§μ μμ²­μ΄ μλ κ°λ°μ λμ  λ©ν° μ°λ λ μ²λ¦¬λ₯Ό μλνν΄μ€λλ€.
  
#### λμ μμ²­ - λ©ν° μ°λ λ

μΌλ°μ μΌλ‘ μΉ λΈλΌμ°μ  μμ²­μ WASμ TCP/IP μ»€λ₯μμ΄ μ°κ²°λμ΄ μλΈλ¦Ώμ νΈμΆν©λλ€. 

![request](https://images.velog.io/images/urtimeislimited/post/0a42826e-8d2e-43da-99a7-6f103a7ccaf6/image.png)


μ΄ μν©μμ μλΈλ¦Ώμ νΈμΆνλ κ²μ μ°λ λ μλλ€.
> μ°λ λ
- μ νλ¦¬μΌμ΄μ μ½λλ₯Ό νλνλ μμ°¨μ μΌλ‘ μ€ννλ κ²μλλ€.(νλ‘μΈμ€λ νλ‘κ·Έλ¨ μν, μ°λ λλ κ·Έ λ΄λΆμμ λ€μνκ² λλ©λλ€.)
- μ) μλ° λ©μΈ λ©μλλ₯Ό μ²μ μ€ννλ©΄ mainμ΄λΌλ μ΄λ¦μ μ°λ λκ° μ€νλ©λλ€.
- μ°λ λκ° μλ€λ©΄ μλ° μ νλ¦¬μΌμ΄μ μ€νμ΄ λΆκ°λ₯ν©λλ€.
- μ°λ λλ νλ²μ νλμ μ½λ λΌμΈλ§ μνν©λλ€.
- λμ μ²λ¦¬κ° νμνλ©΄ μ°λ λλ₯Ό μΆκ°λ‘ μμ±ν΄μ€μΌ ν©λλ€.

μ) λ¨μΌ μμ²­ - μ°λ λ νλ μ¬μ©

![singleThread](https://images.velog.io/images/urtimeislimited/post/26de2a84-5b67-434d-ae30-46da7f5a97ed/image.png)
![singleThread2](https://images.velog.io/images/urtimeislimited/post/9d418226-c8fd-440b-9219-011c99e9992b/image.png)
![singleThread3](https://images.velog.io/images/urtimeislimited/post/2e13ed33-04a0-4e80-8cc0-5c25be87da89/image.png)

λ§μ½ μ°λ λλ νλμΈλ° μμ²­ μ λ¦¬κ° μ§μ°λλ μν©μμ
λ€μ€ μμ²­μ΄ λ°μν  κ²½μ° κΈ°μ‘΄ μμ²­κ³Ό ν¨κ» μ₯μ κ° λ°μν©λλ€.

![manyRequest](https://images.velog.io/images/urtimeislimited/post/2ac15e1c-d6ea-42b0-8e96-fa10ada73f71/image.png)

μμ²­1 μ°λ λλ μ§μ°λλ©΄μ λμμ μμ²­2μ μ°λ λλ μ²λ¦¬λμ§ μκΈ° λλ¬Έμλλ€.


λ¨μνκ² μμ²­λ§λ€ μ°λ λλ₯Ό μμ±νλ€λ©΄ λ€μκ³Ό κ°μ μ₯λ¨μ μ΄ μμ΅λλ€.
![requestByThread](https://images.velog.io/images/urtimeislimited/post/fae81e04-3d3e-4ffa-9e10-a91faa51174e/image.png)
- μ₯μ 
  - λμ μμ²­μ μ²λ¦¬ν  μ μμ΅λλ€.
  - λ¦¬μμ€(CPU, λ©λͺ¨λ¦¬)κ° νμ©ν  λκΉμ§ μ²λ¦¬ κ°λ₯ν©λλ€.
  - νλμ μ°λ λκ° μ§μ° λμ΄λ, λλ¨Έμ§ μ°λ λλ μ μμΌλ‘ λμν©λλ€.
- λ¨μ 
  - μ°λ λλ μμ± λΉμ©μ΄ λ§€μ° λΉμλλ€.
    - λ°λΌμ κ³ κ° μμ²­λ§λ€ μ°λ λλ₯΄λ₯΄ μμ±νλ©΄ μλ΅ μλκ° λ¦μ΄μ§λλ€.
  - μ°λ λλ μ»¨νμ€νΈ μ€μμΉ­ λΉμ©μ΄ λ°μν©λλ€.
  - μ°λ λ μμ±μ μ νμ΄ μμ΅λλ€.
    - λ°λΌμ κ³ κ° μμ²­μ΄ λλ¬΄ λ§μ΄ μ€λ©΄ CPU, λ©λͺ¨λ¦¬ μκ³μ μ λμ΄μ μλ²κ° μ£½μ μλ μμ΅λλ€.

μ΄λ¬ν μ₯λ¨μ μ ν΄κ²°νκΈ° μν΄ μ°λ λ ν(λ―Έλ¦¬ μμ±ν μ°λ λ)μ΄ μ‘΄μ¬ν©λλ€.
 - μ°λ λ νμ΄ μλ μν©μμ μμ²­μ΄ μ€λ©΄ μ°λ λλ₯Ό λκΈ°νκ±°λ κ±°μ ν  μ μμ΅λλ€.
 
 ![threadPool](https://images.velog.io/images/urtimeislimited/post/c84fa659-29c6-4731-b275-6ed715a8adb4/image.png)
 
 #### μ°λ λ ν (μμ²­ λ§λ€ μ°λ λ μμ±μ λ¨μ  λ³΄μ)
 - νΉμ§
   - νμν μ°λ λλ₯Ό μ°λ λ νμ λ³΄κ΄νκ³  κ΄λ¦¬ν©λλ€.
   - μ°λ λ νμ μμ± κ°λ₯ν μ°λ λμ μ΅λμΉλ₯Ό κ΄λ¦¬ν©λλ€. ν°μΊ£μ μ΅λ 200κ° κΈ°λ³Έ μ€μ (λ³κ²½ κ°λ₯)
 - μ¬μ©
   - μ°λ λκ° νμνλ©΄, μ΄λ―Έ μμ±λμ΄ μλ μ°λ λλ₯Ό μ°λ λ νμμ κΊΌλ΄μ μ¬μ©ν©λλ€.
   - μ¬μ© μ’λ£μ μ°λ λ νμ ν΄λΉ μ°λ λλ₯Ό λ°λ©ν©λλ€.
   - μ΅λ μ°λ λκ° λͺ¨λ μ¬μ©μ€μ΄μ΄μ νμ μ°λ λκ° μμ κ²½μ°
     - κΈ°λ€λ¦¬λ μμ²­μ κ±°μ νκ±°λ νΉμ  μ«μλ§νΌλ§ λκΈ°νλλ‘ μ€μ ν  μ μμ΅λλ€.
 - μ₯μ 
   - μ°λ λκ° λ―Έλ¦¬ μμ±λμ΄ μμΌλ―λ‘, μ°λ λλ₯Ό μμ±νκ³  μ’λ£νλ λΉμ©(CPU)μ΄ μ μ½λκ³ , μλ΅ μκ°μ΄ λΉ λ¦λλ€.
   - μμ± κ°λ₯ν μ°λ λμ μ΅λμΉκ° μ€μ λμ΄ μμΌλ―λ‘ λλ¬΄ λ§μ μμ²­μ΄ λ€μ΄μλ κΈ°μ‘΄ μμ²­μ μμ νκ² μ²λ¦¬ν  μ μμ΅λλ€.
   
#### TIP
- WASμ μ£Όμ νλ ν¬μΈνΈλ μ΅λ μ°λ λ(max thread) μμλλ€.
- μ΄ κ°μ λλ¬΄ λ?κ² μ€μ νλ©΄
  - λμ μμ²­μ΄ λ§μ λ μλ² λ¦¬μμ€λ μ¬μ λ‘­μ§λ§, ν΄λΌμ΄μΈνΈλ μλ΅ μ§μ° μνκ° λ©λλ€.
  ![threadPoolLow](https://images.velog.io/images/urtimeislimited/post/786a29fd-9d27-4c25-b79f-69bfeeb9e419/image.png)
- μ΄ κ°μ λλ¬΄ λκ² μ€μ νλ©΄
  - λμ μμ²­μ΄ λ§μ λ CPU, λ©λͺ¨λ¦¬ λ¦¬μμ€ μκ³μ  μ΄κ³Όλ‘ μλ²κ° λ€μ΄λ©λλ€.
- μ₯μ  λ°μμ
  - ν΄λΌμ°λλ©΄ μΌλ¨ μλ²λΆν° λλ¦¬κ³ , μ΄νμ νλν©λλ€.
  - ν΄λΌμ°λκ° μλλ©΄ μ΄μ¬ν νλν©λλ€.

#### μ°λ λ νμ μ μ  μ«μ
- μ νλ¦¬μΌμ΄μ λ‘μ§μ λ³΅μ‘λ, CPU, λ©λͺ¨λ¦¬, IO λ¦¬μμ€ μν©μ λ°λΌ λͺ¨λ λ€λ₯΄κΈ° λλ¬Έμ λκ΅¬λΌλ μ΅μ μ ν΄λ₯Ό λ΄κΈ΄ μ΄λ ΅λ€κ³  ν©λλ€. λ€λ§ λλ΅μ μΈ κ°μ μ‘μ΅λλ€. κ·Έλμ μ±λ₯νμ€νΈλ₯Ό ν΄λ΄μΌ νλ€κ³  ν©λλ€.
- μ±λ₯ νμ€νΈ
  - μ΅λν μ€μ  μλΉμ€μ μ μ¬νκ² μ±λ₯ νμ€νΈλ₯Ό μλν©λλ€.
  - ν΄: μνμΉ ab, μ μ΄λ―Έν°, nGrinder
  
> ν΅μ¬
__WASλ λ©ν°μ°λ λλ₯Ό μ§μν©λλ€.__
- λ©ν° μ°λ λμ λν λΆλΆμ WASκ° μ²λ¦¬ν©λλ€.
- __κ°λ°μκ° λ©ν° μ°λ λ κ΄λ ¨ μ½λλ₯Ό μ κ²½μ°μ§ μμλ λ©λλ€.__
- λ°λΌμ κ°λ°μλ λ§μΉ __μ±κΈ μ°λ λ νλ‘κ·Έλλ°μ νλ―μ΄ νΈλ¦¬νκ² μμ€ μ½λλ₯Ό κ°λ°__ν  μ μμ΅λλ€.
- λ©ν° μ°λ λ νκ²½μ΄λ―λ‘ μ±κΈν€ κ°μ²΄(μλΈλ¦Ώ, μ€νλ§ λΉ)λ μ£Όμν΄μ μ¬μ©ν΄μΌ ν©λλ€.

#### HTML, HTTP API, CSR, SSR
1. μ μ  λ¦¬μμ€
- κ³ μ λ HTML νμΌ, CSS, JS, μ΄λ―Έμ§, μμ λ±μ μ κ³΅ν©λλ€.
- μ£Όλ‘ μΉ λΈλΌμ°μ μμ μμ²­μ΄ μ΅λλ€.
![staticResource](https://images.velog.io/images/urtimeislimited/post/8a7602c4-094f-4de2-a285-082d0e9cb9d2/image.png)
2. HTML νμ΄μ§
- λμ μΌλ‘ νμν HTML νμ΄μ§λ₯Ό μμ²­ν  κ²½μ° 
- WASμμ DBμ μ κ·Ό νμ¬ μ‘°νν μ λ³΄λ₯Ό κΈ°λ°μΌλ‘ λμ μΈ HTMLμ μμ±νμ¬ μ λ¬ν©λλ€. μ) JSP, Thymeleaf
![nonStaticHtml](https://images.velog.io/images/urtimeislimited/post/cb3a996c-7838-404a-a493-7e6427287c47/image.png)
3. HTTP API
- HTMLμ΄ μλ λ°μ΄ν°λ₯Ό μ κ³΅ν©λλ€.
- μ£Όλ‘ JSON νμμ μ¬μ©ν©λλ€.
![httpAPI](https://images.velog.io/images/urtimeislimited/post/630ca1b7-14f7-4cdd-b961-2c2a92ffece2/image.png)
- λ€μν μμ€νμμ νΈμΆν  μ μμ΅λλ€.
  - λ°μ΄ν°λ§ μ£Όκ³  λ°μ΅λλ€. 
    - UI νλ©΄μ΄ νμνλ©΄ ν΄λΌμ΄μΈνΈκ° λ³λλ‘ μ²λ¦¬ν©λλ€.
  - μ± : μμ΄ν°, μλλ‘μ΄λ κ°μ μ± ν΄λΌμ΄μΈνΈμμ UIμ λ³λλ‘ λ°μ΄ν°λ§ μ£Όκ³  λ°λλ°μ μ¬μ©λ©λλ€.
  - μΉ ν΄λΌμ΄μΈνΈ : HTMLμμ Form μ μ‘ λμ  μλ° μ€ν¬λ¦½νΈλ₯Ό ν΅ν ν΅μ μ μ¬μ©(AJAX)λ©λλ€. μ) React, VueJs κ°μ μΉ ν΄λΌμ΄μΈνΈμ ν¨κ»ν  λ API ν΅μ μ λ§μ΄ μ¬μ©νλ€κ³  ν©λλ€.
  - μλ² to μλ² : μ£Όλ‘ λ°±μλ μμ€ν ν΅μ μ μ¬μ©λ©λλ€. (HTMLμ΄ μ ν μμ΅λλ€.)
  ![httpAPI2](https://images.velog.io/images/urtimeislimited/post/d507e9e2-088d-43fa-b393-3e0f14aeba3f/image.png)
  - λ€μν μμ€ν μ°λ
    - μ£Όλ‘ JSON ννλ‘ λ°μ΄ν° ν΅μ 
    - UI ν΄λΌμ΄μΈνΈ μ μ 
      - μ± ν΄λΌμ΄μΈνΈ(μμ΄ν°, μλλ‘μ΄λ, PC μ±)
      - μΉ λΈλΌμ°μ μμ μλ°μ€ν¬λ¦½νΈλ₯Ό ν΅ν HTTP API νΈμΆ
      - React, Vue.js κ°μ μΉ ν΄λΌμ΄μΈνΈ
    - μλ² to μλ²
      - μ£Όλ¬Έ μλ² -> κ²°μ  μλ²
      - κΈ°μκ° λ°μ΄ν° ν΅μ 
  
  λ°±μλ κ°λ°μλ μ μ  λ¦¬μμ€, HTML νμ΄μ§, HTTP APIλ₯Ό μ΄λ»κ² μ κ³΅ν μ§μ λν΄ κ³ λ―Όν΄μΌ ν©λλ€.
  
#### μλ²μ¬μ΄λ λ λλ§, ν΄λΌμ΄μΈνΈ μ¬μ΄λ λ λλ§
- __SSR - μλ² μ¬μ΄λ λ λλ§__
  - μλ²μμ μ΅μ’ HTMLμ μμ±ν΄μ ν΄λΌμ΄μΈνΈμ μ λ¬νλ κ²μ μλ―Έν©λλ€.
    1. μλ²μμ DBμ μ κ·Όμ μ λ³΄λ₯Ό μ‘°νν©λλ€.
    2. 1μ κΈ°λ°μΌλ‘ λμ  HTMLμ μμ±νμ¬ μ΅μ’ HTMLμ μλ΅ν©λλ€.
  - μ¦, HTML μ΅μ’ κ²°κ³ΌκΉμ§ μλ²μμ λ§λ€μ΄μ μΉ λΈλΌμ°μ μ μ λ¬ν©λλ€.
  - μ£Όλ‘ μ μ μΈ νλ©΄μ μ¬μ©λ©λλ€.
  - κ΄λ ¨κΈ°μ : JSP, νμλ¦¬ν -> __λ°±μλ κ°λ°μ__
  ![ssr](https://images.velog.io/images/urtimeislimited/post/8ca6bb69-ed59-4222-9d62-6d8713d81f21/image.png)
- __CSR - ν΄λΌμ΄μΈνΈ μ¬μ΄λ λ λλ§__
  - HTML κ²°κ³Όλ₯Ό μλ°μ€ν¬λ¦½νΈλ₯Ό μ¬μ©ν΄ μΉ λΈλΌμ°μ μμ λμ μΌλ‘ μμ±ν΄μ μ μ©ν©λλ€.
    1. HTMLμ μμ²­ν©λλ€. (λ΄μ© μμ΄ μλ°μ€ν¬λ¦½νΈ λ§ν¬λ§ μ λ¬ν©λλ€.)
    2. ν΄λΌμ΄μΈνΈ λ‘μ§κ³Ό HTML λ λλ§ μ λ³΄λ₯Ό ν¬ν¨ν μλ°μ€ν¬λ¦½νΈλ₯Ό μμ²­ν©λλ€.
    3. HTTP API λ°μ΄ν°λ₯Ό μμ²­νμ¬ μλ²λ₯Ό ν΅ν΄ DBμ μ μ₯λ λ°μ΄ν°λ₯Ό JSONκ³Ό κ°μ νμμΌλ‘ μλ΅λ°μ΅λλ€.
    4. μΉ λΈλΌμ°μ μμ 2μ 3μ μ‘°ν©νμ¬ μ΅μ’ HTML κ²°κ³Όλ₯Ό λ λλ§ν©λλ€.
  - μ£Όλ‘ λμ μΈ νλ©΄μ μ¬μ©νλ©° μΉ νκ²½μ λ§μΉ μ±μ²λΌ νμν λΆλΆλ§λ€ λ³κ²½ν  μ μμ΅λλ€.
  - μ) κ΅¬κΈ μ§λ, Gmail, κ΅¬κΈ μΊλ¦°λ
  - κ΄λ ¨κΈ°μ : React, Vue.js -> __μΉ νλ‘ νΈμλ κ°λ°μ__
![csr](https://images.velog.io/images/urtimeislimited/post/d1deb42f-98cb-4897-8582-9ce8915a0767/image.png)
- μ°Έκ³ 
  - React, Vue.jsλ₯Ό CSR + SSR λμμ μ§μνλ μΉ νλ μμν¬λ μμ΅λλ€.
  - SSRμ μ¬μ©νλλΌλ, μλ°μ€ν¬λ¦½νΈλ₯Ό μ¬μ©ν΄μ νλ©΄ μΌλΆλ₯Ό λμ μΌλ‘ λ³κ²½ κ°λ₯ν©λλ€.
  
  #### κ·Έλ λ€λ©΄ λ°±μλ κ°λ°μ μμ₯μμ UIκΈ°μ μ μ΄λκΉμ§ μμμΌ νλμ?
- __λ°±μλ - μλ² μ¬μ΄λ λ λλ§ κΈ°μ __
  - JSP, νμλ¦¬ν
  - νλ©΄μ΄ μ μ μ΄κ³ , λ³΅μ‘νμ§ μμ λ μ¬μ©ν©λλ€.
  - λ°±μλ κ°λ°μλ μλ² μ¬μ΄λ λ λλ§ κΈ°μ  νμ΅ __νμ__μλλ€.
- __μΉ νλ‘ νΈμλ - ν΄λΌμ΄μΈνΈ μ¬μ΄λ λ λλ§ κΈ°μ __
  - React, Vue.js
  - λ³΅μ‘νκ³  λμ μΈ UI μ¬μ©ν©λλ€.
  - μΉ νλ‘ νΈμλ κ°λ°μμ μ λ¬Έ λΆμΌ
- __μ νκ³Ό μ§μ€__
  - λ°±μλ κ°λ°μμ μΉ νλ‘ νΈμλ κΈ°μ  νμ΅μ __μ΅μ__μλλ€.
  - λ°±μλ κ°λ°μλ μλ², DB, μΈνλΌ λ±λ± μ λ§μ λ°±μλ κΈ°μ μ κ³΅λΆν΄μΌ ν©λλ€.
  - μΉ νλ‘ νΈμλλ κΉμ΄μκ² μ νλ €λ©΄ μλ ¨μ μ€λ μκ°μ΄ νμνλ€κ³  ν©λλ€.
  
#### μλ° μΉ κΈ°μ  μ­μ¬ - κ³Όκ±° κΈ°μ 
- μλΈλ¦Ώ - 1997
  - λμ  HTML μμ±μ΄ μ΄λ ΅λ€λ λ¨μ μ΄ μμμ΅λλ€.
- JSP - 1999
  - λμ  HTML μμ±μ νΈλ¦¬νμ§λ§, λΉμ¦λμ€ λ‘μ§κΉμ§ λλ¬΄ λ§μ μ­ν  λ΄λΉνμ¬ μ μ§ λ³΄μκ° λλ¬΄ μ΄λ €μ λ€κ³  ν©λλ€.
- μλΈλ¦Ώ, JSP μ‘°ν© MVC ν¨ν΄ μ¬μ©
  - λͺ¨λΈ, λ·° μ»¨νΈλ‘€λ¬λ‘ μ­ν μ λλμ΄ κ°λ°νλλ‘ λ³κ²½λμμ΅λλ€.
- MVC νλ μμν¬ μΆμΆ μ κ΅­ μλ - 2000λ μ΄ ~ 2010λ μ΄
  - MVC ν¨ν΄ μλν, λ³΅μ‘ν μΉ κΈ°μ μ νΈλ¦¬νκ² μ¬μ©ν  μ μλ λ€μν κΈ°λ₯μ μ§μν μ μκ²λ©λλ€.
  - νΈλ¦¬ν¨κ³Ό λ€μμ± λλΆμ μ¬λ¬ νλ μμν¬κ° λ±μ₯νκ² λ©λλ€. μ) μ€νΈλΏμΈ , μΉμν¬, μ€νλ§ MVC(κ³Όκ±° λ²μ )
  
#### μλ° μΉ κΈ°μ  μ­μ¬ - νμ¬ μ¬μ© κΈ°μ 
- __μ λΈνμ΄μ κΈ°λ°μ μ€νλ§ MVC λ±μ₯__μΌλ‘ νλ μμν¬κ° ν΅ν©λλ€.
  - @Controller
  - MVC νλ μμν¬μ μΆμΆ μ κ΅­ μλ λ§λ¬΄λ¦¬
- __μ€νλ§ λΆνΈμ λ±μ₯__
  - μ€νλ§ λΆνΈλ μλ²λ₯Ό λ΄μ₯ν©λλ€.
    - κ³Όκ±°μλ μλ²μ WASλ₯Ό μ§μ  μ€μΉνκ³ , μμ€λ λ°λ‘ War νμΌμ λ§λ€μ΄μ μ€μΉν WASμ λ°°ν¬νμ΅λλ€. (ν°μΊ£ μ€μΉ, μμ€ λΉλ.... λ³΅μ‘νμ΅λλ€.)
  - __μ€νλ§ λΆνΈλ λΉλ κ²°κ³Ό(Jar)μ WAS μλ² ν¬ν¨__νμ¬ λ³΅μ‘ν¨μ ν΄κ²°νμ΅λλ€. -> __λΉλ λ°°ν¬ λ¨μν__
  
#### μ΅μ  κΈ°μ  - μ€νλ§ μΉ κΈ°μ μ λΆν
- Web Servlet - Spring MVC
  - μλΈλ¦Ώ μμμ Spring MVCλ₯Ό κΈ°λ°μΌλ‘ λμνλ λ°©μ
    - HTTP Request, HTTPResponseμ¬μ©, WASμμ λ©ν° μ°λ λ μ§μνλ μ₯μ μ κ°μ§λλ€.
- Web Reactive - Spring WebFlux(μλ°λ Node.jsμ²λΌ..)
  - μμ ν λΉλκΈ° λ λΈλ¬νΉ μ²λ¦¬
  - μ΅μ μ°λ λλ‘ μ΅λ μ±λ₯ -> μ°λ λ μ»¨νμ€νΈ μ€μμΉ­ λΉμ© ν¨μ¨ν
  - ν¨μν μ€νμΌλ‘ κ°λ° - λμμ²λ¦¬ μ½λ ν¨μ¨ν
  - μλΈλ¦Ώ κΈ°μ μ μ¬μ©νμ§ μμ΅λλ€. ([Netty](https://www.baeldung.com/spring-boot-reactor-netty#:~:text=Reactor%20Netty%20is%20an%20asynchronous,and%20UDP%20clients%20and%20servers.&text=Spring%20WebFlux%20is%20a%20part,programming%20support%20for%20web%20applications.))
  - κ·Έλ°λ°
    - μΉ νλ­μ€λ κΈ°μ μ  λμ΄λκ° λ§€μ° λμ΅λλ€.
    - μμ§μ RDB μ§μμ΄ λΆμ‘±ν©λλ€.
    - μΌλ° MVCμ μ°λ λ λͺ¨λΈλ μΆ©λΆν λΉ λ¦λλ€.
    - μ€λ¬΄μμ μμ§ λ§μ΄ μ¬μ©νμ§ μλλ€κ³  ν©λλ€.(μ μ²΄ 1% μ΄ν, μ±λ₯ μ΅μ ν + λ³΅μ‘ν API νΈμΆμ μ¬μ©ν΄μΌ ν¨κ³Όκ° μλ€κ³  ν©λλ€.)
    
#### μλ° λ·° ννλ¦Ώ μ­μ¬
λ°±μλμμ HTMLμ λμ μΌλ‘ νΈλ¦¬νκ² μμ±νλ κΈ°λ₯μ μλ―Έν©λλ€.
λ°μ ν΄μ¨ μμλ λ€μκ³Ό κ°μ΅λλ€.
1. JSP : μλ λλ¦Ό, κΈ°λ₯μ΄ λΆμ‘±νμ΅λλ€.
2. νλ¦¬λ§μ»€(Freemarker), Velocity(λ²¨λ‘μν°)
   - μλ λ¬Έμ  ν΄κ²°, λ€μν κΈ°λ₯μ μ κ³΅νλ μ½λκ° λ€μμ¬ λ³΅μ‘νμ΅λλ€.
3. νμλ¦¬ν(Thymeleaf)
   - λ΄μΆλ΄ ννλ¦Ώ: HTMLμ λͺ¨μμ μ μ§νλ©΄μ λ·° ννλ¦Ώ μ μ© κ°λ₯ν ννλ¦Ώμ μλ―Έν©λλ€.
   - __μ€νλ§ MVCμ κΈ°λ₯ ν΅ν©__μ΄ κ°λ ₯ν©λλ€.
   - μ΅μ μ μ ν, λ¨ μ±λ₯μ νλ¦¬λ§μ»€, λ²¨λ‘μν°κ° λ λΉ λ¦λλ€.(μ΄μκ° λ  μ λμ μ°¨μ΄λ μλλΌκ³  ν©λλ€.)

***
### 2. μλΈλ¦Ώ
μλ° μΉ κΈ°μ μ κ°μ₯ κΈ°μ΄κ° λλ μλΈλ¦Ώμ λν΄ λ€μκ³Ό κ°μ μμλ‘ μμλ³΄κ² μ΅λλ€.
1. μλΈλ¦Ώ
2. JSP
3. MVC ν¨ν΄ 
4. MVC νλ μμν¬ 
5. μ€νλ§ MVC νμ©

#### νλ‘μ νΈ μμ±
[μ€νλ§ λΆνΈ μ€νν°](https://start.spring.io/)

- νλ‘μ νΈ μ ν
  - Project: Gradle Project
  - Language: Java
  - Spring Boot: 2.6.3
- Project Metadata
  -Group: hello
  -Artifact: servlet
  -Name: servlet
  -Package name: hello.servlet
-Packaging: War
  - JSPλ₯Ό μ€ννκΈ° μν΄ Jarκ° μλ Warλ₯Ό μ νν©λλ€.
-Java: 11
Dependencies: Spring Web, Lombok

build.gradle
```
plugins {
	id 'org.springframework.boot' version '2.6.3'
	id 'io.spring.dependency-management' version '1.0.11.RELEASE'
	id 'java'
	id 'war'
}

group = 'hello'
version = '0.0.1-SNAPSHOT'
sourceCompatibility = '11'

configurations {
	compileOnly {
		extendsFrom annotationProcessor
	}
}

repositories {
	mavenCentral()
}

dependencies {
	implementation 'org.springframework.boot:spring-boot-starter-web'
	compileOnly 'org.projectlombok:lombok'
	annotationProcessor 'org.projectlombok:lombok'
	providedRuntime 'org.springframework.boot:spring-boot-starter-tomcat'
	testImplementation 'org.springframework.boot:spring-boot-starter-test'
}

tasks.named('test') {
	useJUnitPlatform()
}

```
μ°Έκ³  
- Settings | File | Settings | Build, Execution, Deployment | Build Tools | Gradle
-> Build and run using, Run test using : IntelliJ IDEA μ€μ μ μ€ν μλκ° ν₯μλ©λλ€.
- Lombok λΌμ΄λΈλ¬λ¦¬ μΆκ°
  - File | Settings | Plugins | Marketplace μμ lombok μΆκ°
- File | Settings | Build, Execution, Deployment | Compiler | Annotation Processors
  - Enable annotaition processing μ²΄ν¬ ν΄μΌ λ‘¬λ³΅μ΄ λμν©λλ€.
  
λμ νμΈ - main() μ€ν
```
Tomcat started on port(s): 8080 (http) with context path ''
```
![localhost:8080](https://images.velog.io/images/urtimeislimited/post/4e7a7094-07c0-411c-bcf6-c02949f3c3cb/image.png)

[POSTMAN μ€μΉ](https://www.postman.com/downloads/)
API νΈμΆμ μν΄ μ€μΉν©λλ€.

#### Hello μλΈλ¦Ώ
μλΈλ¦Ώμ ν°μΊ£ κ°μ μΉ μ νλ¦¬μΌμ΄μ μλ²λ₯Ό μ§μ  μ€μΉνκ³ ,κ·Έ μμ μλΈλ¦Ώ μ½λλ₯Ό ν΄λμ€ νμΌλ‘ λΉλν΄μ μ¬λ¦° λ€μ, ν°μΊ£ μλ²λ₯Ό μ€ννλ©΄ λ©λλ€. νμ§λ§ μ΄ κ³Όμ μ λ§€μ° λ²κ±°λ‘­κΈ° λλ¬Έμ ν°μΊ£ μλ²λ₯Ό λ΄μ₯νκ³ , ν°μΊ£ μλ² μ€μΉ μμ΄ νΈλ¦¬νκ² μλΈλ¦Ώ μ½λλ₯Ό μ€νν  μ μλ μ€νλ§ λΆνΈ νκ²½μμ μλΈλ¦Ώμ λ±λ‘νκ³  μ¬μ©ν΄λ³΄κ² μ΅λλ€.

```java
@WebServlet(name = "helloServlet", urlPatterns = "/hello")
public class HelloServlet extends HttpServlet {
    @Override
    protected void service(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {

        System.out.println("HelloServlet.service");
        System.out.println("request = " + request);
        System.out.println("response = " + response);

        String username = request.getParameter("username");
        System.out.println("username = " + username);

        response.setContentType("text/plain");
        response.setCharacterEncoding("utf-8"); // κΆμ₯
        response.getWriter().write("hello " + username); 
    }
}
```
- @ServletComponentScan : μ€νλ§μ΄ ν΄λΉ ν¨ν€μ§μ νμ ν¨ν€μ§λ₯Ό μλ νμν΄μ μλΈλ¦Ώ λ±λ‘μ μ§μν΄μ£Όλ μ΄λΈνμ΄μ
- HttpServlet : HttpServletμ μμλ°μ΅λλ€.
- @WebServlet(μλΈλ¦Ώ μ΄λΈνμ΄μ) : urlPatternsλ‘ μ λ¬λ°λ νλΌλ―Έν°μ μΌμΉνλ ν΄λμ€λ₯Ό μ€νν΄μ€λλ€.
  - name: μλΈλ¦Ώ μ΄λ¦
  - urlPatterns: URL λ§€ν
  - μ€λ³΅λλ©΄ μ λ©λλ€.
- setContentType : HTTP ν€λμ λ€μ΄κ°λ μ λ³΄
- setCharacterEncoding : HTTP λ°λμ λ€μ΄κ°λ μ λ³΄
>- http://localhost:8080/hello μ½μ μ€νκ²°κ³Ό
HelloServlet.service
request = org.apache.catalina.connector.RequestFacade@51d0e482
response = org.apache.catalina.connector.ResponseFacade@65964004
>- http://localhost:8080/hello?username=kim μ½μ μ€νκ²°κ³Ό
username = kim
>- λΈλΌμ°μ  νλ©΄ 
![hellokim](https://images.velog.io/images/urtimeislimited/post/f76914e8-e514-4937-b90c-d4171026230e/image.png)
![content-type](https://images.velog.io/images/urtimeislimited/post/b9f0cf59-8815-4054-9ef7-67a48788cbef/image.png)

HttpServletRequest, HttpServletResponseμ μΈν°νμ΄μ€μλλ€.
ν°μΊ£ λ±λ± μ¬λ¬ WAS μλ²μ νμ€ μ€νμ κ΅¬νν κ²°κ³Όλ₯Ό νΈμΆνκ² λ©λλ€.
λ§μ½ HTTP λ©μμ§λ₯Ό μΌμΌν νμ±ν΄μ μ½μΌλ €λ©΄ κ΅μ₯ν λ²κ±°λ‘­μ΅λλ€.
μλΈλ¦Ώμ μ΄λ¬ν λ²κ±°λ‘μμ νΈλ¦¬νκ² μ¬μ©νλλ‘ λμμ€λλ€.

HTTP μμ²­μ΄ μ€λ©΄, λ§€νλ URLμ΄ νΈμΆλλ©΄μ μλΈλ¦Ώ μ»¨νμ΄λλ ν΄λΉ λ©μλλ₯Ό μ€νν©λλ€.

#### HTTP μμ²­ λ©μμ§ νμΈνκΈ°

application.propertiesμ λ€μ μ€μ μ μΆκ°νλ©΄ μμ²­ λ©μμ§κ° μ΄λ»κ² μλμ§ νμΈν  μ μμ΅λλ€.

μμ²­ λ©μμ§ μ λ³΄
![μμ²­ λ©μμ§ μ λ³΄](https://images.velog.io/images/urtimeislimited/post/30b163ed-484d-40e2-ab0a-7b24267ce65a/image.png)
ν€λ μ λ³΄..
![ν€λ μ λ³΄](https://images.velog.io/images/urtimeislimited/post/18292fec-41fc-464e-8deb-ea17891e3329/image.png)
```java
logging.level.org.apache.coyote.http11=debug
```

- μ°Έκ³  : μ΄μμλ²μ λͺ¨λ  μμ²­ μ λ³΄λ₯Ό λ¨κΈ°λ κ²μ μ±λ₯ μ νκ° λ°μν  μ μκΈ° λλ¬Έμ κ³ λ €ν΄μΌν©λλ€. κ°λ° λ¨κ³μμλ§ μ μ©ν  κ²μ κΆμ₯ν©λλ€.

#### μλΈλ¦Ώ μ»¨νμ΄λ λμ λ°©μ
1. μ€νλ§ λΆνΈλ₯Ό ν΅ν΄ λ΄μ₯ ν°μΊ£ μλ²λ₯Ό λμμν΅λλ€.
2. μλΈλ¦Ώ μ»¨νμ΄λλ₯Ό ν¬ν¨μν¨ ν°μΊ£ μλ²μ λ΄λΆλ helloServletμ΄λΌλ μλΈλ¦Ώμ μμ±ν©λλ€.
![λ΄μ₯ ν°μΊ£ μλ² μμ±](https://images.velog.io/images/urtimeislimited/post/b68d2744-ef81-4039-bba9-317f967437f3/image.png)
3. μΉ λΈλΌμ°μ κ° HTTP μμ²­ λ©μμ§λ₯Ό μμ±νμ¬ μ λ¬ν©λλ€.
4. μλ²λ μ λ¬λ°μ HTTP μμ²­ λ©μμ§λ₯Ό κΈ°λ°μΌλ‘ request, response κ°μ²΄λ₯Ό μμ±ν΄μ μ±κΈν€ ννμ helloServletμ νΈμΆν΄μ€λλ€.
5. νλΌλ―Έν°κ° μΌμΉνλ ν΄λΉ λ©μλμ HTTP λ©νλ°μ΄ν°κ° ν¬ν¨λμ΄μλ request, response κ°μ²΄λ₯Ό μ λ¬νλ©΄ λ΄λΆ μμμ μ²λ¦¬ν©λλ€.
6. μμμ΄ μ’λ£λλ©΄ WAS μλ²κ° response κ°μ²΄ μ λ³΄λ₯Ό κΈ°λ°μΌλ‘ HTTP μλ΅ λ©μμ§λ₯Ό μμ±νκ³  λ°νν©λλ€.
7. μλ΅ λ°μ κ²°κ³Όλ₯Ό μΉ λΈλΌμ°μ μμ νμΈν  μ μμ΅λλ€.
![HTTP μμ²­, HTTP μλ΅ λ©μμ§](https://images.velog.io/images/urtimeislimited/post/7faea610-081c-4fbf-b281-9cba5d5018ce/image.png)


- μ°Έκ³  : HTTP μλ΅μμ μ Content-Lengthκ°μ λΆκ° μ λ³΄λ€μ WASκ° μλμΌλ‘ μμ±ν΄μ€λλ€.

welcomPage (localhost:8080 νΈμΆμ κΈ°λ³Έ νμ΄μ§)
main/webapp/index.html
```html
<!DOCTYPE html>
<html>
<head>
 <meta charset="UTF-8">
 <title>Title</title>
</head>
<body>
<ul>
 <li><a href="basic.html">μλΈλ¦Ώ basic</a></li>
</ul>
</body>
</html>
```
![index.html](https://images.velog.io/images/urtimeislimited/post/f67e6e0e-209d-4606-b506-0717be4bfcf1/image.png)
main/webapp/basic.html
```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>Title</title>
</head>
<body>
<ul>
    <li>hello μλΈλ¦Ώ
        <ul>
            <li><a href="/hello?username=servlet">hello μλΈλ¦Ώ νΈμΆ</a></li>
        </ul>
    </li>
    <li>HttpServletRequest
        <ul>
            <li><a href="/request-header">κΈ°λ³Έ μ¬μ©λ², Header μ‘°ν</a></li>
            <li>HTTP μμ²­ λ©μμ§ λ°λ μ‘°ν
                <ul>
                    <li><a href="/request-param?username=hello&age=20">GET -
                        μΏΌλ¦¬ νλΌλ―Έν°</a></li>
                    <li><a href="/basic/hello-form.html">POST - HTML Form</a></li>
                    <li>HTTP API - MessageBody -> Postman νμ€νΈ</li>
                </ul>
            </li>
        </ul>
    </li>
    <li>HttpServletResponse
        <ul>
            <li><a href="/response-header">κΈ°λ³Έ μ¬μ©λ², Header μ‘°ν</a></li>
            <li>HTTP μλ΅ λ©μμ§ λ°λ μ‘°ν
                <ul>
                    <li><a href="/response-html">HTML μλ΅</a></li>
                    <li><a href="/response-json">HTTP API JSON μλ΅</a></li>
                </ul>
            </li>
        </ul>
    </li>
</ul>
</body>
</html>
```
![basic.html](https://images.velog.io/images/urtimeislimited/post/fab9af34-a50a-48dd-ad28-f666306dc82e/image.png)

#### HttpServletRequest κ°μ

__HttpServletRequest μ­ν __
HTTP μμ²­ λ©μμ§λ₯Ό κ°λ°μκ° μ§μ  νμ±ν΄μ μ¬μ©ν΄λ λμ§λ§, λ§€μ° λΆνΈν  κ²μλλ€. μλΈλ¦Ώμ κ°λ°μκ° HTTP μμ²­ λ©μμ§λ₯Ό νΈλ¦¬νκ² μ¬μ©ν  μ μλλ‘ κ°λ°μ λμ μ HTTP μμ²­ λ©μμ§λ₯Ό νμ±νκ³  κ·Έ κ²°κ³Όλ₯Ό HttpServletRequest κ°μ²΄μ λ΄μμ μ κ³΅ν©λλ€.

HttpServletRequestλ₯Ό μ¬μ©νλ©΄ λ€μκ³Ό κ°μ HTTP μμ²­ λ©μμ§λ₯Ό νΈλ¦¬νκ² μ‘°νν  μ μμ΅λλ€.
![HTTP μμ²­ λ©μμ§](https://images.velog.io/images/urtimeislimited/post/562c88be-9e0c-42e8-b27b-0b4044d0b9ca/image.png)

- START LINE
  - HTTP λ©μλ
  - URL
  - μΏΌλ¦¬ μ€νΈλ§
  - μ€ν€λ§, νλ‘ν μ½
- ν€λ
  - ν€λ μ‘°ν
- λ°λ
  - form νλΌλ―Έν° νμ μ‘°ν
  - message body λ°μ΄ν° μ§μ  μ‘°ν
  
HttpServletRequest κ°μ²΄λ μΆκ°λ‘ μ¬λ¬κ°μ§ λΆκ°κΈ°λ₯λ ν¨κ» μ κ³΅ν©λλ€.

μμ μ μ₯μ κΈ°λ₯
- ν΄λΉ HTTP μμ²­ μλͺμ£ΌκΈ° λμ(μμλΆν° λλ  λ κΉμ§) μ μ§λλ μμ μ μ₯μ κΈ°λ₯
  - μ μ₯: request.setAttribute(name, value)
  - μ‘°ν: request.getAttribute(name)
μΈμ κ΄λ¦¬ κΈ°λ₯
- request.getSession(create: true)
> μ€μ
> HttpServletRequest, HttpServletResponseλ₯Ό μ¬μ©ν  λ κ°μ₯ μ€μν μ μ μ΄ __κ°μ²΄λ€μ΄ HTTP μμ²­
λ©μμ§, HTTP μλ΅ λ©μμ§λ₯Ό νΈλ¦¬νκ² μ¬μ©νλλ‘ λμμ£Όλ κ°μ²΄λΌλ μ __μλλ€. λ°λΌμ μ΄ κΈ°λ₯μ λν΄μ
κΉμ΄μλ μ΄ν΄λ₯Ό νλ €λ©΄ __HTTP μ€νμ΄ μ κ³΅νλ μμ²­, μλ΅ λ©μμ§ μμ²΄λ₯Ό μ΄ν΄__ν΄μΌ ν©λλ€.

#### HttpServletRequest - κΈ°λ³Έ μ¬μ©λ²

```java
@WebServlet(name = "requestHeaderServlet", urlPatterns = "/request-header")
public class RequestHeaderServlet extends HttpServlet {
    @Override
    protected void service(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        printStartLine(request);
    }

    private void printStartLine(HttpServletRequest request) {
        System.out.println("--- REQUEST-LINE - start ---");
        System.out.println("request.getMethod() = " + request.getMethod()); //GET
        System.out.println("request.getProtocal() = " + request.getProtocol()); //HTTP/1.1
        System.out.println("request.getScheme() = " + request.getScheme()); //http
        // http://localhost:8080/request-header
        System.out.println("request.getRequestURL() = " + request.getRequestURL());
        // /request-test
        System.out.println("request.getRequestURI() = " + request.getRequestURI());
        //username=hi
        System.out.println("request.getQueryString() = " +
                request.getQueryString());
        System.out.println("request.isSecure() = " + request.isSecure()); //httpsμ¬μ© μ λ¬΄
        System.out.println("--- REQUEST-LINE - end ---");
        System.out.println();
    }
}
```
- μ°Έκ³  : Ctrl+Alt+M(Windows/Linux) -> ExtractMethod λ©μλ μΆμΆ

> μ½μ μ€ν κ²°κ³Ό
--- REQUEST-LINE - start ---
request.getMethod() = GET
request.getProtocal() = HTTP/1.1
request.getScheme() = http
request.getRequestURL() = http://localhost:8080/request-header
request.getRequestURI() = /request-header
request.getQueryString() = null
request.isSecure() = false // https or http μ¬λΆ
--- REQUEST-LINE - end ---

ν€λ μ λ³΄ λΆλ¬μ€λ κ³Όκ±° λ°©λ²
``` java
//Header λͺ¨λ  μ λ³΄
    private void printHeaders(HttpServletRequest request) {
        System.out.println("--- Headers - start ---");

         Enumeration<String> headerNames = request.getHeaderNames(); // λ°©λ²1
         while (headerNames.hasMoreElements()) {
         String headerName = headerNames.nextElement();
         System.out.println(headerName + ": " + request.getHeader(headerName));
         }

        System.out.println("--- Headers - end ---");
        System.out.println();
    }
```
getHeaderNamesλ₯Ό EnumerationμΌλ‘ whileλ¬ΈμΌλ‘
μμκ° μμΌλ©΄ λ€μ μμ λ°ννλ λ°λ³΅λ¬Έμ νμμλλ€.
```java
printHeaders(request);
```
> μ½μ μ€ν κ²°κ³Ό
--- Headers - start ---
host: localhost:8080
connection: keep-alive
cache-control: max-age=0
sec-ch-ua: " Not A;Brand";v="99", "Chromium";v="98", "Google Chrome";v="98"
sec-ch-ua-mobile: ?0
sec-ch-ua-platform: "Windows"
upgrade-insecure-requests: 1
user-agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/98.0.4758.102 Safari/537.36
accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9
sec-fetch-site: none
sec-fetch-mode: navigate
sec-fetch-user: ?1
sec-fetch-dest: document
accept-encoding: gzip, deflate, br
accept-language: ko-KR,ko;q=0.9,en-US;q=0.8,en;q=0.7,ja;q=0.6
--- Headers - end ---

κ°κ²°ν λ¬Έλ²μΌλ‘ λ¦¬ν©ν λ§ν΄λ κ²°κ³Όλ κ°μ΅λλ€.
```java
request.getHeaderNames().asIterator()
                .forEachRemaining(headerName -> System.out.println(headerName + ": " + request.getHeader(headerName)));
                //request.getHeader("ν€λλͺ"); // νΉμ  ν€λλ§ μ‘°ν
                        System.out.println("--- Headers - end ---");
        System.out.println();
```

μ’ λ νΈλ¦¬νκ² μ‘°νν΄λ³΄κ² μ΅λλ€.
```java
//Header νΈλ¦¬ν μ‘°ν
    private void printHeaderUtils(HttpServletRequest request) {
        System.out.println("--- Header νΈμ μ‘°ν start ---");
        System.out.println("[Host νΈμ μ‘°ν]");
        System.out.println("request.getServerName() = " +
                request.getServerName()); //Host ν€λ
        System.out.println("request.getServerPort() = " +
                request.getServerPort()); //Host ν€λ
        System.out.println();
        System.out.println("[Accept-Language νΈμ μ‘°ν]");
        request.getLocales().asIterator()
                .forEachRemaining(locale -> System.out.println("locale = " +
                        locale));
        System.out.println("request.getLocale() = " + request.getLocale());
        System.out.println();
        System.out.println("[cookie νΈμ μ‘°ν]");
        if (request.getCookies() != null) {
            for (Cookie cookie : request.getCookies()) {
                System.out.println(cookie.getName() + ": " + cookie.getValue());
            }
        }
        System.out.println();
        System.out.println("[Content νΈμ μ‘°ν]");
        System.out.println("request.getContentType() = " +
                request.getContentType());
        System.out.println("request.getContentLength() = " +
                request.getContentLength());
        System.out.println("request.getCharacterEncoding() = " +
                request.getCharacterEncoding());
        System.out.println("--- Header νΈμ μ‘°ν end ---");
        System.out.println();
    }
```
> μ½μ μ€ν κ²°κ³Ό
--- Header νΈμ μ‘°ν start ---
[Host νΈμ μ‘°ν]
request.getServerName() = localhost
request.getServerPort() = 8080
>[Accept-Language νΈμ μ‘°ν]
locale = ko_KR
locale = ko
locale = en_US
locale = en
locale = ja
request.getLocale() = ko_KR
>[cookie νΈμ μ‘°ν]
>[Content νΈμ μ‘°ν]
request.getContentType() = null
request.getContentLength() = -1
request.getCharacterEncoding() = UTF-8
--- Header νΈμ μ‘°ν end ---

- getServerName : μλ² μ λ³΄ μ‘°ν
- getServerPort : ν¬νΈ μ λ³΄ μ‘°ν
μ) Host: localhost:8080
- getLocale : κ°μ₯ μ°μ μμλ‘ μ§μνλ μΈμ΄λ₯Ό νΈμΆν©λλ€.
μ) Accept-Language: ko-KR,ko;q=0.9,en-US;q=0.8,en;q=0.7,ja;q=0.6
- getCookies : μΏ ν€ μ λ³΄λ₯Ό μ‘°νν΄μ ν€λμ ν¬ν¨ν©λλ€.
- getContentType, getContentLength, getCharacterEncoding
  - getμ΄κΈ° λλ¬Έμ null μΆλ ₯, POSTMANμΌλ‘ κ°λ¨ν λ°μ΄ν°(hello!)λ₯Ό POSTν΄λ³΄λ©΄
  >
request.getContentType() = application/json
request.getContentLength() = 6
request.getCharacterEncoding() = UTF-8

κΈ°ν μ λ³΄ μ‘°ν
```java
private void printEtc(HttpServletRequest request) {
        System.out.println("--- κΈ°ν μ‘°ν start ---");
        System.out.println("[Remote μ λ³΄]");
        System.out.println("request.getRemoteHost() = " +
                request.getRemoteHost()); //
        System.out.println("request.getRemoteAddr() = " +
                request.getRemoteAddr()); //
        System.out.println("request.getRemotePort() = " +
                request.getRemotePort()); //
        System.out.println();
        System.out.println("[Local μ λ³΄]");
        System.out.println("request.getLocalName() = " +
                request.getLocalName()); //
        System.out.println("request.getLocalAddr() = " +
                request.getLocalAddr()); //
        System.out.println("request.getLocalPort() = " +
                request.getLocalPort()); //
        System.out.println("--- κΈ°ν μ‘°ν end ---");
        System.out.println();
    }
    @Override
    protected void service(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        printEtc(request);
    }
```
> μ½μ μ€ν κ²°κ³Ό
--- κΈ°ν μ‘°ν start ---
[Remote μ λ³΄] // μμ²­μ λν μ λ³΄
request.getRemoteHost() = 0:0:0:0:0:0:0:1
request.getRemoteAddr() = 0:0:0:0:0:0:0:1
request.getRemotePort() = 9322
[Local μ λ³΄] // νμ¬ λμ μλ² μ λ³΄
request.getLocalName() = 0:0:0:0:0:0:0:1
request.getLocalAddr() = 0:0:0:0:0:0:0:1
request.getLocalPort() = 8080
--- κΈ°ν μ‘°ν end ---

- μ°Έκ³ 
  - λ‘μ»¬μμ νμ€νΈνλ©΄ IPv6 μ λ³΄κ° λμ€λλ°, IPv4 μ λ³΄λ₯Ό λ³΄κ³  μΆμΌλ©΄ λ€μ μ΅μμ VM optionsμ λ£μ΄μ£Όλ©΄ λ©λλ€.
``` -Djava.net.preferIPv4Stack=true ```

μ§κΈκΉμ§ HttpServletRequestλ₯Ό ν΅ν΄μ HTTP λ©μμ§μ start-line, header μ λ³΄ μ‘°ν λ°©λ²μ
μ΄ν΄νμ΅λλ€. μ΄μ  λ³Έκ²©μ μΌλ‘ HTTP μμ²­ λ°μ΄ν°λ₯Ό μ΄λ»κ² μ‘°ννλμ§ μμλ³΄κ² μ΅λλ€.

#### HTTP μμ²­ λ°μ΄ν°
HTTP μμ²­ λ©μμ§λ₯Ό ν΅ν΄ ν΄λΌμ΄μΈνΈμμ μλ²λ‘ λ°μ΄ν°λ₯Ό μ λ¬νλ λ°©λ²μ μ£Όλ‘ λ€μ 3κ°μ§ λ°©λ²μ μ¬μ©ν©λλ€.

- __GET - μΏΌλ¦¬ νλΌλ―Έν°__
  - /url**?username=hello&age=20**
  - λ©μμ§ λ°λ μμ΄, URLμ μΏΌλ¦¬ νλΌλ―Έν°μ λ°μ΄ν°λ₯Ό ν¬ν¨ν΄μ μ λ¬ν©λλ€.
  - μ) κ²μ, νν°, νμ΄μ§λ±μμ λ§μ΄ μ¬μ©νλ λ°©μ
- __POST - HTML Form__
  - content-type: application/x-www-form-urlencoded
  - λ©μμ§ λ°λμ μΏΌλ¦¬ νλ¦¬λ―Έν° νμμΌλ‘ μ λ¬ν©λλ€.
    - username=hello&age=20κ°μ νμκ³Ό νΈνλ©λλ€.
  - μ) νμ κ°μ, μν μ£Όλ¬Έ, HTML Form μ¬μ©
  ![POST - HTML Form](https://images.velog.io/images/urtimeislimited/post/8b0ee59e-64e2-48e1-b398-c3c51aa16d27/image.png)
- __HTTP message body__μ λ°μ΄ν°λ₯Ό μ§μ  λ΄μμ μμ²­
  -HTTP APIμμ μ£Όλ‘ μ¬μ©, JSON, XML, TEXT
- λ°μ΄ν° νμμ μ£Όλ‘ JSON μ¬μ©
  - POST, PUT, PATCH
  
#### HTTP μμ²­ λ°μ΄ν° - GET μΏΌλ¦¬ νλΌλ―Έν°
λ€μ λ°μ΄ν°λ₯Ό ν΄λΌμ΄μΈνΈμμ μλ²λ‘ μ μ‘ν΄λ³΄κ² μ΅λλ€.
λ©μμ§ λ°λ μμ΄, URLμ __μΏΌλ¦¬ νλΌλ―Έν°__λ₯Ό μ¬μ©ν΄μ λ°μ΄ν°λ₯Ό μ λ¬νκ² μ΅λλ€. 
μ) κ²μ, νν°, νμ΄μ§ λ±μμ λ§μ΄ μ¬μ©νλ λ°©μμλλ€.

- μ λ¬ λ°μ΄ν°
  - username=hello
  - age=20
- URL
  - μΏΌλ¦¬ νλΌλ―Έν°λ URLμ λ€μκ³Ό κ°μ΄ ? λ₯Ό μμμΌλ‘ λ³΄λΌ μ μμΌλ©° μΆκ° νλΌλ―Έν°λ & λ‘ κ΅¬λΆνλ©΄ λ©λλ€.
  - http://localhost:8080/request-param?username=hello&age=20
  
μλ²μμλ HttpServletRequest κ° μ κ³΅νλ λ€μ λ©μλλ₯Ό ν΅ν΄ μΏΌλ¦¬ νλΌλ―Έν°λ₯Ό νΈλ¦¬νκ² μ‘°νν  μμμ΅λλ€.
``` java
String username = request.getParameter("username"); //λ¨μΌ νλΌλ―Έν° μ‘°ν
Enumeration<String> parameterNames = request.getParameterNames(); //νλΌλ―Έν° μ΄λ¦λ€ λͺ¨λ μ‘°ν
Map<String, String[]> parameterMap = request.getParameterMap(); //νλΌλ―Έν°λ₯Ό Map μΌλ‘ μ‘°ν
String[] usernames = request.getParameterValues("username"); //λ³΅μ νλΌλ―Έν° μ‘°ν
```

``` java
/**
 * 1. νλΌλ―Έν° μ μ‘ κΈ°λ₯
 * http://localhost:8080/request-param?username=hello&age=20
 * <p>
 * 2. λμΌν νλΌλ―Έν° μ μ‘ κ°λ₯
 * http://localhost:8080/request-param?username=hello&username=kim&age=20
 */
@WebServlet(name = "requesetParamServlet", urlPatterns = "/request-param")
public class RequesetParamServlet extends HttpServlet {

    @Override
    protected void service(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        System.out.println("RequesetParamServlet.service");
        System.out.println("[μ μ²΄ νλΌλ―Έν°] - start");
        request.getParameterNames().asIterator()
                .forEachRemaining(paramName -> System.out.println(paramName+ " =" + request.getParameter(paramName)));
        System.out.println("[μ μ²΄ νλΌλ―Έν°] - end");
        System.out.println();

        System.out.println("[λ¨μΌ νλΌλ―Έν° μ‘°ν]");
        String username = request.getParameter("username");
        System.out.println("username = " + username);
        String age = request.getParameter("age");
        System.out.println("age = " + age);

        System.out.println("[μ΄λ¦μ΄ κ°μ λ³΅μ νλΌλ―Έν° μ‘°ν]");
        String[] usernames = request.getParameterValues("username");
        for (String name : usernames) {
            System.out.println("username = " + name);
        }
        response.getWriter().write("ok");
    }
}
```

**λ³΅μ νλΌλ―Έν°μμ λ¨μΌ νλΌλ―Έν° μ‘°ν**
username=hello&username=kim κ³Ό κ°μ΄ νλΌλ―Έν° μ΄λ¦μ νλμΈλ° κ°μ΄ μ€λ³΅μ΄λΌλ©΄?

request.getParameter() λ νλμ νλΌλ―Έν° μ΄λ¦μ λν΄μ λ¨ νλμ κ°λ§ μμ λ μ¬μ©ν΄μΌ νκΈ° λλ¬Έμ μ§κΈμ²λΌ μ€λ³΅μΌ λλ request.getParameterValues() λ₯Ό μ¬μ©ν΄μΌ ν©λλ€.

μ°Έκ³ λ‘ μ΄λ κ² μ€λ³΅μΌ λ request.getParameter() λ₯Ό μ¬μ©νλ©΄ request.getParameterValues() μ μ²« λ²μ§Έ κ°μ λ°νν©λλ€.
μ€λ¬΄μμλ **request.getParameter()**λ₯Ό κ°μ₯ λ§μ΄ μ¬μ©νλ€κ³  ν©λλ€.

#### HTTP μμ²­ λ°μ΄ν° - POST HTML Form

HTMLμ Formμ μ¬μ©ν΄μ ν΄λΌμ΄μΈνΈμμ μλ²λ‘ λ°μ΄ν°λ₯Ό μ μ‘ν΄λ³΄κ² μ΅λλ€. μ£Όλ‘ νμ κ°μ, μν μ£Όλ¬Έ λ±μμ μ¬μ©νλ λ°©μμλλ€.
- νΉμ§
  - content-type: application/x-www-form-urlencoded
  - λ©μμ§ λ°λμ μΏΌλ¦¬ νλ¦¬λ―Έν° νμμΌλ‘ λ°μ΄ν°λ₯Ό μ λ¬ν©λλ€.     
    - username=hello&age=20
    
src/main/webapp/basic/hello-form.html μμ±
```html
<!DOCTYPE html>
<html>
<head>
 <meta charset="UTF-8">
 <title>Title</title>
</head>
<body>
<form action="/request-param" method="post">
 username: <input type="text" name="username" />
 age: <input type="text" name="age" />
 <button type="submit">μ μ‘</button>
</form>
</body>
</html>
```

http://localhost:8080/basic/hello-form.html
![hello-form.html](https://images.velog.io/images/urtimeislimited/post/93598eab-17ca-4bca-ad64-78ac1283a126/image.png)
POSTμ HTML Formμ μ μ‘νλ©΄ μΉ λΈλΌμ°μ λ λ€μ νμμΌλ‘ HTTP λ©μμ§λ₯Ό λ§λ­λλ€. (μΉ λΈλΌμ°μ  κ°λ°μ λͺ¨λ νμΈ)
- μμ²­ URL: http://localhost:8080/request-param
- content-type: application/x-www-form-urlencoded
- message body: username=hello&age=20

application/x-www-form-urlencoded νμμ μμ **GETμμ μ΄ν΄λ³Έ μΏΌλ¦¬ νλΌλ―Έν° νμκ³Ό κ°μ΅λλ€.** 
λ°λΌμ **μΏΌλ¦¬ νλΌλ―Έν° μ‘°ν λ©μλλ₯Ό κ·Έλλ‘ μ¬μ©**νλ©΄ λ©λλ€.
ν΄λΌμ΄μΈνΈ(μΉ λΈλΌμ°μ ) μμ₯μμλ λ λ°©μμ μ°¨μ΄κ° μμ§λ§, μλ² μμ₯μμλ λμ νμμ΄ λμΌνλ―λ‘, **request.getParameter() λ‘ νΈλ¦¬νκ² κ΅¬λΆμμ΄ μ‘°ν**ν  μ μμ΅λλ€.

μ¦, **request.getParameter() λ GET URL μΏΌλ¦¬ νλΌλ―Έν° νμλ μ§μνκ³ , POST HTML Form νμλ λ λ€ μ§μν©λλ€.**

- μ°Έκ³  : content-typeμ HTTP λ©μμ§ λ°λμ λ°μ΄ν° νμμ μ§μ ν©λλ€. GET URL μΏΌλ¦¬ νλΌλ―Έν° νμμΌλ‘ ν΄λΌμ΄μΈνΈμμ μλ²λ‘ λ°μ΄ν°λ₯Ό μ λ¬ν  λλ HTTP λ©μμ§ λ°λλ₯Ό μ¬μ©νμ§ μκΈ° λλ¬Έμ content-typeμ΄ μμ΅λλ€.
 POST HTML Form νμμΌλ‘ λ°μ΄ν°λ₯Ό μ λ¬νλ©΄ HTTP λ©μμ§ λ°λμ ν΄λΉ λ°μ΄ν°λ₯Ό ν¬ν¨ν΄μ λ³΄λ΄κΈ° λλ¬Έμ λ°λμ ν¬ν¨λ λ°μ΄ν°κ° μ΄λ€ νμμΈμ§ content-typeμ κΌ­ μ§μ ν΄μΌ ν©λλ€. μ΄λ κ² νΌμΌλ‘ λ°μ΄ν°λ₯Ό
μ μ‘νλ νμμ application/x-www-form-urlencoded λΌ ν©λλ€.

μ΄λ° κ°λ¨ν νμ€νΈμ HTML formμ λ§λ€κΈ°λ κ·μ°?λ€λ©΄ Postmanμ μ¬μ©νλ©΄ λ©λλ€.

- Postman νμ€νΈ μ£Όμμ¬ν­
  - POST μ μ‘μ
    - Body x-www-form-urlencoded μ ν
    - Headersμμ content-type: application/x-www-form-urlencoded λ‘ μ§μ λ λΆλΆ κΌ­ νμΈ
    
![Postman](https://images.velog.io/images/urtimeislimited/post/faa09bf0-0c5c-495c-bc87-f1031c72b249/image.png)

#### HTTP μμ²­ λ°μ΄ν° - API λ©μμ§ λ°λ - λ¨μ νμ€νΈ
- HTTP message bodyμ λ°μ΄ν°λ₯Ό μ§μ  λ΄μμ μμ²­νλ λ°©μμλλ€.
  - HTTP APIμμ μ£Όλ‘ JSON, XML, TEXT μ¬μ©ν©λλ€.
  - λ°μ΄ν° νμμ μ£Όλ‘ JSON μ¬μ©ν©λλ€.
  - POST, PUT, PATCH
  
HTTP λ©μμ§ λ°λμ λ°μ΄ν°λ₯Ό InputStreamμ μ¬μ©ν΄μ μ§μ  μ½μ μ μμ΅λλ€. λ¨Όμ  κ°μ₯ λ¨μν νμ€νΈ λ©μμ§λ₯Ό HTTP λ©μμ§ λ°λμ λ΄μμ μ μ‘νκ³ , μ½μ΄λ³΄κ² μ΅λλ€.

```java
@WebServlet(name = "requestBodyStringServlet", urlPatterns = "/request-body-string")
public class RequestBodyStringServlet extends HttpServlet{
    @Override
    protected void service(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        ServletInputStream inputStream = request.getInputStream(); // λ©μμ§ λ°λμ λ΄μ©μ λ°μ΄νΈμ½λλ‘ λ°λ‘ μ»μ μ μμ
        String messageBody = StreamUtils.copyToString(inputStream, StandardCharsets.UTF_8);// StreamUtils: λ°μ΄νΈμ½λλ₯Ό λ¬ΈμνμΌλ‘ λ³ν
        System.out.println("messageBody = " + messageBody);
        response.getWriter().write("ok");

    }
}
```
- inputStreamμ byte μ½λλ₯Ό λ°νν©λλ€. byte μ½λλ₯Ό μ°λ¦¬κ° μ½μ μ μλ λ¬Έμ(String)λ‘ λ³΄λ €λ©΄ λ¬Έμν (Charset)λ₯Ό μ§μ ν΄μ£Όμ΄μΌ ν©λλ€. μΌλ°μ μΈ UTF_8 Charsetμ μ§μ ν΄μ£Όμμ΅λλ€.
![requesetString](https://images.velog.io/images/urtimeislimited/post/4d509f3f-4a70-4cc4-9395-2835f0d09b74/image.png)
> μ½μ μ€νκ²°κ³Ό
```messageBody = hello!```

#### HTTP μμ²­ λ°μ΄ν° - API λ©μμ§ λ°λ - JSON
 HTTP APIμμ μ£Όλ‘ μ¬μ©νλ JSON νμμΌλ‘ λ°μ΄ν°λ₯Ό μ λ¬ν΄λ³΄κ² μ΅λλ€.

JSON νμ μ μ‘
- POST http://localhost:8080/request-body-json
- content-type: application/json
- message body: {"username": "hello", "age": 20}
- κ²°κ³Ό: messageBody = {"username": "hello", "age": 20}

JSON λ°μ΄ν°λ λ³΄ν΅ κ·Έλλ‘ μ¬μ©νμ§ μκ³  κ°μ²΄λ‘ λ³ννμ¬ μ¬μ©ν©λλ€. JSON νμμΌλ‘ νμ±ν  μ μλλ‘ κ°μ²΄λ₯Ό λ¨Όμ  μμ±ν©λλ€.

hello.servlet.basic;
```java
@Getter @Setter
public class HelloData {
    private String username;
    private int age;
}
```
- μ°Έκ³ : lombokμ΄ μ κ³΅νλ @Getter , @Setter λλΆμ λ€μ μ½λκ° μλμΌλ‘ μΆκ°λ©λλ€.(λμ λ³΄μ΄μ§λ μμ΅λλ€.)
```java
 //==== lombok μμ± μ½λ ====//
 public String getUsername() {
 return username;
 }
 public void setUsername(String username) {
 this.username = username;
 }
 public int getAge() {
 return age;
 }
 public void setAge(int age) {
 this.age = age;
 }
```
```java
@WebServlet(name = "requestBodyJsonServlet", urlPatterns = "/request-body-json")
public class RequestBodyJsonServlet extends HttpServlet {
    @Override
    protected void service(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        ServletInputStream inputStream = request.getInputStream();
        String messageBody = StreamUtils.copyToString(inputStream, StandardCharsets.UTF_8);

        System.out.println("messageBody = " + messageBody);
    }
}
```
POSTMAN : Body - raw - JSON
```{"username": "hello!", "age": 20}```
![headerConvertoJson](https://images.velog.io/images/urtimeislimited/post/4efc82fb-f626-43ce-9a07-8465d20f5776/image.png)

> μ½μ μ€νκ²°κ³Ό
```messageBody = {username: "hello!", age: 20}```

μ€νλ§μ΄ κ°μ§κ³ μλ jackson λΌμ΄λΈλ¬λ¦¬λ₯Ό ν΅ν΄ JSON λ°μ΄ν°λ₯Ό κ°μ²΄λ‘ λ³νν  μλ μμ΅λλ€.
![jackson](https://images.velog.io/images/urtimeislimited/post/d1856892-273d-4e20-aede-78a81600b812/image.png)
```java
	    private ObjectMapper objectMapper = new ObjectMapper();

    @Override
    protected void service(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        ServletInputStream inputStream = request.getInputStream();
        String messageBody = StreamUtils.copyToString(inputStream, StandardCharsets.UTF_8);

        System.out.println("messageBody = " + messageBody);
        HelloData helloData = objectMapper.readValue(messageBody, HelloData.class);

        System.out.println("helloData.getUsername() = " + helloData.getUsername());
        System.out.println("helloData.getAge() = " + helloData.getAge());

        response.getWriter().write("ok");
    }
```

> μ½μ μ€ν κ²°κ³Ό
```
helloData.getUsername() = hello!
helloData.getAge() = 20
```

- JSON κ²°κ³Όλ₯Ό νμ±ν΄μ μ¬μ©ν  μ μλ μλ° κ°μ²΄λ‘ λ³ννλ €λ©΄ Jackson, Gson κ°μ JSON λ³ν λΌμ΄λΈλ¬λ¦¬λ₯Ό μΆκ°ν΄μ μ¬μ©ν΄μΌ ν©λλ€. μ€νλ§ λΆνΈλ‘ Spring MVCλ₯Ό μ ννλ©΄ κΈ°λ³ΈμΌλ‘ Jackson 
λΌμ΄λΈλ¬λ¦¬( ObjectMapper )λ₯Ό ν¨κ» μ κ³΅ν©λλ€.

- HTML form λ°μ΄ν°λ HTTP μ€νμ μμ²­ λ©μμ§ λ°λλ₯Ό ν΅ν΄ μ μ‘λλ―λ‘ μ§μ  μ½μ μ μμ΅λλ€. νμ§λ§ νΈλ¦¬ν νλ¦¬λ―Έν° μ‘°ν κΈ°λ₯ (request.getParameter(...) )μ μ΄λ―Έ μ κ³΅νκΈ° λλ¬Έμ νλΌλ―Έν° μ‘°ν κΈ°λ₯μ μ¬μ©νλ©΄ λλ€κ³  ν©λλ€.

#### HttpServletResponse - κΈ°λ³Έ μ¬μ©λ²
 HttpServletResponseμ μ­ν μ λ€μκ³Ό κ°μ΅λλ€.
- HTTP μλ΅ λ©μμ§ μμ±
  - HTTP μλ΅μ½λ μ§μ 
  - ν€λ μμ±
  - λ°λ μμ±
- νΈμ κΈ°λ₯ μ κ³΅
  - Content-Type, μΏ ν€, Redirect

``` java
@WebServlet(name = "responseHeaderServlet", urlPatterns = "/response-header")
public class ResponseHeaderServlet extends HttpServlet {

    @Override
    protected void service(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        //[status-line]
        response.setStatus(HttpServletResponse.SC_OK); //200 λ§€μ§ λλ²κ° μλκΈ° λλ¬Έμ κΆμ₯

        //[response-headers]
        response.setHeader("Content-Type","text/plain;char-set=UTF-8");
        response.setHeader("Cache-Control", "no-cache, no-store, must-revalidate"); // μΊμ μμ  λΆμ¬
        response.setHeader("Pragma","no-cache"); // μΊμ λ¬΄ν¨ν
        response.setHeader("my-header","hello"); // μμμ ν€λ
        //[message Body]
        PrintWriter writer = response.getWriter();
        writer.println("ok");
    }
}
```

![responseHeader](https://images.velog.io/images/urtimeislimited/post/811e948a-e3dc-4689-9e22-896e0aa935a1/image.png)
κ°κ²°ν μ½λλ₯Ό μν νΈμ λ©μλλ μ¬μ©ν  μ μμ΅λλ€.
```java
		//[Header νΈμ λ©μλ]
        content(response);
        
    private void content(HttpServletResponse response) {
        //Content-Type: text/plain;charset=utf-8
        //Content-Length: 2
        //response.setHeader("Content-Type", "text/plain;charset=utf-8");
        response.setContentType("text/plain");
        response.setCharacterEncoding("utf-8");
        //response.setContentLength(2); //(μλ΅μ μλ μμ±)
    }
```
μΏ ν€ νΈμ λ©μλ
```java
	cookie(response);
    
    private void cookie(HttpServletResponse response){
        //Set-Cookie: myCookie=good; Max-Age=600;
        //response.setHeader("Set-Cookie", "myCookie=good; Max-Age=600");
        Cookie cookie = new Cookie("myCookie", "good"); // μΏ ν€ κ°μ²΄ μμ± μλ΅κ°λ₯
        cookie.setMaxAge(600); //600μ΄
        response.addCookie(cookie);
    }
```
![cookie()](https://images.velog.io/images/urtimeislimited/post/1d729374-a1b0-4da6-bfb7-54d2d9096dbe/image.png)

λ¦¬λ€μ΄λ νΈ λ©μλ
```java

redirect(response);

private void redirect(HttpServletResponse response) throws IOException{
        //Status Code 302
        //Location: /basic/hello-form.html

        //response.setStatus(HttpServletResponse.SC_FOUND); //302
        //response.setHeader("Location", "/basic/hello-form.html");

        response.sendRedirect("/basic/hello-form.html");
    }
```

![redirection](https://images.velog.io/images/urtimeislimited/post/63fdedcf-fde0-438e-a829-df8679767d31/image.png)
![302](https://images.velog.io/images/urtimeislimited/post/6bc29aee-46fd-4c95-b9d4-45c399c44f1b/image.png)
- [304](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/304) : HTTP 304 Not Modified ν΄λΌμ΄μΈνΈ λ¦¬λλ μ μλ΅ μ½λλ μμ²­λ λ¦¬μμ€λ₯Ό μ¬μ μ‘ν  νμκ° μμμ λνλλλ€. μΊμλ λ¦¬μμ€μ λν μμμ  λ¦¬λλ μμλλ€.

#### HTTP μλ΅ λ°μ΄ν° - λ¨μ νμ€νΈ, HTML

HTTP μλ΅ λ©μμ§λ μ£Όλ‘ λ€μ λ΄μ©μ λ΄μμ μ λ¬ν©λλ€.
- λ¨μ νμ€νΈ μλ΅
  - μμμ μ΄ν΄λ³Έ ( writer.println("ok"); )
- HTML μλ΅
- HTTP API - MessageBody JSON μλ΅

```java
@WebServlet(name = "responseHtmlServlet", urlPatterns = "/response-html")
public class ResponseHtmlServlet extends HttpServlet {
    @Override
    protected void service(HttpServletRequest request, HttpServletResponse
            response)
            throws ServletException, IOException {
        //Content-Type: text/html;charset=utf-8
        response.setContentType("text/html");
        response.setCharacterEncoding("utf-8");

        PrintWriter writer = response.getWriter();
        writer.println("<html>");
        writer.println("<body>");
        writer.println(" <div>μλ?</div>");
        writer.println("</body>");
        writer.println("</html>");
    }
}
```
![responseHtml](https://images.velog.io/images/urtimeislimited/post/c104f391-7fd0-4743-bb0d-1cc386119fcd/image.png)
![Content-Type](https://images.velog.io/images/urtimeislimited/post/b37e0422-717d-4dee-8fed-97047a46e672/image.png)
>μμ€λ³΄κΈ°
```html
<html>
<body>
 <div>μλ?</div>
</body>
</html>
```
- HTTP μλ΅μΌλ‘ HTMLμ λ°νν  λλ content-typeμ text/html λ‘ μ§μ ν΄μΌ ν©λλ€.
- νμ΄μ§ μμ€λ³΄κΈ°λ₯Ό μ¬μ©νλ©΄ κ²°κ³Ό HTMLμ νμΈν  μ μμ΅λλ€.

#### HTTP μλ΅ λ°μ΄ν° - API JSON
λ©μμ§ λ°λμ ν¬ν¨ν  HTTP μλ΅ λ°μ΄ν°λ₯Ό λ§λ€ λ μ¬μ©νλ JSON νμμ μμλ³΄κ² μ΅λλ€.

```java
@WebServlet(name = "responseJsonServlet", urlPatterns = "/response-json")
public class ResponseJsonServlet extends HttpServlet {
    private ObjectMapper objectMapper = new ObjectMapper();

    @Override
    protected void service(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        //Content-Type: application/json
        response.setContentType("application/json");
        response.setCharacterEncoding("utf-8");

        HelloData helloData = new HelloData();
        helloData.setUsername("kim");
        helloData.setAge(20);

        //{"username":"kim","age":20}
        String result = objectMapper.writeValueAsString(helloData);
        response.getWriter().write(result);

    }
}
```
> http://localhost:8080/response-json
![responseJson](https://images.velog.io/images/urtimeislimited/post/4f59fe98-b858-4419-86d1-3d3c235ae02c/image.png)
![responseJson2](https://images.velog.io/images/urtimeislimited/post/ebf4c1b5-1488-4db9-a495-c786e30acecb/image.png)

- HTTP μλ΅μΌλ‘ JSONμ λ°νν  λλ content-typeμapplication/json λ‘ μ§μ ν΄μΌ ν©λλ€.
- Jackson λΌμ΄λΈλ¬λ¦¬κ° μ κ³΅νλ objectMapper.writeValueAsString() λ₯Ό μ¬μ©νλ©΄ κ°μ²΄λ₯Ό JSON λ¬Έμλ‘ λ³κ²½ν  μ μμ΅λλ€.
- μ°Έκ³  : application/json μ μ€νμ utf-8 νμμ μ¬μ©νλλ‘ μ μλμ΄ μμ΅λλ€. κ·Έλμ μ€νμμ charset=utf-8 κ³Ό κ°μ μΆκ° νλΌλ―Έν°λ₯Ό μ§μνμ§ μμ΅λλ€. λ°λΌμ application/json μ΄λΌκ³ λ§ μ¬μ©ν΄μΌμ§ application/json;charset=utf-8 μ΄λΌκ³  μ λ¬νλ κ²μ μλ―Έ μλ νλΌλ―Έν°λ₯Ό μΆκ°ν κ²μ΄ λ©λλ€.
- response.getWriter()λ₯Ό μ¬μ©νλ©΄ μΆκ° νλΌλ―Έν°λ₯Ό μλμΌλ‘ μΆκ°ν΄λ²λ¦½λλ€. μ΄λλ response.getOutputStream()μΌλ‘ λ³νν΄μ μΆλ ₯νλ©΄ κ·Έλ° λ¬Έμ κ° μμ΅λλ€.

> μλΈλ¦Ώ μ λ¦¬
- HttpServlet κ°μ²΄λ HTTP μ€νλλ‘ μμ²­ λ©μμ§ νμ±μ μ΅μννμ¬ νΈλ¦¬νκ² μ¬μ©ν  μ μλλ‘ μ‘°ννλ λ°©λ²μλλ€.
- HttpServletRequestκ° μ κ³΅νλ κΈ°λ³Έ κΈ°λ₯
  - printStartLine(request); //μ€νν° λΌμΈ μ λ³΄
  - printHeaders(request); //Header λͺ¨λ  μ λ³΄
  - printHeaderUtils(request); //Header νΈμ μ‘°ν 
  - printEtc(request); //κΈ°ν μ λ³΄
- HTTP μμ²­ λ©μμ§λ₯Ό ν΅ν΄ ν΄λΌμ΄μΈνΈμμ μλ²λ‘ λ°μ΄ν°λ₯Ό μ λ¬νλ λ°©λ²
  - GET : μΏΌλ¦¬ νλΌλ―Έν°
    - λ©μμ§ λ°λ μμ΄, URLμ μΏΌλ¦¬ νλΌλ―Έν°μ λ°μ΄ν°λ₯Ό ν¬ν¨ν΄μ μ λ¬ (κ²μ, νν°, νμ΄μ§ λ±μμ λ§μ΄ μ¬μ©)
  - POST : HTML Form
    - μΉ λΈλΌμ°μ κ° content-type: application/x-www-form-urlencoded νμμ HTTP λ©μμ§ μμ±
    - λ©μμ§ λ°λμ μΏΌλ¦¬ νλΌλ―Έν° νμμΌλ‘ μ λ¬(νμ κ°μ, μν μ£Όλ¬Έ, HTML Form μ¬μ©)
    - getParameter() λ GET URL μΏΌλ¦¬ νλΌλ―Έν° νμλ μ§μνκ³ , POST HTML Form νμ λ λ€ μ§μ
    - HTTP μ€νμ HTML Form μ¬μ©μ POSTλ§ νμ©
  - HTTP message body
    - HTTP APIμμ μ£Όλ‘ μ¬μ©, JSON, XML, TEXT
    - λ°μ΄ν° νμμ μ£Όλ‘ JSON μ¬μ©
    - POST, PUT, PATCH
- μλ΅
  - λ°μ΄ν°λ λ©μμ§, HTML, API JSON ννλ‘ μλ΅ κ°λ₯
  - ν€λλ setStatus()λ‘ μν μ§μ , setHeader(), νΈμ λ©μλ λ± μ¬μ© κ°λ₯
  
***

### 3. μλΈλ¦Ώ, JSP, MVC ν¨ν΄
μλΈλ¦Ώ - λΆνΈν¨ κ°μ  JSP - λΆνΈν¨ κ°μ  MVC ν¨ν΄ μ μ©
μμλλ‘ κ°λ¨ν νμ κ΄λ¦¬ μΉ μ νλ¦¬μΌμ΄μμ λ§λ€μ΄ λ³΄κ² μ΅λλ€.

#### μκ΅¬μ¬ν­
- νμ μ λ³΄
  - μ΄λ¦: username
  - λμ΄: age
- κΈ°λ₯ μκ΅¬μ¬ν­
  - νμ μ μ₯
  - νμ λͺ©λ‘ μ‘°ν

λλ©μΈ λͺ¨λΈμ μ€κ³ν΄λ³΄κ² μ΅λλ€.
hello.servlet.domain.member;
νμ λλ©μΈ
```java
@Getter @Setter
public class Member {

    private Long id; // νμ μ μ₯μ FK
    private String username;
    private int age;

    public Member(){}
    public Member(Long id, String username, int age) {
        this.id = id;
        this.username = username;
        this.age = age;
    }
}
```
- id λ Member λ₯Ό νμ μ μ₯μμ μ μ₯νλ©΄ νμ μ μ₯μκ° ν λΉν©λλ€.

νμ μ μ₯μ
```java
public class MemberRepository {

    /**
     * λμμ± λ¬Έμ κ° κ³ λ €λμ΄ μμ§ μμ, μ€λ¬΄μμλ ConcurrentHashMap, AtomicLong μ¬μ© κ³ λ €
     */
    // {key: id, value: member}
    private static Map<Long, Member> store = new HashMap<>();
    private static long sequence = 0L; // id νλμ© μ¦κ°νλ κ°μ²΄

    //μ±κΈν€ ν¨ν΄ μν΄ static μ¬μ©
    private static final MemberRepository instance = new MemberRepository();

    public static MemberRepository getInstance(){
        return instance;
    }

    private MemberRepository() {}

    public Member save(Member member){
        member.setId(++sequence);
        store.put(member.getId(), member);
        return member;
    }
    public Member findById(Long id){
        return store.get(id);
    }
    public List<Member> findAll(){
        return new ArrayList<>(store.values()); //storeμ λͺ¨λ  κ° μλ‘μ΄ ArrayListμ μ μ₯
    }

    public void clearStore(){
        store.clear(); // νμ€νΈμ μ¬μ©
    }
}
```
- νμ μ μ₯μλ μ±κΈν€ ν¨ν΄μ μ μ©νμ΅λλ€. μ€νλ§μ μ¬μ©νλ©΄ μ€νλ§ λΉμΌλ‘ λ±λ‘νλ©΄ λμ§λ§, μ§κΈμ μ΅λν μ€νλ§ μμ΄ μμ μλΈλ¦Ώ λ§μΌλ‘ κ΅¬ννλ κ²μ΄ λͺ©μ μλλ€.
μ±κΈν€ ν¨ν΄μ κ°μ²΄λ₯Ό λ¨ νλλ§ μμν΄μ κ³΅μ ν΄μΌ νλ―λ‘ μμ±μλ₯Ό private μ κ·Όμλ‘ λ§μλ‘λλ€.

νμ μ μ₯μ νμ€νΈ
```java
class MemberRepositoryTest {

    MemberRepository memberRepository = MemberRepository.getInstance(); // μ±κΈν€μ newμ¬μ© νμ x

    @AfterEach // νμ€νΈ μ’λ£μ μ΄κΈ°ν, λ°μ΄ν° μ μ₯ μμ λ³΄μ₯μ μν΄ μ¬μ©
    void afterEach(){
        memberRepository.clearStore();
    }

    @Test
    void save() {
        //given
        Member member = new Member("hello", 20);
        //when
        Member savedMember = memberRepository.save(member);
        //then
        Member findMember = memberRepository.findById(savedMember.getId());
        assertThat(findMember).isEqualTo(savedMember);
    }

    @Test
    void findAll(){
        //given
        Member member1 = new Member("member1", 20);
        Member member2 = new Member("member2", 30);

        memberRepository.save(member1);
        memberRepository.save(member2);
        //when
        List<Member> result = memberRepository.findAll();

        //then
        assertThat(result.size()).isEqualTo(2);
        assertThat(result).contains(member1, member2);
    }
}
```
> Test Passed

- νμμ μ μ₯νκ³ , λͺ©λ‘μ μ‘°ννλ νμ€νΈλ₯Ό μμ±νμ΅λλ€.
κ° νμ€νΈκ° λλ  λ, λ€μ νμ€νΈμ μν₯μ μ£Όμ§ μλλ‘ κ° νμ€νΈμ μ μ₯μλ₯Ό clearStore() λ₯Ό νΈμΆν΄μ μ΄κΈ°ννμ΅λλ€.

#### μλΈλ¦ΏμΌλ‘ νμ κ΄λ¦¬ μΉ μ νλ¦¬μΌμ΄μ λ§λ€κΈ°
λ³Έκ²©μ μΌλ‘ μλΈλ¦Ώ νμ κ΄λ¦¬ μΉ μ νλ¦¬μΌμ΄μμ λ§λ€κΈ° μν΄
κ°μ₯ λ¨Όμ  μλΈλ¦ΏμΌλ‘ νμ λ±λ‘ HTML νΌμ μ κ³΅ν΄λ³΄κ² μ΅λλ€.

νμ λ±λ‘ νΌ
```java
@WebServlet(name = "memberFormServlet", urlPatterns = "/servlet/members/new-form")
public class MemberFormServlet extends HttpServlet {

    private MemberRepository memberRepository = MemberRepository.getInstance();

    @Override
    protected void service(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {

        // HTTP μλ΅ Content λ°λ
        response.setContentType("text/html");
        response.setCharacterEncoding("utf-8");


        PrintWriter w = response.getWriter();
        // λ³΄ν΅ μΌμ΄ μλλ€..
        w.write("<!DOCTYPE html>\n" +
                "<html>\n" +
                "<head>\n" +
                " <meta charset=\"UTF-8\">\n" +
                " <title>Title</title>\n" +
                "</head>\n" +
                "<body>\n" +
                "<form action=\"/servlet/members/save\" method=\"post\">\n" +
                " username: <input type=\"text\" name=\"username\" />\n" +
                " age: <input type=\"text\" name=\"age\" />\n" +
                " <button type=\"submit\">μ μ‘</button>\n" +
                "</form>\n" +
                "</body>\n" +
                "</html>\n");
    }
}
```
> http://localhost:8080/servlet/members/new-form
![/servlet/members/new-form](https://images.velog.io/images/urtimeislimited/post/ecef2521-346d-4a21-a256-ff19d43abd37/image.png)
>νμ΄μ§ μμ€
![/servlet/members/new-form2](https://images.velog.io/images/urtimeislimited/post/b73e20af-4ea0-4330-9e11-dc39e80211fb/image.png)

νμ μ μ₯
```java
@WebServlet(name = "memberSaveServlet", urlPatterns = "/servlet/members/save")
public class MemberSaveServlet extends HttpServlet {
    private MemberRepository memberRepository = MemberRepository.getInstance();
    @Override
    protected void service(HttpServletRequest request, HttpServletResponse
            response)
            throws ServletException, IOException {
        System.out.println("MemberSaveServlet.service");

        //GET μΏΌλ¦¬ νλΌλ―Έν°, HTML Form λλ€ getParameter() μ¬μ© κ°λ₯
        // Form submit κ²°κ³Ό getParameter()λ‘ μ‘°ν
        String username = request.getParameter("username");
        int age = Integer.parseInt(request.getParameter("age"));

        //μ μ₯
        Member member = new Member(username, age);
        memberRepository.save(member);

        //κ²°κ³Ό μλ΅
        response.setContentType("text/html");
        response.setCharacterEncoding("utf-8");
        PrintWriter w = response.getWriter();
        w.write("<html>\n" +
                "<head>\n" +
                " <meta charset=\"UTF-8\">\n" +
                "</head>\n" +
                "<body>\n" +
                "μ±κ³΅\n" +
                "<ul>\n" +
                " <li>id="+member.getId()+"</li>\n" +
                " <li>username="+member.getUsername()+"</li>\n" +
                " <li>age="+member.getAge()+"</li>\n" +
                "</ul>\n" +
                "<a href=\"/index.html\">λ©μΈ</a>\n" +
                "</body>\n" +
                "</html>");
    }
}
```
> http://localhost:8080/servlet/members/new-form μμ submin κ²°κ³Ό
![save](https://images.velog.io/images/urtimeislimited/post/7124f534-f648-49c0-8281-497bbd5341fe/image.png)

νμ λͺ©λ‘

```java
@WebServlet(name = "memberListServlet", urlPatterns = "/servlet/members")
public class MemberListServlet extends HttpServlet {
    private MemberRepository memberRepository = MemberRepository.getInstance();

    @Override
    protected void service(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        List<Member> members = memberRepository.findAll();

        response.setContentType("text/html");
        response.setCharacterEncoding("utf-8");

        PrintWriter w = response.getWriter();

        w.write("<html>");
        w.write("<head>");
        w.write(" <meta charset=\"UTF-8\">");
        w.write(" <title>Title</title>");
        w.write("</head>");
        w.write("<body>");
        w.write("<a href=\"/index.html\">λ©μΈ</a>");
        w.write("<table>");
        w.write(" <thead>");
        w.write(" <th>id</th>");
        w.write(" <th>username</th>");
        w.write(" <th>age</th>");
        w.write(" </thead>");
        w.write(" <tbody>");
/*
 w.write(" <tr>");
 w.write(" <td>1</td>");
 w.write(" <td>userA</td>");
 w.write(" <td>10</td>");
 w.write(" </tr>");
*/
        for (Member member : members) {
            w.write(" <tr>");
            w.write(" <td>" + member.getId() + "</td>");
            w.write(" <td>" + member.getUsername() + "</td>");
            w.write(" <td>" + member.getAge() + "</td>");
            w.write(" </tr>");
        }
        w.write(" </tbody>");
        w.write("</table>");
        w.write("</body>");
        w.write("</html>");
    }
}
```
![memberList](https://images.velog.io/images/urtimeislimited/post/1eb3a7d0-ce5d-4d12-8dde-175397809e90/image.png)

MemberListServlet μ λ€μ μμλ‘ λμν©λλ€.
1. memberRepository.findAll() μ ν΅ν΄ λͺ¨λ  νμμ μ‘°ννλ€.
2. νμ λͺ©λ‘ HTMLμ for λ£¨νλ₯Ό ν΅ν΄μ νμ μ λ§νΌ λμ μΌλ‘ μμ±νκ³  μλ΅ν©λλ€.

>ννλ¦Ώ μμ§μΌλ‘
μ§κΈκΉμ§ μλΈλ¦Ώκ³Ό μλ° μ½λλ§μΌλ‘ HTMLμ λ§λ€μ΄λ³΄μμ΅λλ€. 
μλΈλ¦Ώ λλΆμ λμ μΌλ‘ μνλ HTMLμ λ§μκ» λ§λ€ μ μμ§λ§ 
μ μ μΈ HTML λ¬ΈμλΌλ©΄ νλ©΄μ΄ κ³μ λ¬λΌμ§λ νμμ μ μ₯ κ²°κ³ΌλΌλκ°, νμ λͺ©λ‘ κ°μ λμ μΈ HTMLμ λ§λλ μΌμ λΆκ°λ₯ ν  κ²μλλ€.
κ·Έλ°λ°, μ½λμμ λ³΄λ―μ΄ μ΄κ²μ λ§€μ° λ³΅μ‘νκ³  λΉν¨μ¨ μ μλλ€.
μλ° μ½λλ‘ HTMLμ λ§λ€μ΄ λ΄λ κ² λ³΄λ€
μ°¨λΌλ¦¬ HTML λ¬Έμμ λμ μΌλ‘ λ³κ²½ν΄μΌ νλ λΆλΆλ§ μλ° μ½λλ₯Ό λ£μ μ μλ€λ©΄ λ νΈλ¦¬ν  κ² κ°μ΅λλ€.
μ΄κ²μ΄ λ°λ‘ ννλ¦Ώ μμ§μ΄ λμ¨ μ΄μ μλλ€. 
ννλ¦Ώ μμ§μ μ¬μ©νλ©΄ HTML λ¬Έμμμ νμν κ³³λ§ μ½λλ₯Ό μ μ©ν΄μ λμ μΌλ‘ λ³κ²½ν  μ μμ΅λλ€.
ννλ¦Ώ μμ§μλ JSP, Thymeleaf, Freemarker, Velocityλ±μ΄ μμ΅λλ€.

 - μ°Έκ³ 
  - JSPλ μ±λ₯κ³Ό κΈ°λ₯λ©΄μμ λ€λ₯Έ ννλ¦Ώ μμ§κ³Όμ κ²½μμμ λ°λ¦¬λ©΄μ, μ μ  μ¬μ₯λμ΄ κ°λ μΆμΈμλλ€. ννλ¦Ώ μμ§λ€μ κ°κ° μ₯λ¨μ μ΄ μλλ°, JSPλ μ κΉ λ€λ£¨κ³ , μ€νλ§κ³Ό μ ν΅ν©λλ Thymeleafλ₯Ό μ¬μ©νκ² μ΅λλ€.
  


#### JSPλ‘ νμ κ΄λ¦¬ μΉ μ νλ¦¬μΌμ΄μ λ§λ€κΈ°
JSPλ₯Ό μ¬μ©νλ €λ©΄ λ¨Όμ  λ€μ λΌμ΄λΈλ¬λ¦¬λ₯Ό μΆκ°ν΄μΌ ν©λλ€.

```java
//JSP μΆκ° μμ
implementation 'org.apache.tomcat.embed:tomcat-embed-jasper'
implementation 'javax.servlet:jstl'
//JSP μΆκ° λ
```
νμ λ±λ‘ νΌ JSP
```jsp
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<html>
<head>
    <title>Title</title>
</head>
<body>
<form action="/jsp/members/save.jsp" method="post">
    username: <input type="text" name="username" />
    age:      <input type="text" name="age" />
    <button type="submit">μ μ‘</button>
</form>
</body>
</html>
```
![/jsp/members/save.jsp](https://images.velog.io/images/urtimeislimited/post/3e898bf0-f209-476d-a335-2ec7208ae8b0/image.png)

νμ μ μ₯ JSP
```jsp
<%@ page import="hello.servlet.domain.member.Member" %>
<%@ page import="hello.servlet.domain.member.MemberRepository" %>
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<%--μλ° λ‘μ§ νκ·Έ--%>
<%
    // request, responseμ κ·Έλ₯ μ¬μ© κ°λ₯
    MemberRepository memberRepository = MemberRepository.getInstance();
    String username = request.getParameter("username");
    int age = Integer.parseInt(request.getParameter("age"));

    Member member = new Member(username, age);
    memberRepository.save(member);
%>
<html>
<head>
    <title>Title</title>
</head>
<body>
μ±κ³΅
<ul>
    <li>id=<%=member.getId()%></li>
    <li>username=<%=member.getUsername()%></li>
    <li>age=<%=member.getAge()%></li>
</ul>
<a href="/index.html">λ©μΈ</a>
</body>
</html>
```
>http://localhost:8080/jsp/members/new-form.jsp μ μ₯ κ²°κ³Ό
![save.jsp](https://images.velog.io/images/urtimeislimited/post/7bcadb28-3ff6-4ea4-80e2-a92cc052afbf/image.png)

JSPλ μλ° μ½λλ₯Ό κ·Έλλ‘ λ€ μ¬μ©ν  μ μμ΅λλ€.
- <%@ page import="hello.servlet.domain.member.MemberRepository" %>
  - μλ°μ import λ¬Έκ³Ό κ°λ€.
- <% ~~ %>
  - μ΄ λΆλΆμλ μλ° μ½λλ₯Ό μλ ₯ν  μ μλ€.
- <%= ~~ %>
  - μ΄ λΆλΆμλ μλ° μ½λλ₯Ό μΆλ ₯ν  μ μλ€.
νμ μ μ₯ JSPλ₯Ό λ³΄λ©΄, νμ μ μ₯ μλΈλ¦Ώ μ½λμ κ°μ΅λλ€. 
λ€λ₯Έ μ μ΄ μλ€λ©΄, HTMLμ μ€μ¬μΌλ‘ νκ³ , μλ° μ½λλ₯Ό λΆλΆλΆλΆ μλ ₯ν΄μ£Όμμ΅λλ€. <% ~ %> λ₯Ό μ¬μ©ν΄μ HTML μ€κ°μ μλ° μ½λλ₯Ό μΆλ ₯νκ³  μμ΅λλ€.

νμ λͺ©λ‘ JSP
``` jsp
<%
    MemberRepository memberRepository = MemberRepository.getInstance();
    List<Member> members = memberRepository.findAll();
%>
<html>
<head>
    <meta charset="UTF-8">
    <title>Title</title>
</head>
<a href="/index.html">λ©μΈ</a>
<table>
    <thead>
    <th>id</th>
    <th>username</th>
    <th>age</th>
    </thead>
    <tbody>
    <%
        for (Member member : members) {
            out.write(" <tr>");
            out.write(" <td>" + member.getId() + "</td>");
            out.write(" <td>" + member.getUsername() + "</td>");
            out.write(" <td>" + member.getAge() + "</td>");
            out.write(" </tr>");
        }
    %>
    </tbody>
</table>
</body>
</html>
```

νμ λ¦¬ν¬μ§ν λ¦¬λ₯Ό λ¨Όμ  μ‘°ννκ³ , κ²°κ³Ό Listλ₯Ό μ¬μ©ν΄μ μ€κ°μ <tr><td> HTML νκ·Έλ₯Ό λ°λ³΅ν΄μ μΆλ ₯νκ³  μμ΅λλ€.
  
#### μλΈλ¦Ώκ³Ό JSPμ νκ³
  
μλΈλ¦ΏμΌλ‘ κ°λ°ν  λλ λ·°(View)νλ©΄μ μν HTMLμ λ§λλ μμμ΄ μλ° μ½λμ μμ¬μ μ§μ λΆνκ³  λ³΅μ‘νμ΅λλ€.
JSPλ₯Ό μ¬μ©ν λλΆμ λ·°λ₯Ό μμ±νλ HTML μμμ κΉλνκ² κ°μ Έκ°κ³ , μ€κ°μ€κ° λμ μΌλ‘ λ³κ²½μ΄ νμν λΆλΆμλ§ μλ° μ½λλ₯Ό μ μ©νμ§λ§ ν΄κ²°λμ§ μλ λͺκ°μ§ κ³ λ―Όμ΄ λ¨μ΅λλ€.
νμ μ μ₯ JSPλ₯Ό λ³΄λ©΄, μ½λμ μμ μ λ°μ νμμ μ μ₯νκΈ° μν λΉμ¦λμ€ λ‘μ§μ΄κ³ , λλ¨Έμ§ νμ μ λ°λ§ κ²°κ³Όλ₯Ό HTMLλ‘ λ³΄μ¬μ£ΌκΈ° μν λ·° μμ­μλλ€. 
νμ λͺ©λ‘μ κ²½μ°μλ λ§μ°¬κ°μ§μλλ€.
μ½λλ₯Ό μ λ³΄λ©΄, JAVA μ½λ, λ°μ΄ν°λ₯Ό μ‘°ννλ λ¦¬ν¬μ§ν λ¦¬ λ±λ± λ€μν μ½λκ° λͺ¨λ JSPμ λΈμΆλμ΄ μλ€. 
JSPκ° λλ¬΄ λ§μ μ­ν μ νλ€. μ΄λ κ² μμ νλ‘μ νΈλ λ²μ¨ λ¨Έλ¦¬κ° μνμ€λλ°, μλ°± μμ²μ€μ΄ λμ΄κ°λ JSPλ₯Ό λ μ¬λ €λ³΄λ©΄ μ λ§ μ§μ₯κ³Ό κ°μ κ²μλλ€. 
  
#### MVC ν¨ν΄ - κ°μ
__λλ¬΄ λ§μ μ­ν __
νλμ μλΈλ¦Ώμ΄λ JSPλ§μΌλ‘ λΉμ¦λμ€ λ‘μ§κ³Ό λ·° λ λλ§κΉμ§ λͺ¨λ μ²λ¦¬νκ² λλ©΄, λλ¬΄ λ§μ μ­ν μ νκ²λκ³ , κ²°κ³Όμ μΌλ‘ μ μ§λ³΄μκ° μ΄λ €μμ§λλ€. 
λΉμ¦λμ€ λ‘μ§μ νΈμΆνλ λΆλΆμ λ³κ²½μ΄ λ°μν΄λ ν΄λΉ μ½λλ₯Ό μλμΌ νκ³ , UIλ₯Ό λ³κ²½ν  μΌμ΄ μμ΄λ λΉμ¦λμ€ λ‘μ§μ΄ ν¨κ» μλ ν΄λΉ νμΌμ μμ ν΄μΌ ν©λλ€. 
HTML μ½λ νλ μμ ν΄μΌ νλλ°, μλ°±μ€μ μλ° μ½λκ° ν¨κ» μλ€κ³  μμν΄λ³΄λ©΄.. λλ λΉμ¦λμ€ λ‘μ§μ νλ μμ ν΄μΌ νλλ° μλ°± μμ²μ€μ HTML μ½λκ° ν¨κ» μλ€κ³  μμν΄λ³΄λ©΄ λμ°ν©λλ€!!

__λ³κ²½μ λΌμ΄ν μ¬μ΄ν΄__
μ¬μ€ μ΄κ² μ λ§ μ€μνλ°, μ§μ§ λ¬Έμ λ λ μ¬μ΄μ **λ³κ²½μ λΌμ΄ν μ¬μ΄ν΄μ΄ λ€λ₯΄λ€**λ μ μλλ€. μλ₯Ό λ€μ΄μ UIλ₯Ό μΌλΆ μμ νλ μΌκ³Ό λΉμ¦λμ€ λ‘μ§μ μμ νλ μΌμ κ°κ° λ€λ₯΄κ² λ°μν  κ°λ₯μ±μ΄ λ§€μ° λκ³  λλΆλΆ μλ‘μκ² μν₯μ μ£Όμ§ μμ΅λλ€. 
μ΄λ κ² λ³κ²½μ λΌμ΄ν μ¬μ΄ν΄μ΄ λ€λ₯Έ λΆλΆμ νλμ μ½λλ‘ κ΄λ¦¬νλ κ²μ μ μ§λ³΄μνκΈ° μ’μ§ μμ΅λλ€. (λ¬Όλ‘  UIκ° λ§μ΄ λ³νλ©΄ ν¨κ» λ³κ²½λ  κ°λ₯μ±λ μμ΅λλ€.)
  
__κΈ°λ₯ νΉν__
νΉν JSP κ°μ λ·° ννλ¦Ώμ νλ©΄μ λ λλ§ νλλ° μ΅μ ν λμ΄ μκΈ° λλ¬Έμ μ΄ λΆλΆμ μλ¬΄λ§ λ΄λΉνλ κ²μ΄ κ°μ₯ ν¨κ³Όμ μλλ€.
  
__Model View Controller__
MVC ν¨ν΄μ μ§κΈκΉμ§ νμ΅ν κ² μ²λΌ νλμ μλΈλ¦Ώμ΄λ, JSPλ‘ μ²λ¦¬νλ κ²μ, 
μ»¨νΈλ‘€λ¬(Controller)μ λ·°(View)λΌλ μμ­μΌλ‘ μλ‘ μ­ν μ λλ κ²μ λ§ν©λλ€.  μΉ μ νλ¦¬μΌμ΄μμ λ³΄ν΅ μ΄ MVC ν¨ν΄μ μ¬μ©ν©λλ€.
  
__μ»¨νΈλ‘€λ¬__: HTTP μμ²­μ λ°μμ νλΌλ―Έν°λ₯Ό κ²μ¦νκ³ , λΉμ¦λμ€ λ‘μ§μ μ€νν©λλ€. κ·Έλ¦¬κ³  λ·°μ μ λ¬ν  κ²°κ³Ό λ°μ΄ν°λ₯Ό μ‘°νν΄μ λͺ¨λΈμ μ μ₯ν©λλ€.
__λͺ¨λΈ__: λ·°μ μΆλ ₯ν  λ°μ΄ν°λ₯Ό μ μ₯ν©λλ€. λ·°κ° νμν λ°μ΄ν°λ₯Ό λͺ¨λ λͺ¨λΈμ λ΄μμ μ λ¬ν΄μ£Όλ λλΆμ λ·°λ λΉμ¦λμ€ λ‘μ§μ΄λ λ°μ΄ν° μ κ·Όμ λͺ°λΌλ λκ³ , νλ©΄μ λ λλ§ νλ μΌμ μ§μ€ν  μ μμ΅λλ€.
__λ·°__: λͺ¨λΈμ μ μ₯λ λ°μ΄ν°λ₯Ό μ¬μ©ν΄μ νλ©΄μ κ·Έλ¦¬λ μΌμ μ§μ€ν©λλ€. (HTMLμ μμ±νλ λΆλΆμ λ§ν©λλ€.)

MVC ν¨ν΄ μ΄μ 
![beforeMVC](https://images.velog.io/images/urtimeislimited/post/0591a4d0-ad6c-4bd9-b05a-6cca1a9dc8f8/image.png)

MVC ν¨ν΄ λμ μμ
  1. κ³ κ° μμ²­ μ μ»¨νΈλ‘€λ¬μμ λΉμ¦λμ€ λ‘μ§μ μνν©λλ€.
  2. κ²°κ³Ό λ°μ΄ν°λ₯Ό λͺ¨λΈμ μ μ₯ν©λλ€.
  3. λͺ¨λΈμ ν΅ν΄ λ°μ΄ν°λ₯Ό μ λ¬λ°μ λ·°λ μ μ΄κΆμ λκ²¨λ°κ³  λ·° λ‘μ§μ μνν©λλ€.
    - λͺ¨λΈ λλΆμ μ»¨νΈλ‘€κ³Ό λ·°μ μμ‘΄ κ΄κ³κ° κ°μνλ©λλ€.
  4. λ·° λ‘μ§ μ€ν κ²°κ³Όλ₯Ό κ³ κ°μκ² μλ΅ν©λλ€.
![mvc](https://images.velog.io/images/urtimeislimited/post/378d2958-c5d0-4b12-a341-7128b9316d0d/image.png)
	

***

### 4. MVC νλ μμν¬ λ§λ€κΈ°

MVC ν¨ν΄μ "κ³΅ν΅ μ²λ¦¬μ μ΄λ €μ"μ΄λΌλ νκ³κ° μμμ΅λλ€. νλ‘ νΈ μ»¨νΈλ‘€λ¬ ν¨ν΄μ λμμμΌ μ μ§μ μΌλ‘ κ°μ μμΌλ³΄κ² μ΅λλ€.

####  νλ‘ νΈ μ»¨νΈλ‘€λ¬ ν¨ν΄ μκ°

νλ‘ ν° μ»¨νΈλ‘€λ¬λ₯Ό λμνκΈ° μ μλ
ν΄λΌμ΄μΈνΈκ° λ§€λ² κ³΅ν΅ λ‘μ§κ³Ό μ»¨νΈλ‘€λ¬ λ‘μ§μ κ°κ° μννμ΄μΌ νμ΅λλ€. 
![fc](https://images.velog.io/images/urtimeislimited/post/83b4e885-16f7-4f12-868f-05913be92231/image.png)
νλ‘ νΈ μ»¨νΈλ‘€λ¬λ₯Ό λμ νκ² λλ©΄ λ¨Όμ  κ³΅ν΅ λ‘μ§μ ν κ³³μμ μ²λ¦¬νκ³  κ° μ»¨νΈλ‘€λ¬μκ² λ‘μ§ μ²λ¦¬λ₯Ό λκ²¨μ€λλ€. κ³΅ν΅μ κ΄μ¬μ¬λ₯Ό μ°μ μ μΌλ‘ λ¨Όμ  μ²λ¦¬ν΄μ£Όλ λ¬Έμ§κΈ° μ­ν μ΄λΌκ³  ν  μ μμ΅λλ€.
![afterFc](https://images.velog.io/images/urtimeislimited/post/68b70845-5536-4f9d-81a2-896786950d2f/image.png)

FrontControllerμ νΉμ§μ λ€μκ³Ό κ°μ΅λλ€.

- νλ‘ νΈ μ»¨νΈλ‘€λ¬ μλΈλ¦Ώ νλλ‘ ν΄λΌμ΄μΈνΈμ μμ²­μ λ°μ΅λλ€.
- νλ‘ νΈ μ»¨νΈλ‘€λ¬κ° μμ²­μ λ§λ μ»¨νΈλ‘€λ¬λ₯Ό μ°Ύμμ νΈμΆν©λλ€.
- μκ΅¬λ₯Ό νλλ‘! μ΅μνν©λλ€.
- **κ³΅ν΅ μ²λ¦¬ κ°λ₯**
- νλ‘ νΈ μ»¨νΈλ‘€λ¬λ₯Ό μ μΈν λλ¨Έμ§ μ»¨νΈλ‘€λ¬λ μλΈλ¦Ώμ μ¬μ©νμ§ μμλ λ©λλ€.
  - μμ²­ λ§€νμ μ¬μ©λλ μλΈλ¦Ώμ νλ‘ νΈ μ»¨νΈλ‘€λ¬λ‘ μΆ©λΆν©λλ€.

μ€νλ§ μΉ MVCμ ν΅μ¬μ λ°λ‘ **FrontController**μ μμ΅λλ€. μ€νλ§ μΉ MVCμ __DispatcherServlet__μ΄ FrontController ν¨ν΄μΌλ‘ κ΅¬νλμ΄ μκΈ° λλ¬Έμλλ€.
- [DispatcherServlet](https://www.java67.com/2017/06/what-is-use-of-dispatcherservlet-in-spring-mvc.html#:~:text=The%20DispatcherServlet%20is%20one%20of,acts%20as%20a%20Front%20Controller.&text=The%20DispatcherServlet%20is%20a%20front,Spring%20MVC%20controllers%20for%20processing.) : DispatcherServletμ Spring MVC μΉ μ νλ¦¬μΌμ΄μμ λν ν΄λΌμ΄μΈνΈ μμ²­μ λν λ¨μΌ μ§μμ μ μ κ³΅νκ³  μ²λ¦¬λ₯Ό μν΄ μμ²­μ Spring MVC μ»¨νΈλ‘€λ¬μ μ λ¬νλ κ²κ³Ό κ°μ FrontControllerμλλ€.

#### νλ‘ νΈ μ»¨νΈλ‘€λ¬ λμ - v1

νλ‘ νΈ μ»¨νΈλ‘€λ¬λ₯Ό λ¨κ³μ μΌλ‘ λμν΄λ³΄κ² μ΅λλ€.
κΈ°μ‘΄ μ½λλ₯Ό μ΅λν μ μ§νλ©΄μ, νλ‘ νΈ μ»¨νΈλ‘€λ¬ λμνλ κ²μ λͺ©νλ‘ λ¨Όμ  κ΅¬μ‘°λ₯Ό μ€μ ν ν μ μ§μ  λ¦¬ν©ν°λ§ νκ² μ΅λλ€.
- v1 κ΅¬μ‘°
1. ν΄λΌμ΄μΈνΈκ° HTTP μμ²­ μ FrontControllerλΌλ μλΈλ¦Ώμ΄ μμ²­μ μ λ¬λ°μ΅λλ€.
   - μμ²­ λ©μμ§μμ URL λ§€ν μ λ³΄λ₯Ό κΈ°λ°μΌλ‘ νμν μ»¨νΈλ‘€λ¬λ₯Ό μ‘°νν©λλ€.
2. ν΄λΉ μ»¨νΈλ‘€λ¬λ₯Ό νΈμΆν©λλ€.
3. μ»¨νΈλ‘€λ¬κ° μμ μ λ‘μ§μ μν, 
viewλ‘forward -> JSP(ν΄λΉ μλΈλ¦Ώ) λ λλ§νμ¬ μλ΅μ λ°νν©λλ€.

![v1](https://images.velog.io/images/urtimeislimited/post/ab4fe8e4-6dbd-4dd0-ac06-fe1724724200/image.png)

- μλΈλ¦Ώκ³Ό λΉμ·ν λͺ¨μμ μ»¨νΈλ‘€λ¬ μΈν°νμ΄μ€λ₯Ό λμν©λλ€. 
```java
public interface ControllerV1 {
        void process(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException;
}
```
- κ° μ»¨νΈλ‘€λ¬λ€μ μ΄ μΈν°νμ΄μ€λ₯Ό κ΅¬ννλ©΄
λ©λλ€. 
- νλ‘ νΈ μ»¨νΈλ‘€λ¬λ μ΄ μΈν°νμ΄μ€λ₯Ό νΈμΆν΄μ κ΅¬νκ³Ό κ΄κ³μμ΄ λ‘μ§μ μΌκ΄μ±μ κ°μ Έκ° μ μμ΅λλ€.
- κΈ°μ‘΄ λ‘μ§μ μ΅λν μ μ§νλ©΄μ μΈν°νμ΄μ€λ₯Ό κ΅¬νν μ»¨νΈλ‘€λ¬λ₯Ό λ§λ€μ΄λ³΄κ² μ΅λλ€. 

**νμ λ±λ‘ μ»¨νΈλ‘€λ¬**
 ```java
 public class MemberFormControllerV1 implements ControllerV1{
    @Override
    public void process(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        String viewPATH = "/WEB-INF/views/new-form.jsp";
        RequestDispatcher dispatcher = request.getRequestDispatcher(viewPATH);
        dispatcher.forward(request, response);
    }
}
 ```
__νμ μ μ₯ μ»¨νΈλ‘€λ¬__
```java
public class MemberSaveControllerV1 implements ControllerV1 {
    private MemberRepository memberRepository = MemberRepository.getInstance();

    @Override
    public void process(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        String username = request.getParameter("username");
        int age = Integer.parseInt(request.getParameter("age"));

        Member member = new Member(username, age);
        memberRepository.save(member);
        
        request.setAttribute("member", member); //Modelμ λ°μ΄ν° λ³΄κ΄

        String viewPATH = "/WEB-INF/views/save-result.jsp";
        RequestDispatcher dispatcher = request.getRequestDispatcher(viewPATH);
        dispatcher.forward(request, response);
    }
}
```

**νμ λͺ©λ‘ μ»¨νΈλ‘€λ¬**
```java
public class MemberListControllerV1 implements ControllerV1{

    private MemberRepository memberRepository = MemberRepository.getInstance();

    @Override
    public void process(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        List<Member> members = memberRepository.findAll();

        request.setAttribute("members", members);

        String viewPath = "/WEB-INF/views/members.jsp";
        RequestDispatcher dispatcher = request.getRequestDispatcher(viewPath);
        dispatcher.forward(request, response);
    }
}
```

**νλ‘ νΈ μ»¨νΈλ‘€λ¬**
```java
@WebServlet(name = "frontControllerServeltV1", urlPatterns = "/front-controller/v1/*") // *μ μ΄λ€ URLμ΄ λ€μ΄μλ ν΄λΉ μλΈλ¦Ώ λ¬΄μ‘°κ±΄ νΈμΆλμ΄μ λ§€νλλ μλ¦¬
public class FrontControllerServletV1 extends HttpServlet {

    // λ§€ν μ λ³΄
    private Map<String, ControllerV1> controllerMap = new HashMap<>();

    // μλΈλ¦Ώ μμ±μ λ§€ν μ λ³΄ κ°μ²΄ λ―Έλ¦¬ μ μ₯, ν΄λΉ λ°μ΄ν° μ‘°νν΄μ μ¬μ© κ°λ₯
    public FrontControllerServletV1() {
        controllerMap.put("/front-controller/v1/members/new-form", new MemberFormControllerV1());
        controllerMap.put("/front-controller/v1/members/save", new MemberSaveControllerV1());
        controllerMap.put("/front-controller/v1/members/members", new MemberListControllerV1());
    }

    @Override
    protected void service(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
         System.out.println("FrontControllerServletV1.service"); // test

        String requestURI = request.getRequestURI();
        ControllerV1 controller = controllerMap.get(requestURI);

        if (controller == null){
            response.setStatus(HttpServletResponse.SC_NOT_FOUND);
            return;
        }

        controller.process(request, response);
    }
}
```

- urlPatterns
  - urlPatterns = "/front-controller/v1/*" : /front-controller/v1 λ₯Ό ν¬ν¨ν νμ λͺ¨λ  μμ²­μ μ΄ μλΈλ¦Ώμμ λ°μλ€μλλ€.
  - μ) /front-controller/v1 , /front-controller/v1/a , /front-controller/v1/a/b
- controllerMap
  - key: λ§€ν URL
  - value: νΈμΆλ  μ»¨νΈλ‘€λ¬
- service()
  - λ¨Όμ  requestURI λ₯Ό μ‘°νν΄μ μ€μ  νΈμΆν  μ»¨νΈλ‘€λ¬λ₯Ό controllerMap μμ μ°Ύμ΅λλ€. λ§μ½ μλ€λ©΄ 404(SC_NOT_FOUND) μν μ½λλ₯Ό λ°νν©λλ€.
  - μ»¨νΈλ‘€λ¬λ₯Ό μ°Ύκ³  controller.process(request, response); μ νΈμΆν΄μ ν΄λΉ μ»¨νΈλ‘€λ¬λ₯Ό μ€νν©λλ€.


#### View λΆλ¦¬ - v2
λͺ¨λ  μ»¨νΈλ‘€λ¬μμ μ΄λνλ λΆλΆμ μ€λ³΅μ΄ μκ³  κΉλνμ§ μμ΅λλ€.
```java
String viewPath = "/WEB-INF/views/members.jsp";
RequestDispatcher dispatcher = request.getRequestDispatcher(viewPath);
dispatcher.forward(request, response);
```
μ΄ λΆλΆμ κΉλνκ² λΆλ¦¬νκΈ° μν΄ λ³λλ‘ λ·°λ₯Ό μ²λ¦¬νλ κ°μ²΄λ₯Ό λ§λ€κ² μ΅λλ€.
κ΅¬μ‘°λ λ€μκ³Ό κ°μ΄ λ³κ²½λ©λλ€.

1. ν΄λΌμ΄μΈνΈκ° HTTP μμ²­ μ FrontControllerλΌλ μλΈλ¦Ώμ΄ μμ²­μ μ λ¬λ°μ΅λλ€.
   - μμ²­ λ©μμ§μμ URL λ§€ν μ λ³΄λ₯Ό κΈ°λ°μΌλ‘ νμν μ»¨νΈλ‘€λ¬λ₯Ό μ‘°νν©λλ€.
2. ν΄λΉ μ»¨νΈλ‘€λ¬λ₯Ό νΈμΆν©λλ€.
3. μ»¨νΈλ‘€λ¬κ° μμ μ λ‘μ§(forward)μ μ§μ  μ²λ¦¬νμ§ μμ΅λλ€. λμ  view μ­ν μ νλ κ°μ²΄λ₯Ό λ°νν©λλ€.
4. νλ‘ νΈ μ»¨νΈλ‘€λ¬κ° ν΄λΉ κ°μ²΄μ render() λ©μλλ₯Ό νΈμΆνλ©΄ JSPλ‘ μ λ¬(forward)ν©λλ€.

![v2](https://images.velog.io/images/urtimeislimited/post/8eeed517-f449-4405-be2d-8070455bdb19/image.png)

λ€λ₯Έ κ³³μμ μ¬μ©λ  λ·° κ°μ²΄λ
```java
public class MyView {
    private String viewPath;

    public MyView(String viewPath) {
        this.viewPath = viewPath;
    }

    public void render(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        RequestDispatcher dispatcher = request.getRequestDispatcher(viewPath);
        dispatcher.forward(request, response);
    }
}
```

μ»¨νΈλ‘€λ¬ μΈν°νμ΄μ€λ₯Ό ν΅ν΄ μ μ§μ μΌλ‘ κ΅¬νλ©λλ€.
```java
public interface ControllerV2 {
     MyView process(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException;
}
```
νμλ±λ‘
```java
public class MemberFormControllerV2 implements ControllerV2 {
    @Override
    public MyView process(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        /**
        String viewPATH = "/WEB-INF/views/new-form.jsp";
        RequestDispatcher dispatcher = request.getRequestDispatcher(viewPATH);
        dispatcher.forward(request, response);
        */

        /**
        MyView myView = new MyView("/WEB-INF/views/new-form.jsp");
        return myView;
         */

        // Ctrl Alt n (inline method)
        return new MyView("/WEB-INF/views/new-form.jsp");
    }
}
```
μ΄μ  λ³΅μ‘ν dispatcher.forward μμ± νΈμΆκ°μ λ‘μ§μ΄ νμμμ΄μ‘μ΅λλ€. λ¨μν MyView κ°μ²΄λ₯Ό μμ±νκ³  κ±°κΈ°μ λ·° μ΄λ¦λ§ μ§μ νμ¬ λ°νλ°μΌλ©΄ λ©λλ€.

ControllerV1μ λΉν΄ ControllerV2λ₯Ό κ΅¬νν ν΄λμ€λ μ΄λ¬ν μ€λ³΅μ΄ νμ€ν μ κ±°λμμμ νμΈν  μ μμ΅λλ€.

```java
public class MemberSaveControllerV2 implements ControllerV2 {
    private MemberRepository memberRepository = MemberRepository.getInstance();

    @Override
    public MyView process(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        String username = request.getParameter("username");
        int age = Integer.parseInt(request.getParameter("age"));

        Member member = new Member(username, age);
        memberRepository.save(member);

        request.setAttribute("member", member); //Modelμ λ°μ΄ν° λ³΄κ΄

        /**
         String viewPATH = "/WEB-INF/views/save-result.jsp";
         RequestDispatcher dispatcher = request.getRequestDispatcher(viewPATH);
         dispatcher.forward(request, response);
         */

        return new MyView("/WEB-INF/views/save-result.jsp");
    }
}
```
νμ λͺ©λ‘
```java
public class MemberListControllerV2 implements ControllerV2 {
    private MemberRepository memberRepository = MemberRepository.getInstance();

    @Override
    public MyView process(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {

        List<Member> members = memberRepository.findAll();
        request.setAttribute("members", members);
        return new MyView("/WEB-INF/views/members.jsp");

        /**
         String viewPath = "/WEB-INF/views/members.jsp";
         RequestDispatcher dispatcher = request.getRequestDispatcher(viewPath);
         dispatcher.forward(request, response);
         */
    }
}

```

νλ‘ νΈ μ»¨νΈλ‘€λ¬
```java
@WebServlet(name = "frontControllerServeltV2", urlPatterns = "/front-controller/v5/*") // *μ μ΄λ€ URLμ΄ λ€μ΄μλ ν΄λΉ μλΈλ¦Ώ λ¬΄μ‘°κ±΄ νΈμΆλμ΄μ λ§€νλλ μλ¦¬
public class FrontControllerServletV2 extends HttpServlet {

    // λ§€ν μ λ³΄
    private Map<String, ControllerV2> controllerMap = new HashMap<>();

    // μλΈλ¦Ώ μμ±μ λ§€ν μ λ³΄ κ°μ²΄ λ―Έλ¦¬ μ μ₯, ν΄λΉ λ°μ΄ν° μ‘°νν΄μ μ¬μ© κ°λ₯
    public FrontControllerServletV2() {
        controllerMap.put("/front-controller/v2/members/new-form", new MemberFormControllerV2());
        controllerMap.put("/front-controller/v2/members/save", new MemberSaveControllerV2());
        controllerMap.put("/front-controller/v2/members/members", new MemberListControllerV2());
    }

    @Override
    protected void service(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        System.out.println("FrontControllerServletV2.service"); // test

        String requestURI = request.getRequestURI();
        ControllerV2 controller = controllerMap.get(requestURI);

        if (controller == null){
            response.setStatus(HttpServletResponse.SC_NOT_FOUND);
            return;
        }
        
        MyView view = controller.process(request, response);
        view.render(request, response);
    }
}
```
ControllerV2μ λ°ν νμμ΄ MyView μ΄λ―λ‘ νλ‘ νΈ μ»¨νΈλ‘€λ¬λ μ»¨νΈλ‘€λ¬μ νΈμΆ κ²°κ³Όλ‘ MyViewλ₯Ό λ°μ΅λλ€. 
- view.reinder()λ₯Ό νΈμΆνλ©΄ forward λ‘μ§μ μνν΄μ JSPκ° μ€νλ©λλ€.

>νλ‘ νΈ μ»¨νΈλ‘€λ¬μ λμμΌλ‘ MyView κ°μ²΄μ render() νΈμΆ μ­ν μ λͺ¨λ μΌκ΄λκ² μ²λ¦¬ν  μ μμ΅λλ€. κ°κ°μ μ»¨νΈλ‘€λ¬λ μ€μ§ MyView κ°μ²΄λ₯Ό μμ±, λ°ννλ©΄ λ©λλ€.

#### Model μΆκ° - v3

- μλΈλ¦Ώ μ’μμ± μ κ±°
  - μ»¨νΈλ‘€λ¬ μμ₯μμ HttpServletRequest, HttpServletResponseκ° κΌ­ νμν μ§ κ³ λ―Όν΄λ΄μΌ ν©λλ€.
  - μμ²­ νλΌλ―Έν° μ λ³΄λ μλ°μ MapμΌλ‘ λμ  λκΈ°λλ‘ νλ©΄ μ§κΈ κ΅¬μ‘°μμλ **μ»¨νΈλ‘€λ¬κ° μλΈλ¦Ώ κΈ°μ μ λͺ°λΌλ λμν  μ μμ΅λλ€.**
  - request κ°μ²΄λ₯Ό Modelλ‘ μ¬μ©νλ λμ  λ³λμ Model κ°μ²΄λ₯Ό λ§λ€μ΄μ λ°ννλ©΄ λ©λλ€.
  - **κ΅¬ννλ μ»¨νΈλ‘€λ¬κ° μλΈλ¦Ώ κΈ°μ μ μ ν μ¬μ©νμ§ μλλ‘ λ³κ²½νλ©΄ κ΅¬ν μ½λλ λ§€μ° λ¨μν΄μ§κ³ , νμ€νΈ μ½λ μμ±μ΄ μ½μ΅λλ€.**
  
- λ·° μ΄λ¦ μ€λ³΅ μ κ±°
  - μ»¨νΈλ‘€λ¬μμ μ§μ νλ λ·° μ΄λ¦μ μ€λ³΅μ΄ μλ κ²μ νμΈν  μ μμ΅λλ€.
  - μ»¨νΈλ‘€λ¬λ "λ·°μ λΌλ¦¬ μ΄λ¦"μ λ³ννκ³ , μ€μ  λ¬Όλ¦¬ μμΉμ μ΄λ¦μ νλ‘ νΈ μ»¨νΈλ‘€λ¬μμ μ²λ¦¬νλλ‘ λ¨μνν©λλ€.
  - μ΄λ κ² ν΄λλ©΄ ν₯ν **λ·°μ ν΄λ μμΉκ²½λ‘κ° ν¨κ» λ³κ²½λλλΌλ νλ‘ νΈ μ»¨νΈλ‘€λ¬λ§ κ³ μΉλ©΄ λ©λλ€.** μ¦, λ³κ²½ μ§μ μ΄ ν΅μΌλμ΄ λμν  μ μλ μ’μ μ€κ³μλλ€.

>
- "/WEB-INF/views/new-form.jsp" -> **new-form**
- "/WEB-INF/views/save-result.jsp" -> **save-result**
- "/WEB-INF/views/members.jsp" ->** members**

λ³κ²½λ κ΅¬μ‘°λ λ€μκ³Ό κ°μ΅λλ€.
1. ν΄λΌμ΄μΈνΈμ HTTP μμ²­ -> λ§€ν μ λ³΄ μ»¨νΈλ‘€λ¬ μ‘°ν
2. μ»¨νΈλ‘€λ¬ νΈμΆ
3. κΈ°μ‘΄μ view κ°μ²΄λ§ λ°ννλ κ²κ³Ό λ¬λ¦¬ modelκ³Ό viewκ° ν¨κ» ν¬ν¨λμ΄μλ ModelViewλ₯Ό λ°νν©λλ€.
4. "λ·°μ λ¬Όλ¦¬ μμΉ"λ₯Ό κ΄λ¦¬νλ μ»¨νΈλ‘€λ¬μμ "λ·°μ λΌλ¦¬ μ΄λ¦"μ λ°ννμ¬ νλ‘ νΈ μ»¨νΈλ‘€λ¬μμ λ¨μνκ² μ²λ¦¬ν©λλ€.

![v3 κ΅¬μ‘°](https://images.velog.io/images/urtimeislimited/post/27e21e1f-58f3-46ab-86b8-eb18db87e655/image.png)

ModelView
μ§κΈκΉμ§ μ»¨νΈλ‘€λ¬μμ μλΈλ¦Ώμ μ’μμ μΈ HttpServletRequestλ₯Ό μ¬μ©νμ΅λλ€. κ·Έλ¦¬κ³  Modelλ request.setAttribute()λ₯Ό ν΅ν΄ λ°μ΄ν°λ₯Ό μ μ₯νκ³  λ·°μ μ λ¬νμ΅λλ€. μλΈλ¦Ώμ μ’μμ±μ μ κ±°νκΈ° μν΄ Modelμ μ§μ  λ§λ€κ³ , μΆκ°λ‘ View μ΄λ¦κΉμ§ μ λ¬νλ κ°μ²΄λ₯Ό λ§λ€μ΄ λ³΄κ² μ΅λλ€.

```java
public class ModelView {
    private String viewName;
    private Map<String, Object> model = new HashMap<>();

    public ModelView(String viewName) {
        this.viewName = viewName;
    }

    public String getViewName() {
        return viewName;
    }

    public void setViewName(String viewName) {
        this.viewName = viewName;
    }

    public Map<String, Object> getModel() {
        return model;
    }

    public void setModel(Map<String, Object> model) {
        this.model = model;
    }
}
```
λ·°μ μ΄λ¦κ³Ό λ·°λ₯Ό λ λλ§ν  λ νμν model κ°μ²΄λ₯Ό κ°μ§κ³  μμ΅λλ€. modelμ λ¨μν mapμΌλ‘ κ΅¬μ±λμ΄ μμΌλ―λ‘ μ»¨νΈλ‘€λ¬μμ λ·°μ νμν λ°μ΄ν°λ₯Ό key, valueλ‘ λ£μ΄μ£Όλ©΄ λ©λλ€.

ControllerV3
```java
public interface ControllerV3 {
    ModelView process(Map<String, String> paramMap); // μλΈλ¦Ώ μ’μμ± μ κ±°
}
```
μ΄ μ»¨νΈλ‘€λ¬λ μλΈλ¦Ώ κΈ°μ μ μ ν μ¬μ©νμ§ μκΈ° λλ¬Έμ κ΅¬νμ΄ λ§€μ° λ¨μν΄μ§κ³ , νμ€νΈ μ½λ μμ±μ νμ€νΈνκΈ° μ½μ΅λλ€.
HttpServletRequestκ° μ κ³΅νλ νλΌλ―Έν°λ νλ‘ νΈ μ»¨νΈλ‘€λ¬κ° paramMapμ λ΄μμ νΈμΆν΄μ£Όλ©΄ λ©λλ€. μλ΅ κ²°κ³Όλ‘ λ·° μ΄λ¦κ³Ό λ·°μ μ λ¬ν  Model λ°μ΄ν°λ₯Ό ν¬ν¨νλ ModelViewκ°μ²΄λ₯Ό λ°ννλ©΄ λ©λλ€.

νμ λ±λ‘ νΌ
```java
@WebServlet(name = "mvcMemberFormServlet", urlPatterns = "/servlet-mvc/members/new-form")
public class MvcMemberFormServlet extends HttpServlet {
    @Override
    protected void service(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        String viewPath = "/WEB-INF/views/new-form.jsp";
        RequestDispatcher dispatcher = request.getRequestDispatcher(viewPath);
        dispatcher.forward(request, response);
    }
}
```
ModelViewλ₯Ό μμ±ν  λ new-formμ΄λΌλ viewμ λΌλ¦¬μ μΈ μ΄λ¦μ μ§μ ν©λλ€.
μ€μ  λ¬Όλ¦¬μ μΈ μ΄λ¦μ νλ‘ νΈ μ»¨νΈλ‘€λ¬μμ μ²λ¦¬ν©λλ€.

νμμ μ₯
```java
@WebServlet(name = "mvcMemberSaveServlet", urlPatterns = "/servlet-mvc/members/save")
public class MvcMemberSaveServlet extends HttpServlet {

    private MemberRepository memberRepository = MemberRepository.getInstance();

    @Override
    protected void service(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {

        String username = request.getParameter("username");
        int age = Integer.parseInt(request.getParameter("age"));

        Member member = new Member(username, age);
        memberRepository.save(member);

        //Modelμ λ°μ΄ν°λ₯Ό λ³΄κ΄
        request.setAttribute("member", member);

        String viewPath = "/WEB-INF/views/save-result.jsp";
        RequestDispatcher dispatcher = request.getRequestDispatcher(viewPath);
        dispatcher.forward(request, response);
    }
}
```
- paramMap.get("username");
νλΌλ―Έν° μ λ³΄λ mapμ λ΄κ²¨μμ΅λλ€. mapμμ νμν μμ²­ νλΌλ―Έν°λ₯Ό μ‘°ννλ©΄ λ©λλ€.
- mv.getModel().put("member", member);
λͺ¨λΈμ λ¨μν mapμ΄λ―λ‘ λͺ¨λΈμ λ·°μμ νμν member κ°μ²΄λ₯Ό λ΄κ³  λ°νν©λλ€.

FrontControllerServletV3
```java
@WebServlet(name = "frontControllerServeltV3", urlPatterns = "/front-controller/v3/*") // *μ μ΄λ€ URLμ΄ λ€μ΄μλ ν΄λΉ μλΈλ¦Ώ λ¬΄μ‘°κ±΄ νΈμΆλμ΄μ λ§€νλλ μλ¦¬
public class FrontControllerServletV3 extends HttpServlet {

    // λ§€ν μ λ³΄
    private Map<String, ControllerV3> controllerMap = new HashMap<>();

    // μλΈλ¦Ώ μμ±μ λ§€ν μ λ³΄ κ°μ²΄ λ―Έλ¦¬ μ μ₯, ν΄λΉ λ°μ΄ν° μ‘°νν΄μ μ¬μ© κ°λ₯
    public FrontControllerServletV3() {
        controllerMap.put("/front-controller/v3/members/new-form", new MemberFormControllerV3());
        controllerMap.put("/front-controller/v3/members/save", new MemberSaveControllerV3());
        controllerMap.put("/front-controller/v3/members/members", new MemberListControllerV3());
    }

    @Override
    protected void service(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        System.out.println("FrontControlControllerV3.service"); // test

        String requestURI = request.getRequestURI();
        ControllerV3 controller = controllerMap.get(requestURI);

        if (controller == null){
            response.setStatus(HttpServletResponse.SC_NOT_FOUND);
            return;
        }

        //paramMap
        /**
         * Map<String, String> paramMap = new HashMap<>();
         *         request.getParameterNames().asIterator()
         *                 .forEachRemaining(paramName -> paramMap.put(paramName, request.getParameter(paramName)));
         */

        Map<String, String> paramMap = createParamMap(request);

        ModelView mv = controller.process(paramMap);
        String viewName = mv.getViewName();// λΌλ¦¬ μ΄λ¦ new-form
        /**
         // /WEB-INF/views/new-form.jsp
         MyView view = new MyView("/WEB-INF/views/" + viewName + ".jsp");
         view.render(request, response);
         */
        // /WEB-INF/views/new-form.jsp
        MyView view = viewResolver(viewName);

        view.render(mv.getModel(), request, response);
    }

    private MyView viewResolver(String viewName) {
        return new MyView("/WEB-INF/views/" + viewName + ".jsp");
    }

    private Map<String, String> createParamMap(HttpServletRequest request) {
        Map<String, String> paramMap = new HashMap<>();
        request.getParameterNames().asIterator()
                .forEachRemaining(paramName -> paramMap.put(paramName, request.getParameter(paramName)));
        return paramMap;
    }
}
```
- createParamMap()
HttpServletRequestμμ νλΌλ―Έν° μ λ³΄λ₯Ό κΊΌλ΄μ MapμΌλ‘ λ³νν©λλ€. κ·Έλ¦¬κ³  ν΄λΉ Map( paramMap )μ μ»¨νΈλ‘€λ¬μ μ λ¬νλ©΄μ νΈμΆν©λλ€.
- view.render(mv.getModel(), request, response) μ½λμμ μ»΄νμΌ μ€λ₯κ° λ°μν  κ²μλλ€. λ€μ μ½λλ₯Ό μ°Έκ³ ν΄μ MyView κ°μ²΄μ νμν λ©μλλ₯Ό μΆκ°ν©λλ€.

λ·° λ¦¬μ‘Έλ²

```MyView view = viewResolver(viewName)```
- μ»¨νΈλ‘€λ¬κ° λ°νν λΌλ¦¬ λ·° μ΄λ¦μ μ€μ  λ¬Όλ¦¬ λ·° κ²½λ‘λ‘ λ³κ²½νκ³ , μ€μ  λ¬Όλ¦¬ κ²½λ‘κ° μλ MyView 
κ°μ²΄λ₯Ό λ°νν©λλ€.
- λΌλ¦¬ λ·° μ΄λ¦: members
- λ¬Όλ¦¬ λ·° κ²½λ‘: /WEB-INF/views/members.jsp
view.render(mv.getModel(), request, response)
- λ·° κ°μ²΄λ₯Ό ν΅ν΄μ HTML νλ©΄μ λ λλ§ ν©λλ€.
- λ·° κ°μ²΄μ render() λ λͺ¨λΈ μ λ³΄λ ν¨κ» λ°μ΅λλ€.
- JSPλ request.getAttribute() λ‘ λ°μ΄ν°λ₯Ό μ‘°ννκΈ° λλ¬Έμ, λͺ¨λΈμ λ°μ΄ν°λ₯Ό κΊΌλ΄μ
- request.setAttribute() λ‘ λ΄μλ‘λλ€.
- JSPλ‘ ν¬μλ ν΄μ JSPλ₯Ό λ λλ§ ν©λλ€.

MyView
```java
public class MyView {
    private String viewPath;

    public MyView(String viewPath) {
        this.viewPath = viewPath;
    }

    public void render(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        RequestDispatcher dispatcher = request.getRequestDispatcher(viewPath);
        dispatcher.forward(request, response);
    }

    public void render(Map<String, Object> model, HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException{
        modelToRequesetAttribute(model, request);
        RequestDispatcher dispatcher = request.getRequestDispatcher(viewPath);
        dispatcher.forward(request, response);
    }

    private void modelToRequesetAttribute(Map<String, Object> model, HttpServletRequest request) {
        model.forEach((key, value) -> request.setAttribute(key, value));
    }
}
```

#### λ¨μνκ³  μ€μ©μ μΈ μ»¨νΈλ‘€λ¬ - v4
μμ λ§λ  v3 μ»¨νΈλ‘€λ¬λ μλΈλ¦Ώ μ’μμ±μ μ κ±°νκ³  λ·° κ²½λ‘μ μ€λ³΅μ μ κ±°νλ λ±, μ μ€κ³λ μ»¨νΈλ‘€λ¬μλλ€. κ·Έλ°λ° μ€μ  μ»¨νΈλ‘€λ¬ μΈν°νμ΄μ€λ₯Ό κ΅¬ννλ κ°λ°μ μμ₯μμ λ³΄λ©΄, ν­μ ModelView κ°μ²΄λ₯Ό μμ±νκ³  λ°νν΄μΌ νλ λΆλΆμ΄ μ‘°κΈμ λ²κ±°λ‘­μ΅λλ€.
μ’μ νλ μμν¬λ μν€νμ³λ μ€μνμ§λ§, κ·Έμ λλΆμ΄ μ€μ  κ°λ°νλ κ°λ°μκ° λ¨μνκ³  νΈλ¦¬νκ² μ¬μ©ν  μ μμ΄μΌ ν©λλ€. μμ μ€μ©μ±μ΄ μμ΄μΌ ν©λλ€.

v3λ₯Ό μ‘°κΈ λ³κ²½ν΄μ μ€μ  κ΅¬ννλ κ°λ°μλ€μ΄ λ§€μ° νΈλ¦¬νκ² κ°λ°ν  μ μλ v4 λ²μ μ κ°λ°ν΄λ³΄κ² μ΅λλ€.

![v4](https://images.velog.io/images/urtimeislimited/post/51b02f1c-3a05-4405-b00b-d5f8be21d563/image.png)
- κΈ°λ³Έμ μΈ κ΅¬μ‘°λ v3μ κ°μ΅λλ€. 
λμ  μ»¨νΈλ‘€λ¬κ° ModelViewλ₯Ό λ°ννμ§ μκ³ , ViewNameλ§ λ°νν©λλ€.

ControllerV4
```java
public interface ControllerV4 {
    /**
     *
     * @param paramMap
     * @param model
     * @return viewName
     */
    String process(Map<String, String> paramMap, Map<String, Object> model);
}
```
- μΈν°νμ΄μ€μ ModelViewκ° μμ΅λλ€.
- model κ°μ²΄λ νλΌλ―Έν°λ‘ μ λ¬λκΈ° λλ¬Έμ κ·Έλ₯ μ¬μ©νλ©΄ λκ³ , κ²°κ³Όλ‘ λ·°μ μ΄λ¦λ§ λ°νν΄μ£Όλ©΄ λ©λλ€. μ€μ  κ΅¬ν μ½λλ₯Ό λ³΄λ©΄

MemberFormControllerV4
```java
public class MemberFormControllerV4 implements ControllerV4 {
    @Override
    public String process(Map<String, String> paramMap, Map<String, Object> model) {
        return "new-form";
    }
}
```
- μ λ§ λ¨μνκ² new-formμ΄λΌλ λ·°μ λΌλ¦¬ μ΄λ¦λ§ λ°ννλ©΄ λ©λλ€.

MemberSaveControllerV4
```java
public class MemberSaveControllerV4 implements ControllerV4 {
    private MemberRepository memberRepository = MemberRepository.getInstance();
    
    @Override
    public String process(Map<String, String> paramMap, Map<String, Object> model) {
        String username = paramMap.get("username");
        int age = Integer.parseInt(paramMap.get("age"));

        Member member = new Member(username, age);
        memberRepository.save(member);

        model.put("member", member);
        return "save-result";
    }
}
```
- λͺ¨λΈμ΄ νλΌλ―Έν°λ‘ μ λ¬λ©λλ€. λͺ¨λΈμ μ§μ  μμ±νμ§ μμλ λ©λλ€.

MemberListControllerV4
```java
public class MemberListControllerV4 implements ControllerV4 {

    private MemberRepository memberRepository = MemberRepository.getInstance();

    @Override
    public String process(Map<String, String> paramMap, Map<String, Object> model) {
        List<Member> members = memberRepository.findAll();

        model.put("members", members);
        return "members";
        /**
        ModelView mv = new ModelView("members");
        mv.getModel().put("members", members);

        return mv;
         */
    }
}
```
FrontControllerServletV4
```java
@WebServlet(name = "frontControllerServeltV4", urlPatterns = "/front-controller/v4/*") // *μ μ΄λ€ URLμ΄ λ€μ΄μλ ν΄λΉ μλΈλ¦Ώ λ¬΄μ‘°κ±΄ νΈμΆλμ΄μ λ§€νλλ μλ¦¬
public class FrontControllerServletV4 extends HttpServlet {

    // λ§€ν μ λ³΄
    private Map<String, ControllerV4> controllerMap = new HashMap<>();

    // μλΈλ¦Ώ μμ±μ λ§€ν μ λ³΄ κ°μ²΄ λ―Έλ¦¬ μ μ₯, ν΄λΉ λ°μ΄ν° μ‘°νν΄μ μ¬μ© κ°λ₯
    public FrontControllerServletV4() {
        controllerMap.put("/front-controller/v4/members/new-form", new MemberFormControllerV4());
        controllerMap.put("/front-controller/v4/members/save", new MemberSaveControllerV4());
        controllerMap.put("/front-controller/v4/members/members",
                new MemberListControllerV4());
    }

    @Override
    protected void service(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        System.out.println("FrontControlControllerV4.service"); // test

        String requestURI = request.getRequestURI();
        ControllerV4 controller = controllerMap.get(requestURI);

        if (controller == null){
            response.setStatus(HttpServletResponse.SC_NOT_FOUND);
            return;
        }


        Map<String, String> paramMap = createParamMap(request);
        /**
        * μΆκ°
        */
        Map<String, Object> model = new HashMap<>(); 
        String viewName = controller.process(paramMap, model);


        // /WEB-INF/views/new-form.jsp
        MyView view = viewResolver(viewName);

        view.render(model, request, response);
    }

    private MyView viewResolver(String viewName) {
        return new MyView("/WEB-INF/views/" + viewName + ".jsp");
    }

    private Map<String, String> createParamMap(HttpServletRequest request) {
        Map<String, String> paramMap = new HashMap<>();
        request.getParameterNames().asIterator()
                .forEachRemaining(paramName -> paramMap.put(paramName, request.getParameter(paramName)));
        return paramMap;
    }
}
```
- **λͺ¨λΈ κ°μ²΄ μ λ¬** : Map<String, Object> model = new HashMap<>(); μΆκ°
- λͺ¨λΈ κ°μ²΄λ₯Ό νλ‘ νΈ μ»¨νΈλ‘€λ¬μμ μμ±ν΄μ λκ²¨μ€λλ€. μ»¨νΈλ‘€λ¬μμ λͺ¨λΈ κ°μ²΄μ κ°μ λ΄μΌλ©΄ μ¬κΈ°μ κ·Έλλ‘ λ΄κ²¨μκ² λ©λλ€.
- **λ·°μ λΌλ¦¬ μ΄λ¦μ μ§μ  λ°ν** : μ»¨νΈλ‘€λ¬κ° μ§μ  λ·°μ λΌλ¦¬ μ΄λ¦μ λ°ννλ―λ‘ μ΄ κ°μ μ¬μ©ν΄μ μ€μ  λ¬Όλ¦¬ λ·°λ₯Ό μ°Ύμ μ μμ΅λλ€.
```java
String viewName = controller.process(paramMap, model);
MyView view = viewResolver(viewName);
```
μ»¨νΈλ‘€λ¬κ° μ§μ  λ·°μ λΌλ¦¬ μ΄λ¦μ λ°ννλ―λ‘ μ΄ κ°μ μ¬μ©ν΄μ μ€μ  λ¬Όλ¦¬ λ·°λ₯Ό μ°Ύμ μ μμ΅λλ€.

μ΄λ² λ²μ μ μ»¨νΈλ‘€λ¬λ **λ§€μ° λ¨μνκ³  μ€μ©μ **μλλ€. **"κΈ°μ‘΄ κ΅¬μ‘°μμ λͺ¨λΈμ νλΌλ―Έν°λ‘ λκΈ°κ³ , λ·°μ λΌλ¦¬ μ΄λ¦μ λ°ννλ€"**λΌλ μμ μμ΄λμ΄λ₯Ό μ μ©νμ λΏμΈλ°, μ»¨νΈλ‘€λ¬λ₯Ό κ΅¬ννλ μμ₯μμ κ΅°λλκΈ° μλ μ½λλ₯Ό μμ±ν  μ μμ΅λλ€.
λν μ¬κΈ°κΉμ§ ν λ²μ μ¨ κ²μ΄ μλλΌ νλ μμν¬κ° μ μ§μ μΌλ‘ λ°μ νλ κ³Όμ  μμμ μ΄λ° λ°©λ²μ μ°Ύμ μ μμμ΅λλ€.
**νλ μμν¬λ κ³΅ν΅ κΈ°λ₯μ΄ μκ³ λ‘μμΌ μ¬μ©νλ κ°λ°μκ° νΈλ¦¬**ν΄μ§λ€κ³  ν©λλ€.

#### μ μ°ν μ»¨νΈλ‘€λ¬1 - v5
λ§μ½ ControllerV3 λ°©μμΌλ‘ κ°λ°νκ³  μΆμ μ¬λκ³Ό, ControllerV4 λ°©μμΌλ‘ κ°λ°νκ³  μΆμ μ¬λμ΄ μλ€λ©΄ μ΄λ»κ² ν΄μΌ ν κΉμ? νλμ νλ‘μ νΈ λ΄μμ λ€μν μ»¨νΈλ‘€λ¬λ₯Ό μ¬μ©νκ³  μΆλ€λ©΄?
```java
public interface ControllerV3 {
 ModelView process(Map<String, String> paramMap);
}
```
```java
public interface ControllerV4 {
 String process(Map<String, String> paramMap, Map<String, Object> model);
}
```
**μ΄λν° ν¨ν΄**μ ν΅ν΄ μμ κ°μ λ¬Έμ λ₯Ό ν΄κ²°ν  μ μμ΅λλ€.

- **μ΄λν° ν¨ν΄**
μ§κΈκΉμ§ κ°λ°ν νλ‘ νΈ μ»¨νΈλ‘€λ¬λ νκ°μ§ λ°©μμ μ»¨νΈλ‘€λ¬ μΈν°νμ΄μ€λ§ μ¬μ©ν  μ μμμ΅λλ€.
  - ControllerV3, ControllerV4λ μμ ν λ€λ₯Έ μΈν°νμ΄μ€μλλ€. λ°λΌμ νΈνμ΄ λΆκ°λ₯ν©λλ€.
  - μλ₯Ό λ€μ΄ 110v, 220v μ κΈ° μ½μΌνΈλ₯Ό κ³΅ν΅μΌλ‘ νΈννκΈ° μν΄ νκ°μ§ μ΄λν°λ₯Ό μ¬μ©νλ κ²μ²λΌ
  - μ΄λν° ν¨ν΄μ μ¬μ©ν΄μ νν€νΈ μ»¨νΈλ‘€λ¬κ° λ€μν λ°©μμ μ»¨νΈλ‘€λ¬λ₯Ό μ²λ¦¬ν  μ μλλ‘ λ³κ²½ν  μ μμ΅λλ€.
  
![v5](https://images.velog.io/images/urtimeislimited/post/be2b60f0-f69c-4073-94c9-4b0782ca1aa4/image.png)

λ΄λΆ κ³Όμ μ μμλ λ€μκ³Ό κ°μ΅λλ€.
1. ν΄λΌμ΄μΈνΈκ° HTTP μμ²­μ νλ‘ ν° μ»¨νΈλ‘€λ¬κ° νΈλ€λ¬(μ»¨νΈλ‘€λ¬) λ§€ν μ λ³΄μμ νΈλ€λ¬λ₯Ό μ‘°νν©λλ€.
2. **νΈλ€λ¬ μ΄ν­ν° λͺ©λ‘μμ νΈλ€λ¬λ₯Ό μ²λ¦¬ν  μ μλ νΈλ€λ¬ μ΄λν°λ₯Ό μ‘°νν©λλ€.**
3. κΈ°μ‘΄ νλ‘ νΈ μ»¨νΈλ‘€λ¬μμ νΈλ€λ¬λ₯Ό λ°λ‘ νΈμΆνλ κ²κ³Ό λ¬λ¦¬, μ μ°ν¨μ μν΄ μ€κ°μμ νΈλ€λ¬ μ΄λν°λ₯Ό ν΅ν΄ νΈλ€λ¬λ₯Ό νΈμΆν©λλ€.
  - νλ‘ νΈ μ»¨νΈλ‘€λ¬μμ νλΌλ―Έν°λ₯Ό μ΄λν°μκ² μ λ¬ν©λλ€.
4. μ΄λν°μμ μ λ¬λ°μ νλΌλ―Έν°μ ν΄λΉνλ νΈλ€λ¬λ₯Ό νΈμΆν©λλ€.
5. νΈλ€λ¬μκ² λ°νλ°μ κ²°κ³Όκ°μ κΈ°λ°μΌλ‘ νλ‘ νΈ μ»¨νΈλ‘€λ¬μκ² ModelViewλ₯Ό λ°νν΄μ€λλ€.
6. ModelViewλ₯Ό λ°μ νλ‘ νΈ μ»¨νΈλ‘€λ¬κ° λ·°μ λΌλ¦¬μ΄λ¦μ μ λ¬νμ¬ viewResolverλ₯Ό νΈμΆν©λλ€.
7. "λ·°μ λ¬Όλ¦¬ μμΉ"λ₯Ό κ΄λ¦¬νλ viewResolverμμ "λ·°μ λΌλ¦¬ μ΄λ¦"μ νλ‘ νΈ μ»¨νΈλ‘€λ¬μκ² λ°νν©λλ€.
8. νλ‘ νΈ μ»¨νΈλ‘€λ¬λ μ λ¬λ°μ "λ·°μ λΌλ¦¬ μ΄λ¦"μ κ°λ¨νκ² μ²λ¦¬νμ¬ κ²°κ³Όλ₯Ό μλ΅ν©λλ€.

- **νΈλ€λ¬** : μ»¨νΈλ‘€λ¬μ μ΄λ¦μ λ λμ λ²μμΈ νΈλ€λ¬λ‘ λ³κ²½ν μ΄μ λ μ΄λν°κ° μκΈ° λλ¬Έμ κΌ­ μ»¨νΈλ‘€λ¬μ κ°λ λΏλ§ μλλΌ μ΄λ ν κ²μ΄λ  ν΄λΉνλ μ’λ₯μ μ΄λν°λ§ μμΌλ©΄ λ€ μ²λ¦¬ν  μ μκΈ° λλ¬Έμλλ€.
- **νΈλ€λ¬ μ΄λν°** : νλ‘ ν° μ»¨νΈλ‘€λ¬μ νΈλ€λ¬ μ€κ°μ μΆκ°λ μ­ν μ μλ―Έν©λλ€. μ΄λν° μ­ν  λλΆμ λ€μν μ’λ₯μ μ»¨νΈλ‘€λ¬λ₯Ό νΈμΆν  μ μμ΅λλ€.

μ΄λν°μ© μΈν°νμ΄μ€λ₯Ό κ΅¬νν΄λ³΄κ² μ΅λλ€.
MyHandlerAdapter
```java
package hello.servlet.web.frontcontroller.v5;

public interface MyHandlerAdapter {
    boolean supports(Object handler);
    ModelView handle(HttpServletRequest request, HttpServletResponse response, Object handler) throws ServletException, IOException;
}
```
- boolean supports(Object handler)
  - handlerλ μ»¨νΈλ‘€λ¬λ₯Ό λ§ν©λλ€.
  - μ΄λν°κ° ν΄λΉ μ»¨νΈλ‘€λ¬λ₯Ό μ²λ¦¬ν  μ μλμ§ νλ¨νλ λ©μλ μλλ€.
- ModelView handle(HttpServletRequest request, HttpServletResponse response, Object handler)
  - μ΄λν°λ μ€μ  μ»¨νΈλ‘€λ¬λ₯Ό νΈμΆνκ³ , κ·Έ κ²°κ³Όλ‘ ModelViewλ₯Ό λ°νν΄μΌ ν©λλ€.
  - μ€μ  μ»¨νΈλ‘€λ¬κ° ModelViewλ₯Ό λ°ννμ§ λͺ»νλ©΄, μ΄λν°κ° ModelViewλ₯Ό μ§μ  μμ±ν΄μλΌλ λ°νν΄μΌ ν©λλ€.
  - μ΄μ μλ νλ‘ νΈ μ»¨νΈλ‘€λ¬κ° μ€μ  μ»¨νΈλ‘€λ¬λ₯Ό νΈμΆνμ§λ§ μ΄μ  μ΄ μ΄λν°λ₯Ό ν΅ν΄μ μ€μ  μ»¨νΈλ‘€λ¬κ° νΈμΆλ©λλ€.
  
μ€μ  μ΄λν° κ΅¬νμ μν΄ λ¨Όμ  ControllerV3λ₯Ό μ§μνλ μ΄λν°λ₯Ό νλμ© κ΅¬νν΄λ³΄κ² μ΅λλ€.
``` java
public boolean supports(Object handler) {
 return (handler instanceof ControllerV3);
}
```
- ControllerV3λ₯Ό μ²λ¦¬ν  μ μλ μ΄λν°μλλ€.
```java
        ControllerV3 controller = (ControllerV3) handler; // νΈλ€λ¬λ₯Ό controllerV3λ‘ μΊμ€ν
        Map<String, String> paramMap = createParamMap(request);
        ModelView mv = controller.process(paramMap);
        return mv;
```
- handlerλ₯Ό μ»¨νΈλ‘€λ¬ V3λ‘ λ³νν λ€μ V3 νμμ λ§λλ‘ νΈμΆν©λλ€.
- supports()λ₯Ό ν΅ν΄ ControllerV3λ§ μ§μνκΈ° λλ¬Έμ νμ λ³ν κ±±μ μμ΄ μ€νν΄λ λ©λλ€.
- ControllerV3λ ModelViewλ₯Ό λ°ννλ―λ‘ κ·Έλλ‘ ModelViewλ₯Ό λ°ννλ©΄ λ©λλ€.


```java
public class ControllerV3HandlerAdapter implements MyHandlerAdapter {
    @Override
    public boolean supports(Object handler) {
        return (handler instanceof ControllerV3); // νΈλ€λ¬λ V3μ μΈμ€ν΄μ€
    }
    @Override
    public ModelView handle(HttpServletRequest request, HttpServletResponse response, Object handler) throws ServletException, IOException {
        ControllerV3 controller = (ControllerV3) handler; // νΈλ€λ¬λ₯Ό controllerV3λ‘ μΊμ€ν
        Map<String, String> paramMap = createParamMap(request);
        ModelView mv = controller.process(paramMap);
        return mv;
    }
    private Map<String, String> createParamMap(HttpServletRequest request) {
        Map<String, String> paramMap = new HashMap<>();
        request.getParameterNames().asIterator()
                .forEachRemaining(paramName -> paramMap.put(paramName, request.getParameter(paramName)));
        return paramMap;
    }
}
```

**FrontControllerServletV5**
```java
@WebServlet(name = "frontControllerServletV5", urlPatterns = "/front-controller/v5/*")
public class FrontControllerServletV5 extends HttpServlet {
    // λͺ¨λ  μ»¨νΈλ‘€λ¬ μ§μ μν΄ Object μ¬μ©
    private final Map<String, Object> handlerMappingMap = new HashMap<>();
    private final List<MyHandlerAdapter> handlerAdapters = new ArrayList<>();

    public FrontControllerServletV5() {
        initHandlerMappingMap();
        initHandlerAdapters();
    }

    private void initHandlerAdapters() {
        handlerAdapters.add(new ControllerV3HandlerAdapter());
    }

    private void initHandlerMappingMap() {
        handlerMappingMap.put("/front-controller/v5/v3/members/new-form", new MemberFormControllerV3());
        handlerMappingMap.put("/front-controller/v5/v3/members/save", new MemberSaveControllerV3());
        handlerMappingMap.put("/front-controller/v5/v3/members/members", new MemberListControllerV3());
    }

    @Override
    protected void service(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        Object handler = getHandler(request);
        if (handler == null){
            response.setStatus(HttpServletResponse.SC_NOT_FOUND);
            return;
        }

        MyHandlerAdapter adapter = getHandlerAdapter(handler);
        ModelView mv = adapter.handle(request, response, handler);

        MyView view = viewResolver(mv.getViewName());
        view.render(mv.getModel(), request, response);
    }

    private Object getHandler(HttpServletRequest request) {
        String requestURI = request.getRequestURI();
        return handlerMappingMap.get(requestURI);
    }

    private MyHandlerAdapter getHandlerAdapter(Object handler) {
        for (MyHandlerAdapter adapter : handlerAdapters) {
            if (adapter.supports(handler)) {
                return adapter;
            }
        }
        throw new IllegalArgumentException("handler adapterλ₯Ό μ°Ύμ μ μμ΅λλ€. handler= " + handler);
    }

    private MyView viewResolver(String viewName){
        return new MyView("/WEB-INF/views/" + viewName + ".jsp");
    }
}
```
- **μ»¨νΈλ‘€λ¬(Controller)  -> νΈλ€λ¬(Handler)**
μ΄μ μ μ»¨νΈλ‘€λ¬λ₯Ό μ§μ  λ§€νν΄μ μ¬μ©νμ§λ§ μ΄λν°λ₯Ό μ¬μ©νκ² λλ©΄ μ»¨νΈλ‘€λ¬ λΏλ§ μλλΌ μ΄λν°κ° μ§μνλ μ΄λ€ κ²μ΄λΌλ URLμ λ§€νν΄μ μ¬μ©ν  μ μμ΅λλ€. μ΄λ¦μ μ»¨νΈλ‘€λ¬μμ λ λμ λ²μμ νΈλ€λ¬λ‘ λ³κ²½ν μ΄μ μλλ€.

μμ±μ
```java
public FrontControllerServletV5() {
        initHandlerMappingMap(); // νΈλ€λ¬ λ§€ν μ΄κΈ°ν
        initHandlerAdapters(); // μ΄λν° μ΄κΈ°ν
    }
```
 - μμ±μλ νΈλ€λ¬ λ§€νκ³Ό μ΄λν°λ₯Ό μ΄κΈ°ν(λ±λ‘)ν©λλ€.

λ§€ν μ λ³΄
```private final Map<String, Object> handlerMappingMap = new HashMap<>();```
- λ§€ν μ λ³΄μ κ°μ΄ ControllerV3 , ControllerV4 κ°μ μΈν°νμ΄μ€μμ μλ¬΄ κ°μ΄λ λ°μ μ μλ Object λ‘ λ³κ²½λμμ΅λλ€.

νΈλ€λ¬ λ§€ν
```Object handler = getHandler(request); // Extract Method```
```java
    private Object getHandler(HttpServletRequest request) {
        String requestURI = request.getRequestURI();
        return handlerMappingMap.get(requestURI);
    }
```
- νΈλ€λ¬ λ§€ν μ λ³΄μΈ handlerMappingMapμμ URLμ λ§€νλ νΈλ€λ¬(μ»¨νΈλ‘€λ¬) κ°μ²΄λ₯Ό μ°Ύμμ λ°νν©λλ€.

νΈλ€λ¬λ₯Ό μ²λ¦¬ν  μ μλ μ΄λν° μ‘°ν
```MyHandlerAdapter adapter = getHandlerAdapter(handler); // Extract Method```
```java
for (MyHandlerAdapter adapter : handlerAdapters) {
            if (adapter.supports(handler)) {
                return adapter;
            }
        }
```
- handlerλ₯Ό μ²λ¦¬ν  μ μλ μ΄λν°λ₯Ό adapter.supports(handler)λ₯Ό ν΅ν΄μ μ°Ύμ΅λλ€.
- handlerκ° ControllerV3 μΈν°νμ΄μ€λ₯Ό κ΅¬ννλ€λ©΄, ControllerV3HandlerAdapter κ°μ²΄κ° λ°νλ©λλ€.

μ΄λν° νΈμΆ
```ModelView mv = adapter.handle(request, response, handler); // Extract Method```

μ΄λν°μ handle(request, response, handler) λ©μλλ₯Ό ν΅ν΄ μ€μ  μ΄λν°κ° νΈμΆλ©λλ€.
μ΄λν°λ handler(μ»¨νΈλ‘€λ¬)λ₯Ό νΈμΆνκ³  κ·Έ κ²°κ³Όλ₯Ό μ΄λν°μ λ§μΆμ΄ λ°νν©λλ€.
ControllerV3HandlerAdapterμ κ²½μ° μ΄λν°μ λͺ¨μκ³Ό μ»¨νΈλ‘€λ¬μ λͺ¨μμ΄ μ μ¬ν΄μ λ³ν λ‘μ§μ΄ λ¨μν©λλ€.

μ§κΈμ V3 μ»¨νΈλ‘€λ¬λ₯Ό μ¬μ©ν  μ μλ μ΄λν°μ ControlelrV3λ§ λ€μ΄ μμΌλ ControlelrV4λ₯Ό μ¬μ©ν  μ μλλ‘ κΈ°λ₯μ μΆκ°ν΄λ³΄κ² μ΅λλ€.

#### μ μ°ν μ»¨νΈλ‘€λ¬2 - v5
FrontControllerServletV5μ ControlelrV4 κΈ°λ₯μ νλμ© μΆκ°ν΄λ³΄κ² μ΅λλ€.
```java
    @Override
    public boolean supports(Object handler) {
        return (handler instanceof ControllerV4);
    }
```
- handlerκ° ControlelrV4μ κ°μ²΄μΈ κ²½μ°μλ§ μ²λ¦¬νλ μ΄λν°μλλ€.

μ€ν λ‘μ§
```java
        ControllerV4 controller = (ControllerV4) handler;

        Map<String, String> paramMap = createParamMap(request);
        Map<String, Object> model = new HashMap<>();

        String viewName = controller.process(paramMap, model);
```
- handlerλ₯Ό ControlelrV4λ‘ μΊμ€ν ν©λλ€. - - paramMap, modelμ λ§λ€μ΄μ ν΄λΉ μ»¨νΈλ‘€λ¬λ₯Ό νΈμΆν©λλ€.
- viewNameμ λ°ν λ°μ΅λλ€.

μ΄λν° λ³ν
```java
ModelView mv = new ModelView(viewName);
mv.setModel(model);
return mv;
```
- μ΄λν°κ° νΈμΆνλ ControlelrV4λ λ·°μ μ΄λ¦μ λ°νν©λλ€.
- μ΄λν°λ λ·°μ μ΄λ¦μ΄ μλλΌ ModelViewλ₯Ό λ§λ€μ΄μ λ°νν΄μΌ ν©λλ€.
- μ΄λν°κ° κΌ­ νμν μ΄μ 
  - ControllerV4 λ λ·°μ μ΄λ¦μ λ°ννμ§λ§, μ΄λν°λ μ΄κ²μ ModelViewλ‘ λ§λ€μ΄μ νμμ λ§μΆμ΄ λ°νν©λλ€. λ§μΉ 110v μ κΈ° μ½μΌνΈλ₯Ό 220v μ κΈ° μ½μΌνΈλ‘ λ³κ²½νλ―μ΄!
- **μ΄λν°μμ μ΄ λΆλΆμ λ¨μνμ§λ§ μ€μν λΆλΆμλλ€.**
  
μ΄λν°μ ControllerV4 μ°¨μ΄
```java
public interface ControllerV4 {
 String process(Map<String, String> paramMap, Map<String, Object> model);
}
public interface MyHandlerAdapter {
 ModelView handle(HttpServletRequest request, HttpServletResponse response,
Object handler) throws ServletException, IOException;
}
```

μ΅μ’ FrontControllerV5

```java
@WebServlet(name = "frontControllerServletV5", urlPatterns = "/front-controller/v5/*")
public class FrontControllerServletV5 extends HttpServlet {
    // λͺ¨λ  μ»¨νΈλ‘€λ¬ μ§μ μν΄ Object μ¬μ©
    private final Map<String, Object> handlerMappingMap = new HashMap<>();
    private final List<MyHandlerAdapter> handlerAdapters = new ArrayList<>();

    public FrontControllerServletV5() {
        initHandlerMappingMap(); // νΈλ€λ¬ λ§€ν μ΄κΈ°ν
        initHandlerAdapters(); // μ΄λν° μ΄κΈ°ν
    }

    private void initHandlerAdapters() {

        handlerAdapters.add(new ControllerV3HandlerAdapter());
        handlerAdapters.add(new ControllerV4HandlerAdapter()); // V4 μΆκ°
    }

    private void initHandlerMappingMap() {
        handlerMappingMap.put("/front-controller/v5/v3/members/new-form", new MemberFormControllerV3());
        handlerMappingMap.put("/front-controller/v5/v3/members/save", new MemberSaveControllerV3());
        handlerMappingMap.put("/front-controller/v5/v3/members/members", new MemberListControllerV3());

        // V4 μΆκ°
        handlerMappingMap.put("/front-controller/v5/v4/members/new-form", new MemberFormControllerV4());
        handlerMappingMap.put("/front-controller/v5/v4/members/save", new MemberSaveControllerV4());
        handlerMappingMap.put("/front-controller/v5/v4/members/members", new MemberListControllerV4());
    }

    @Override
    protected void service(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        Object handler = getHandler(request);
        if (handler == null){
            response.setStatus(HttpServletResponse.SC_NOT_FOUND);
            return;
        }

        MyHandlerAdapter adapter = getHandlerAdapter(handler);
        ModelView mv = adapter.handle(request, response, handler);

        MyView view = viewResolver(mv.getViewName());
        view.render(mv.getModel(), request, response);
    }

    private Object getHandler(HttpServletRequest request) {
        String requestURI = request.getRequestURI();
        return handlerMappingMap.get(requestURI);
    }

    private MyHandlerAdapter getHandlerAdapter(Object handler) {
        for (MyHandlerAdapter adapter : handlerAdapters) {
            if (adapter.supports(handler)) {
                return adapter;
            }
        }
        throw new IllegalArgumentException("handler adapterλ₯Ό μ°Ύμ μ μμ΅λλ€. handler= " + handler);
    }

    private MyView viewResolver(String viewName){
        return new MyView("/WEB-INF/views/" + viewName + ".jsp");
    }
}
```

μ§κΈκΉμ§ v1 ~ v5λ‘ μ μ§μ μΌλ‘ νλ μμν¬λ₯Ό λ°μ μμΌμμ΅λλ€.

1. v1 : νλ‘ νΈ μ»¨νΈλ‘€λ¬λ₯Ό λμ
  - κΈ°μ‘΄ κ΅¬μ‘°λ₯Ό μ΅λν μ μ§νλ©΄μ νλ‘ νΈ μ»¨νΈλ‘€λ¬λ₯Ό λμνμ΅λλ€.
2. v2 : View λΆλ₯
  - λ¨μ λ°λ³΅λλ λ·° λ‘μ§μ λΆλ¦¬νμ΅λλ€.
3. v3 : Model μΆκ°
  - μλΈλ¦Ώ μ’μμ±μ μ κ±°νμ΅λλ€.
  - λ·° μ΄λ¦μ μ€λ³΅μ μ κ±°νμ΅λλ€.
4. v4: λ¨μνκ³  μ€μ©μ μΈ μ»¨νΈλ‘€λ¬
  - v3μ κ±°μ λΉμ·νμ§λ§
  κ΅¬ν μμ₯μμ ModelViewλ₯Ό μ§μ  μμ±ν΄μ λ°ννμ§ μλλ‘ νΈλ¦¬ν μΈν°νμ΄μ€λ₯Ό μ κ³΅ν  μ μμ΅λλ€.
5. v5: μ μ°ν μ»¨νΈλ‘€λ¬
  - μ΄λν° λμ
  - μ΄λν°λ₯Ό μΆκ°ν΄μ νλ μμν¬λ₯Ό μ μ°νκ³  νμ₯μ± μκ² μ€κ³νμ΅λλ€.
  
μ¬κΈ°μ μ΄λΈνμ΄μμ μ¬μ©ν΄μ μ»¨νΈλ‘€λ¬λ₯Ό λ νΈλ¦¬νκ² λ°μ μν¬ μλ μμ΅λλ€. λ§μ½ μ΄λΈνμ΄μμ μ¬μ©ν΄μ μ»¨νΈλ‘€λ¬λ₯Ό νΈλ¦¬νκ² μ¬μ©ν  μ μκ² νλ €λ©΄ μ΄λΈνμ΄μμ μ§μνλ μ΄λν°λ₯Ό μΆκ°νλ©΄ λ©λλ€.

λ€νμ±κ³Ό μ΄λν° λλΆμ κΈ°μ‘΄ κ΅¬μ‘°λ₯Ό μ μ§νλ©΄μ, νλ μμν¬μ κΈ°λ₯μ νμ₯ν  μ μμ΅λλ€.

μ€νλ§ MVC
μ§κΈκΉμ§ μμ±ν μ½λλ μ€νλ§ MVC νλ μμν¬μ ν΅μ¬ μ½λμ μΆμ½ λ²μ μ΄κ³ , κ΅¬μ‘°λ
κ±°μ κ°λ€κ³  ν©λλ€.
μ€νλ§ MVCμλ μ§κΈκΉμ§μ λ΄μ©κ³Ό κ±°μ κ°μ κ΅¬μ‘°λ₯Ό κ°μ§κ³  μμ΅λλ€.
***

### μ€νλ§ MVC - κ΅¬μ‘° μ΄ν΄

#### μ€νλ§ MVC μ μ²΄ κ΅¬μ‘°
μ§μ  λ§λ  MVC νλ μμν¬μ μ€νλ§ MVCλ₯Ό λΉκ΅ν΄λ³΄κ² μ΅λλ€. 

μ§μ  λ§λ  νλ μμν¬μ μ€νλ§ MVCλ₯Ό λΉκ΅ν μ°¨μ΄λ λ€μκ³Ό κ°μ΅λλ€.

- FrontController -> DispatcherServlet
- handlerMappingMap -> HandlerMapping
- MyHandlerAdapter -> HandlerAdapter
- ModelView -> ModelAndView
- viewResolver -> ViewResolver
- MyView -> View 

![mvc](https://images.velog.io/images/urtimeislimited/post/db098793-d37a-44c0-bfb1-eafcdf343593/image.png)
	
![mvc](https://images.velog.io/images/urtimeislimited/post/db098793-d37a-44c0-bfb1-eafcdf343593/image.png)

#### DispatcherServlet κ΅¬μ‘° μ΄ν΄λ³΄κΈ°

```org.springframework.web.servlet.DispatcherServlet```
μ€νλ§ MVCλ νλ‘ νΈ μ»¨νΈλ‘€λ¬ ν¨ν΄μΌλ‘ κ΅¬νλμ΄ μμ΅λλ€.
μ€νλ§ MVCμ νλ‘ νΈ μ»¨νΈλ‘€λ¬κ° λ°λ‘ λμ€ν¨μ² μλΈλ¦Ώ(DispatcherServlet)μλλ€.
κ·Έλ¦¬κ³  μ΄ λμ€ν¨μ² μλΈλ¦Ώμ΄ λ°λ‘ μ€νλ§ MVCμ ν΅μ¬μλλ€.

#### DispacherServlet μλΈλ¦Ώ λ±λ‘
DispacherServlet λ λΆλͺ¨ ν΄λμ€μμ HttpServlet μ μμ λ°μμ μ¬μ©νκ³ , 
μλΈλ¦ΏμΌλ‘ λμν©λλ€.
- DispatcherServlet -> FrameworkServlet -> HttpServletBean -> HttpServlet
- μ€νλ§ λΆνΈλ DispacherServlet μ μλΈλ¦ΏμΌλ‘ μλμΌλ‘ λ±λ‘νλ©΄μ λͺ¨λ  κ²½λ‘(urlPatterns="/" )μ λν΄μ λ§€νν©λλ€.
- μ°Έκ³ : λ μμΈν κ²½λ‘κ° μ°μ μμκ° λκΈ° λλ¬Έμ κΈ°μ‘΄μ λ±λ‘ν μλΈλ¦Ώλ ν¨κ» λμν©λλ€.

#### μμ²­ νλ¦

