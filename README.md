# Knowledge Base
### Specifications

* Key words for use in RFCs to Indicate Requirement Levels [https://www.ietf.org/rfc/rfc2119.txt](https://www.ietf.org/rfc/rfc2119.txt)
* JSON [https://tools.ietf.org/html/rfc7159](https://tools.ietf.org/html/rfc7159)
* JSON Web Token (JWT) [https://tools.ietf.org/html/rfc7519](https://tools.ietf.org/html/rfc7519)
* JWT Best Practices (draft) [https://tools.ietf.org/html/draft-ietf-oauth-jwt-bcp-03](https://tools.ietf.org/html/draft-ietf-oauth-jwt-bcp-03)
* OAuth 2.0 [https://tools.ietf.org/html/rfc6749](https://tools.ietf.org/html/rfc6749)
* OpenId Connect (OIDC) [http://openid.net/developers/specs/](http://openid.net/developers/specs/)

### .NET

* Use [NodaTime](https://nodatime.org/) for date/time handling

### Miscellaneous
* When building API to filter by datetime, Start should be included, but End should not: `[Start, End)`. No need to do this when filtering by dates only (no time)
* Email validation regexp: `^[a-zA-Z0-9._%+-]+@(?:[a-zA-Z0-9-]+\.)+[a-zA-Z]{2,}$` explanation: [http://www.regular-expressions.info/email.html](http://www.regular-expressions.info/email.html)
* GMT, CET, CEST, WET, WEST etc are not time zones
* Microsoft REST API Guidelines [https://github.com/Microsoft/api-guidelines/blob/vNext/Guidelines.md](https://github.com/Microsoft/api-guidelines/blob/vNext/Guidelines.md)

### Usefulle terms

* Race Condition [https://en.wikipedia.org/wiki/Race_condition](https://en.wikipedia.org/wiki/Race_condition) (check-then-act)

### Next
 * .NET resilience and transient-fault-handling library [http://www.thepollyproject.org/](http://www.thepollyproject.org/)
 * Http Client librabries [https://github.com/reactiveui/refit](https://github.com/reactiveui/refit) and [https://flurl.io/](https://flurl.io/)
