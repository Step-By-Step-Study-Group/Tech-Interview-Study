# π¬ λͺ©μ°¨

[REST APIλ λ¬΄μμΈκ°μ?](#rest-apiλ-λ¬΄μμΈκ°μ)
<br/>
[SSRκ³Ό CSRμ μ°¨μ΄μ μ₯λ¨μ ](#ssrκ³Ό-csrμ-μ°¨μ΄μ-μ₯λ¨μ )  
[Network OSI 7κ³μΈ΅μ λν΄μ μ€λͺν΄μ£ΌμΈμ.](#network-osi-7κ³μΈ΅μ-λν΄μ-μ€λͺν΄μ£ΌμΈμ)  
[Network TCP/IP 4κ³μΈ΅μ λν΄μ μ€λͺν΄μ£ΌμΈμ.](#network-tcpip-4κ³μΈ΅μ-λν΄μ-μ€λͺν΄μ£ΌμΈμ)  
[ν¬μλ νλ‘μμ λ¦¬λ²μ€ νλ‘μλ λ¬΄μμ΄κ³ , μ΄λ€ μ°¨μ΄κ° μλμ?](#ν¬μλ-νλ‘μμ-λ¦¬λ²μ€-νλ‘μλ-λ¬΄μμ΄κ³ -μ΄λ€-μ°¨μ΄κ°-μλμ)

# REST APIλ λ¬΄μμΈκ°μ?

- RESTλ HTTP URIλ‘ μ ννλ μμμ λν νμλ₯Ό λ»ν©λλ€.
- μ€κ³κ·μΉμΌλ‘λ βURIλ μ λ³΄μ μμλ§ ννν΄μΌνλ©°, μμμ μνμ νμλ HTTP Methodμ λͺμ νλκ²βμ λ»ν©λλ€.
- μμ κ°μ REST κΈ°λ°μΌλ‘ APIλ₯Ό κ΅¬ν κ²μ REST APIλΌκ³  ν©λλ€.
- RESTful APIλ HTTP ν΅μ μ REST μ€κ³κ·μΉμ μ μ§μΌμ κ°λ°ν APIλ₯Ό λ»ν©λλ€.

-----

# SSRκ³Ό CSRμ μ°¨μ΄μ μ₯λ¨μ 

λͺ¨λ νμ΄μ§λ₯Ό λ λλ§νλ λ°©μ

### SSR( Server-Side Rendering )

- μλ²μμ HTML νμ΄μ§λ₯Ό μ€λΉνμ¬ ν΄λΌμ΄μΈνΈ λΈλΌμ°μ μκ² λ³΄λ
- λΈλΌμ°μ λ μ΄λ₯Ό λ λλ§νμ¬ νμ΄μ§λ₯Ό μμ±

### μ₯μ 

- μλ²μμ HTML νμ΄μ§λ₯Ό μ€λΉνκΈ° λλ¬Έμ μ΄κΈ° λ‘λ© μκ°μ΄ λ¨μΆ

### λ¨μ 

- λͺ¨λ  μμ²­μ λν΄ μλ²μμ HTML νμ΄μ§λ₯Ό μ€λΉν΄μΌ νλ―λ‘ μλ² μμμ΄ λ§μ΄ μ¬μ©
- μ¬μ©μ μνΈμμ©μ λν λκΈ° μκ°μ΄ μμ
    
    μ΄κΈ° λ‘λ© μλκ° λΉ λ₯΄μ§λ§, νμ΄μ§μ μλ°μ€ν¬λ¦½νΈ νμΌμ λ€μ΄λ‘λνκ³  μ€νν΄μΌ μ¬μ©μ μνΈμμ©μ΄ κ°λ₯ν©λλ€.
    

### CSR( Client-Side Rendering )

- νμ΄μ§μ μ΄κΈ° λ‘λ μμλ μλ²μμ λ°μ HTML νμΌμ΄ λΉμ΄μλ μνμ΄λ©°, λΈλΌμ°μ μμ μλ°μ€ν¬λ¦½νΈ νμΌμ λ‘λνκ³  μ€ννμ¬ νμ΄μ§λ₯Ό μμ±

### μ₯μ 

- λΉ λ₯Έ μ¬μ©μ μνΈμμ©μ΄ κ°λ₯
    
    νμ΄μ§λ₯Ό μ²μ λ‘λν  λλ HTML νμΌμ΄ λΉμ΄μμ§λ§, μλ°μ€ν¬λ¦½νΈ νμΌμ λ€μ΄λ‘λνκ³  μ€ννμ¬ νμ΄μ§λ₯Ό μμ±νκΈ° λλ¬Έμ μ¬μ©μ μνΈμμ©μ΄ λΉ λ¦λλ€.
    
- μλ² μμμ΄ μ κ² νμ
    
     μλ²μμλ λ¨μν μλ°μ€ν¬λ¦½νΈ νμΌλ§ λ³΄λ΄μ£Όλ©΄ λλ―λ‘ μλ² μμμ μ κ² μ¬μ©
    

### λ¨μ 

- μ΄κΈ° λ‘λ© μλκ° λλ¦Ό
    
    μ΄κΈ° λ‘λ© μμλ μλ²μμ λ°μ HTML νμΌμ΄ λΉμ΄μκΈ° λλ¬Έμ, μλ°μ€ν¬λ¦½νΈ νμΌμ λ€μ΄λ‘λνκ³  μ€νν΄μΌ νμ΄μ§λ₯Ό μμ±ν  μ μμ
    
# [network]OSI 7κ³μΈ΅μ λν΄μ μ€λͺν΄μ£ΌμΈμ.

**osi 7κ³μΈ΅μ΄λ?**

κ΅­μ νμ€νκΈ°κ΅¬(International Organization for Standardization)μμ λ€νΈμν¬ ν΅μ  κ³Όμ μ 7λ¨κ³λ‘ λλ κ²μ λ§ν©λλ€.

**Physical Layer 1κ³μΈ΅**

λ°μ΄ν°λ₯Ό **μΈν°λ· μΌμ΄λΈμ΄λ λΌμ°ν°** λ±μΌλ‘ μ κΈ°μ  μ νΈλ₯Ό μλ λ‘κ·Έ μ νΈμΈ 0κ³Ό 1λ‘ λ°κΏ λ΄λ³΄λ΄κ³  λ€μ΄μ€κ² νλ μ μΌ μ²«λ²μ§Έ κ³μΈ΅μ΄μ λͺ¨λ / **PHYμΉ©**μ΄λΌλ νλμ¨μ΄ λΆνμ κ΅¬νλμ΄μμ.

**Data Link Layer 2κ³μΈ΅**

κ°μ λ€νΈμν¬μ μλ **μ¬λ¬ λμ μ»΄ν¨ν°λ€μ΄ λ°μ΄ν°λ₯Ό μ£Όκ³  λ°κΈ° μν΄** νμν κ³μΈ΅μ΄μ λͺ¨λμΈλ°, **framing**μ΄λΌλ μμμ΄ μ΄λ£¨μ΄μ§λ©° μ΄κ²μ λ°μ΄ν°λ₯Ό encodingν΄μ£Όλ μ­ν μ νκ³  μ΄λ μ¬λ¬λμ μ»΄ν¨ν°κ° ν΅μ νλ μν©μλ λ°μ΄ν°λ₯Ό κ΅¬λΆν΄μ£Όλ μ­ν μ μν΄ λ§λ  κ² / **λμΉ΄λ**λΌλ νλμ¨μ΄ λΆνμ κ΅¬νλμ΄μμ

**Network Layer 3κ³μΈ΅ β framingν λ°μ΄ν°λ₯Ό λ°κΈ° μν΄ λ§λ€μ΄μ§ κ³μΈ΅**

λ€νΈμν¬ κ° λ°μ΄ν° μ μ‘μ μν΄ **ν¨ν·**νμ¬ λͺ©μ μ§λ₯Ό μ°Ύμλ΄κ³  μμ  λ€μμ **λΌμ°ν°**μ λ°μ΄ν°λ₯Ό λκ²¨μ£Όλ κ³μΈ΅μ΄μ λͺ¨λ / μ΄μμ²΄μ  μ»€λμ μννΈμ¨μ΄μ μΌλ‘ κ΅¬νλμ΄μμ

**ν¨ν·** β dataμ ip μ£Όμλ₯Ό λΆμΈ κ²

**λΌμ°ν°** β μ»΄ν¨ν° λ€νΈμν¬ κ°μ λ°μ΄ν° ν¨ν·μ μ μ‘νλ λ€νΈμν¬ μ₯μΉ

**Transport Layer 4κ³μΈ΅ β μ΄λ€ λ°μ΄ν°λ₯Ό λ¬΄μ¨ νλ‘μΈμ€μκ² μ€μΌν μ§ μ»΄ν¨ν°λ μ΄λ»κ² μκΉ? ν¬νΈλ²νΈ**

**Port** λ²νΈλ₯Ό μ¬μ©νμ¬ λμ°©μ§ μ»΄ν¨ν°μ μ΅μ’ λμ°©μ§μΈ νλ‘μΈμ€ μ¦, **μΌκ³  μλ μΈν°λ· μ°½κΉμ§ λ°μ΄ν°κ° λλ¬νκ² λ§λλ** κ³μΈ΅μ΄μ λͺ¨λ / μ΄μμ²΄μ  μ»€λμ μννΈμ¨μ΄μ μΌλ‘ κ΅¬νλμ΄μμ

**port** β μ΄μ μ²΄μ  ν΅μ μ μ’λ¨μ μΌλ‘ λ€νΈμν¬ μλΉμ€λ νΉμ  νλ‘μΈμ€λ₯Ό μλ³νλ λΌλ¦¬ λ¨μ / ν¬νΈλ₯Ό μ£Όλ‘ μ¬μ©νλ νλ‘ν μ½μ μ μ‘ κ³μΈ΅ νλ‘ν μ½μ΄λΌ νλ©° TCPμ UDPκ° μκ³  ν¬νΈ λ²νΈλ IP μ£Όμμ ν¨κ» μ°μλλ€.

**Session Layer 5κ³μΈ΅**

TCP/IP μΈμμ λ§λ€κ³  μμ λ μ±μμ μ§κ³  μμ΄ **ν΅μ μ κ΄λ¦¬**νλ μ­ν μ κ³μΈ΅μ΄μ λͺ¨λλ‘ ν΅μ  λ°©μμΈ μ μ΄μ€(μ β μ ν), λ°μ΄μ€(μ β λ¬΄μ κΈ°), λ¨μ(μ β TV) λ±μ κ²°μ ν©λλ€. ν¬ν  μ°κ²°μ΄λΌκ³ λ νλ©°, SSH, TLS λ±μ΄ λνμ μΈ νλ‘ν μ½μλλ€.

**Presentation Layer 6κ³μΈ΅**

**λ°μ΄ν°λ₯Ό μ΄λ€ ννλ‘ κ°μ§ κ²μΈμ§ μ νλ μ­ν **μ νλ κ³μΈ΅μ΄μ λͺ¨λλ‘ λ°μ΄ν°μ μΈμ½λ©, λμ½λ©, μνΈν, λ³΅νΈν λ±μ μννκ³  GIFλ JPGκ°μ νμμ κ΅¬λΆνκΈ°λ ν©λλ€.

**Application Layer 7κ³μΈ΅ β dataλ₯Ό status codeλ‘ κ°μΈλ μμ­**

HTTP λ±μ νλ‘ν μ½μ΄ ν¬ν¨λ κ³μΈ΅μ΄μ λͺ¨λλ‘ μ΄κΈ°μλ WWW μμ νμ΄νΌνμ€νΈ ννμ λ¬Έμλ₯Ό μ λ¬νλλ° μ£Όλ‘ μ΄μ©νμκ³  νμ¬λ μ΄λ―Έμ§, λΉλμ€, μμ± λ± κ±°μ λͺ¨λ  νμμ λ°μ΄ν°λ₯Ό μ μ‘ν  μ μλ€.

# [Network]TCP/IP 4κ³μΈ΅μ λν΄μ μ€λͺν΄μ£ΌμΈμ.

**ν¨ν· ν΅μ μ΄λ?**

λ°μ΄ν°λ₯Ό ν¨ν·μ΄λΌλ μμ λ¨μλ‘ λλ  μ μ‘νλ λ°©μ

**IPλ?**

ν¨ν· λ°μ΄ν°λ₯Ό μ΅λν λΉ λ₯΄κ² λͺ©μ  μ£Όμλ‘ λ³΄λ΄λ νλ‘ν μ½

ν¨ν· μ λ¬ μ¬λΆ λ³΄μ¦ x / ν¨ν· λ³΄λΈ μμμ λ°λ μμ λ€λ₯Ό μ μμ

**TCPλ?**

ν¨ν· ν΅μ  μ€ μμκ° λ€μμ΄κ±°λ λ΄μ©μ΄ μ μ€λλ λ¨μ μ λ³΄μν κ²μ΄ TCP, ν¨ν·μ μ μμ μΌλ‘ λ°μ μ μλλ‘ νλ νλ‘ν μ½

**TCP νΉμ§**

**μ₯μ **

- ν¨ν· μ λ¬ μ¬λΆ λ³΄μ¦
- μ‘μ  μμλλ‘ ν¨ν·μ λ°κ² ν΄μ€
- λ§μ½ ν¨ν·μ΄ μμλκ±°λ μμ€λμλ€λ©΄ μΆλ°μ§μμ μ¬μμ²­νλ λ°©μμΌλ‘ μ§ν

**λ¨μ **

- IPλ³΄λ€ ν¨ν· μ μ‘ μλ λλ¦Ό

**TCP/IPλ?**

IPμ TCPμ λ¬ΆμμΌλ‘ λκ°μ§ νλ‘ν μ½ λ°©μμ μ‘°ν©ν μΈν°λ· ν΅μ μ λ§νκ³  TCP/IP λ°©μμ λ€νΈμν¬μμ ν΅μ μ΄ μΌμ΄λλ κ³Όμ μ 4λ¨κ³λ‘ λλ κ²μ΄ TCP/IP 4κ³μΈ΅μλλ€.

λ³΄μμ  β TCPμ λλ¦°μ , IPμ λ΄μ© μμ€ νΉμ μμ λ°λ β μλ ν₯μ, ν¨ν· μ μ λμ°©

- νλ‘ν μ½ μ€ν(;νλ‘ν μ½ μ€μνΈ) β λ³΅μμ νλ‘ν μ½ μ§ν© / νλ‘ν μ½ μ€νλΌλ¦¬λ ν΅μ€ λΆκ°

**TCP/IP 4κ³μΈ΅μ μΊ‘μν, μ­μΊ‘μν**

μΊ‘μν β λ°μ΄ν°κ° Application Layerμμ Network Access Layer νΉμ PhysicalΒ Layerλ‘ μ΄λνλ©΄μ ν΄λΉ κ³μΈ΅μμ μΈμ½λ©μ νλλ°, μ΄κ²μ μΊ‘μνλΌκ³  νλ€.

μ­μΊ‘μν β μΊ‘μνμ λ°λ νμμ΄λ€.

**Application Layer**

μμ© νλ‘κ·Έλ¨μμ λ°μ΄ν°λ₯Ό μ²λ¦¬νλ κ³μΈ΅ / HTTP, HTTPS, POP3, SMTP, FTP λ±

**Transport Layer**

μ΄νλ¦¬μΌμ΄μμμ λμ΄μ¨ λ°μ΄ν°μ λν κ²μ¦, μ¬μ μ‘ λ± κ°μ’ μ μ΄λ₯Ό λ΄λΉνλ κ³μΈ΅ / TCP, UDP λ±

**Internet Layer**

λ°μ΄ν°λ₯Ό λͺ©μ μ§κΉμ§ ν¨μ¨μ μΌλ‘ μ λ¬μ λ΄λΉνλ κ³μΈ΅ / IP, ICMP λ±

**Network Access Layer**

μ€μ§μ μΌλ‘ λ°μ΄ν°λ₯Ό μ μ‘νλ κ³μΈ΅ / Ethernet, Wi-Fi λ±

**νλ¦ μμ½**

- [www.google.com](http://www.google.xn--com-of0o/)Β λΈλΌμ°μ  μ£Όμμ°½μ μλ ₯
- λ³΄λΌ ν¨ν·μ HTTP ν€λ β HTTP Requestλ₯Ό ν΅ν΄ μ±μμ§ μν
- λ³΄λΌ ν¨ν·μ IP ν€λλ₯Ό μ±μ°κΈ° μν΄, DNS μλ²λ₯Ό ν΅ν΄Β [www.google.com](http://www.google.xn--com-of0o/)Β λλ©μΈμ IP μ£Όμλ₯Ό μλ΅ λ°μ΅λλ€.
- λ³΄λΌ ν¨ν·μ TCP ν€λλ₯Ό μ±μ°κΈ° μν΄, ν΄λΌμ΄μΈνΈμ κ΅¬κΈ μΉμλ² κ° TCP μ°κ²°μ ν©λλ€.
    - 3-Way Handshaking
- λ³΄λΌ ν¨ν·μ΄ μμ±λμμΌλ―λ‘,Β [www.google.com](http://www.google.com/)Β μ ν¨ν·μ μ μ‘νκ³ , HTML μ μλ΅λ°μ΅λλ€.
- ν΄λΌμ΄μΈνΈλ μλ΅ λ°μ HTML μ λΈλΌμ°μ μ λμλλ€.
- ν΄λΌμ΄μΈνΈμ κ΅¬κΈ μΉμλ²κ° TCP μ°κ²°μ μ’λ£ν©λλ€.
    - 4-Way Handshaking

# ν¬μλ νλ‘μμ λ¦¬λ²μ€ νλ‘μλ λ¬΄μμ΄κ³ , μ΄λ€ μ°¨μ΄κ° μλμ?

### νλ‘μ(Proxy)λ?
νλ‘μ μλ²λ ν΄λΌμ΄μΈνΈκ° μμ μ ν΅ν΄μ λ€λ₯Έ λ€νΈμν¬ μλΉμ€μ κ°μ μ μΌλ‘ μ κ·Όν  μ μκ² ν΄ μ£Όλ μ»΄ν¨ν° μμ€νμ΄λ μμ© νλ‘κ·Έλ¨μ κ°λ¦¬ν΅λλ€.

νλ§λλ‘, μλ²μ μλ² μ¬μ΄μ μ€κ³μ μ­ν μ νλ€κ³  λ³Ό μ μμ΅λλ€.

νλ‘μλ₯Ό μ°λ μ΄μ λ λ³΄μμμ μ΄μ λ‘ μ§μ  ν΅μ ν  μ μλ λ μ μ¬μ΄μμ λλ¦¬λ‘ ν΅μ μ μννμ¬ λ³΄μμ±, μ±λ₯, μμ μ±μ ν₯μμν€κΈ° μν¨μλλ€.

![img.png](img.png)

> νλ‘μ μλ²λ λ€νΈμν¬ μ μ΄λμ μμΉνλλ, νΉμ μ΄λ λ°©ν₯μΌλ‘ λ°μ΄ν°λ₯Ό μ κ³΅νλλμ λ°λΌ
> Forward Proxy κ·Έλ¦¬κ³  Reverse Proxyλ‘ λλ©λλ€.

### ν¬μλ νλ‘μ(Forward Proxy)
ν¬μλ νλ‘μλ, νλ‘μ μλ²κ° ν΄λΌμ΄μΈνΈ λ°λ‘ λ€μ μλ λ€νΈμν¬ κ΅¬μ‘°λ₯Ό μλ―Έν©λλ€.

κ°μ λ΄λΆλ§μ μ‘΄μ¬νλ ν΄λΌμ΄μΈνΈμ μμ²­μ λ°μ μΈν°λ·μ ν΅ν΄ μΈλΆ μλ²μμ λ°μ΄ν°λ₯Ό κ°μ Έμ ν΄λΌμ΄μΈνΈμκ² μλ΅ν΄μ€λλ€.  
μ¦, ν΄λΌμ΄μΈνΈκ° μλ²μ μ κ·Όνκ³ μ ν  λ, ν΄λΌμ΄μΈνΈλ νκ² μλ²μ μ£Όμλ₯Ό ν¬μλ νλ‘μμ μ λ¬νμ¬, ν¬μλ νλ‘μκ° μΈν°λ·μΌλ‘ μμ²­λ λ΄μ©μ κ°μ Έμ€λ λ°©μμλλ€.
![img_1.png](img_1.png)

#### μ₯μ 
- **ν΄λΌμ΄μΈνΈ λ³΄μ** : ν¬μλ νλ‘μ μλ²λ λ°©νλ²½κ³Ό λΉμ·ν κ°λμΌλ‘ λ³Ό μ μλ€. μλ₯Ό λ€μ΄ ν¬μλ νλ‘μ μλ²μ λ£°μ μΆκ°ν΄ νΉμ  μ¬μ΄νΈμ μ μνλ κ²μ λ§μ μ μλ€.
- **μΊμ±** : ν¬μλ νλ‘μμ μΊμ±λμ΄ μλ λ°μ΄ν°λ₯Ό μ¬μ©νκΈ° λλ¬Έμ λ λΉ λ₯Έ μ±λ₯μ κ²½νν  μ μλ€.
- **μνΈν** : ν΄λΌμ΄μΈνΈμ μμ²­μ ν¬μλ νλ‘μ μλ²λ₯Ό ν΅κ³Όν  λ μνΈνλλ€. μνΈνλ μμ²­μ λ€λ₯Έ μλ²λ₯Ό ν΅κ³Όν  λ νμν μ΅μνμ μ λ³΄λ§ κ°κ² λκ³ , μ΄λ ν΄λΌμ΄μΈνΈ IPλ₯Ό κ°μΆ°μ£Όλ λ³΄μ ν¨κ³Όλ₯Ό κ°μ§λ€.

### λ¦¬λ²μ€ νλ‘μ€(Reverse Proxy)
λ¦¬λ²μ€ νλ‘μλ, νλ‘μ μλ²κ° μλ² λ°λ‘ μμ μλ λ€νΈμν¬ κ΅¬μ‘°λ₯Ό μλ―Έν©λλ€.

ν΄λΌμ΄μΈνΈλ μΉμλΉμ€μ μ κ·Όν  λ, μΉμλ²μ μμ²­νλ κ²μ΄ μλ νλ‘μλ‘ μμ²­νκ² λκ³  νλ‘μκ° λ°°νμ μλ²λ‘λΆν° λ°μ΄ν°λ₯Ό κ°μ Έμ€λ λ°©μμλλ€.

- μ°λ¦¬κ° κ΅¬μ±νλ μΌλ°μ μ WEB - WAS λΆλ¦¬ ννλ₯Ό λ¦¬λ²μ€ νλ‘μλΌκ³  λ³Ό μ μμ΅λλ€.
- μ¬κΈ°μ WEBμ΄ λ¦¬λ²μ€ νλ‘μκ° λλ€.
- λ¬Όλ‘  μνμΉ ν°μΊ£κ³Ό κ°μ΄ λ¬Όλ¦¬μ μΈ νμλ²μ WEB, WASκ° μ‘΄μ¬νλ€λ©΄ λ¦¬λ²μ€ νλ‘μλΌκ³  λ³Ό μ μμ΅λλ€.

#### μ₯μ 
- **λ‘λ λ°Έλ°μ±** : μλ² κ³ΌλΆνλ₯Ό λ§κΈ° μν μμ
- **μλ² λ³΄μ** : λ³Έλ μλ²κ° μλ λ¦¬λ²μ€ νλ‘μλ‘ μμ²­μ νκΈ° λλ¬Έμ, λ³Έλ μλ²μ IP μ£Όμλ₯Ό λΈμΆμν€μ§ μμ μ μλ€.
- **μΊμ±** :  νκ΅­μμ νκ΅­μ μλ μΉμλ²λ₯Ό μ¬μ©ν  λ, λ¦¬λ²μ€ νλ‘μ μλ²κ° νκ΅­μ μλ€κ³  κ°μ ν΄λ³΄μ. νκ΅­μ μλ μ μ λ νκ΅­μ μλ λ¦¬λ²μ€ νλ‘μ μλ²μ ν΅μ ν΄ λ¦¬λ²μ€ νλ‘μ μλ²μ μΊμ±λμ΄ μλ λ°μ΄ν°λ₯Ό μ¬μ©ν  κ²½μ°μ λ λΉ λ₯Έ μ±λ₯μ κ²½νν  μ μλ€.
- **μνΈν** : SSL μνΈνμ μ’λ€.

> ν΄λΌμ΄μΈνΈμͺ½μΌλ‘ λ°μ΄ν°(Response)λ₯Ό λ°μ΄μ£Όλκ² ν¬μλλΌλ©΄, 
> κ·Έ λ°λνΈμΈ μλ² μͺ½μΌλ‘ λ°μ΄ν°(Request)λ₯Ό λ°μ΄μ£Όλ κ²μ΄ λ¦¬λ²μ€λΌκ³  λ³Ό μ μμ΅λλ€.

![img_3.png](img_3.png)

### ν¬μλ νλ‘μμ λ¦¬λ²μ€ νλ‘μμ μ°¨μ΄μ 
- νλ‘μ μλ²μ μμΉμ μ°¨μ΄κ° μλ€.  
ν¬μλ νλ‘μ μλ²λ ν΄λΌμ΄μΈνΈ μμ λμ¬μ Έ μκ³ , λ¦¬λ²μ€ νλ‘μ μλ²λ μλ² μμ λμ¬μ Έ μλ€.
- νλ‘μ μλ²μ ν΅μ  λμμ΄ λ€λ₯΄λ€.  
ν¬μλ νλ‘μλ λ΄λΆλ§μμ ν΄λΌμ΄μΈνΈμ νλ‘μ μλ²κ° ν΅μ νλ©°, λ¦¬λ²μ€ νλ‘μλ νλ‘μ μλ²μ λ΄λΆλ§μλ²κ° ν΅μ μ νλ€.
- κ°μΆ°μ§λ λμ  
ν¬μλ νλ‘μλ μ§μ  μλ² URLλ‘ μμ²­νμ§λ§, λ¦¬λ²μ€ νλ‘μλ νλ‘μ μλ² URLλ‘ μμ²­μ νλ€. λλ¬Έμ λ¦¬λ²μ€ νλ‘μλ λ³Έμλ²μ IP μ λ³΄λ₯Ό μ¨κΈΈ μ μλ€.  
ν¬μλ νλ‘μλ λ΄λΆλ§μ μμ²­μ νλ‘μ μλ²κ° μλ²λ‘ μμ²­νκΈ° λλ¬Έμ μλ²μκ² ν΄λΌμ΄μΈνΈκ° λκ΅¬μΈμ§ κ°μΆ μ μμ΅λλ€.


[[WEB] π Reverse Proxy / Forward Proxy μ μ & μ°¨μ΄ μ λ¦¬](https://inpa.tistory.com/entry/NETWORK-%F0%9F%93%A1-Reverse-Proxy-Forward-Proxy-%EC%A0%95%EC%9D%98-%EC%B0%A8%EC%9D%B4-%EC%A0%95%EB%A6%AC#%EB%A6%AC%EB%B2%84%EC%8A%A4_%ED%94%84%EB%A1%9D%EC%8B%9C_reverse_proxy)


