# Security
This is a small list of vulnerabilities, links and books which help to junior developers with learning security.
The knowledge came to me bit by bit. Accidentally I knew about "OWASP" after seven months of my work. I knew about the "ranbow table" when I was reading the "Learning NodeJs". More programmes don't know about the "HttpOnly" flag although they have more than year of experience of development. Why is this happening?
This is not an article. I won't to explain your about "race condition" or other a specific vulnerability or something else... The goal of this list that you will see links and books which you can read. I want to save your time. Do you know what does "vulnerability scanner" mean? No? So you can read about it here. Now you hear about "vulnerability scanner", you read about "vulnerability scanner" and may be you will use it in the future. This is awesome! My goal was achieved!

## OWASP
> The Open Web Application Security Project (OWASP) is a 501(c)(3) worldwide not-for-profit charitable organization > focused on improving the security of software. Our mission is to make software security visible, so that 
> individuals and organizations worldwide can make informed decisions about true software security risks.

## Vulnerabilities
See [OWASP: TOP 10, 2013](https://www.owasp.org/index.php/Top_10_2013-Top_10) and list of all vulnerabilites on 
the [OWASP](https://www.owasp.org/index.php/Category:Vulnerability) web site.

## XSS
> Critical bug allowing execute code on the server occurs in one third of applications,
> but simple thing such as XSS are almost always.

-- [Egor Homakov](https://twitter.com/homakov)

Articles about XSS:

* [XssAttacks](http://htmlpurifier.org/live/smoketests/xssAttacks.php)
* [OWASP: XSS_(Cross_Site_Scripting)_Prevention_Cheat_Sheet](https://www.owasp.org/index.php/XSS_(Cross_Site_Scripting)_Prevention_Cheat_Sheet)
* [SecurityHeaders: X-XSS-Protection](https://securityheaders.com/x-xss-protection.php)

## CLIENT-SIDE VALIDATION
> Servers should not rely on client-side validation. Client-side validation can be intentionally 
> bypassed by hostile users, and  unintentionally bypassed by users of older user agents or 
> automated tools that do not implement these features. The constraint validation features 
> are only intended to improve the user experience, not to provide any kind of security mechanism.

-- [HTML Living Standard](https://html.spec.whatwg.org/multipage/forms.html#security-forms)

Because don't forget about backend validation!

## Clickjacking
> Clickjacking, also known as a "UI redress attack", is when an attacker uses multiple transparent or opaque layers to trick a user 
> into clicking on a button or link on another page when they were intending to click on the the top level page. Thus, the attacker 
> is "hijacking" clicks meant for their page and routing them to another page, most likely owned by another application, domain, or both.

-- [OWASP: Clickjacking](https://www.owasp.org/index.php/Clickjacking)

## COOKIE
> If the HttpOnly flag (optional) is included in the HTTP response header, the cookie cannot be 
> accessed through client side script (again if the browser supports this flag). As a result, even 
> if a cross-site scripting (XSS) flaw exists, and a user accidentally accesses a link that exploits 
> this flaw, the browser (primarily Internet Explorer) will not reveal the cookie to a third party.

-- [OWASP: HttpOnly](https://www.owasp.org/index.php/HttpOnly)

## Cross-Site Request Forgery (CSRF)
> Cross-Site Request Forgery (CSRF) is an attack that forces an end user to execute unwanted actions on a web application in which 
> they're currently authenticated. CSRF attacks specifically target state-changing requests, not theft of data, since the attacker has no way 
> to see the response to the forged request. With a little help of social engineering (such as sending a link via email or chat), an attacker 
> may trick the users of a web application into executing actions of the attacker's choosing. If the victim is a normal user, a successful CSRF attack 
> can force the user to perform state changing requests like transferring funds, changing their email address, and so forth. 
> If the victim is an administrative account, CSRF can compromise the entire web application.

-- [OWASP: CSRF](https://www.owasp.org/index.php/Cross-Site_Request_Forgery_(CSRF))


## SQL-injection
> A SQL injection attack consists of insertion or "injection" of a SQL query via the input data from the client to the application. 
> A successful SQL injection exploit can read sensitive data from the database, modify database data (Insert/Update/Delete), execute 
> administration operations on the database (such as shutdown the DBMS), recover the content of a given file present on the DBMS 
> file system and in some cases issue commands to the operating system. SQL injection attacks are a type of injection attack, in which SQL 
> commands are injected into data-plane input in order to effect the execution of predefined SQL commands.

-- [OWASP: SQL injection](https://www.owasp.org/index.php/SQL_Injection)

## Rainbow tables
* [Wiki](https://en.wikipedia.org/wiki/Rainbow_table)
* [Learning NodeJS](http://shop.oreilly.com/product/0636920024606.do)
(you can read in this book the chapter "Guards at the Gate"(subchapter "Safely Storing Passwords"))

## Languages and frameworks
* [OWASP: PHP_security_cheatsheet](https://www.owasp.org/index.php/PHP_Security_Cheat_Sheet)
* [OWASP: Ruby_on_Rails_cheatsheet](https://www.owasp.org/index.php/Ruby_on_Rails_Cheatsheet)
* [RailsGuides: Ruby_on_Rails_security_guide](http://guides.rubyonrails.org/security.html)

## Vulnerability scanners

## Links
* [HTML5 Security Cheatsheet](http://html5sec.org)
* [SecurityHeaders.com](https://securityheaders.com)
* [Sakurity.com blog](http://sakurity.com/blog)

## Books
* [The Tangled Web](http://www.amazon.com/The-Tangled-Web-Securing-Applications/dp/1593273886)
* [The web application Hacker's handbook](http://www.amazon.com/Web-Application-Hackers-Handbook-Exploiting/dp/1118026470/ref=sr_1_1?s=books&ie=UTF8&qid=1437737754&sr=1-1&keywords=The+web+application+Hacker%27s+handbook)
* [PHP and MySQL Web Development](http://www.amazon.com/PHP-MySQL-Web-Development-Edition/dp/0672329166)
(you can read in this book the chapter "E-commerce Security issue")
