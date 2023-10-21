---

title: Leverage Security Frameworks and Libraries Checklist
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 2003

---

{% include breadcrumb.html %}

### 20.3 Checklist: Leverage Security Frameworks and Libraries

Secure coding libraries and software frameworks with embedded security help software developers guard against
security-related design and implementation flaws.

Refer to proactive control '[C2: Leverage Security Frameworks and Libraries][control2]'
for more context from the 'OWASP Top 10 Proactive Controls' project.

#### Best practices

* Use libraries and frameworks from trusted sources that are actively maintained and widely used
* Review all secondary applications and third party libraries to determine business necessity
* Validate safe functionality for all secondary applications and third party libraries
* Create and maintain an inventory catalog of all third party libraries using Software Composition Analysis (SCA)
* Proactively keep all third party libraries and components up to date
* Reduce the attack surface by encapsulating the library and expose only the required behaviour into your software
* Use tested and approved managed code rather than creating new unmanaged code for common tasks
* Utilize task specific built-in APIs to conduct operating system tasks
* Do not allow the application to issue commands directly to the Operating System
* Use checksums or hashes to verify the integrity of interpreted code, libraries, executables, and configuration files
* Restrict users from generating new code or altering existing code
* Implement safe updates using encrypted channels

#### References

* OWASP [Dependency Check][dependency]
* OWASP [Top 10 Proactive Controls][proactive10]

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue2002] or a [pull request][pr].

[control2]: https://owasp.org/www-project-proactive-controls/v3/en/c2-leverage-security-frameworks-libraries.html
[dependency]: https://owasp.org/www-project-dependency-check/
[issue2002]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2011-checklist/02-frameworks-libraries
[pr]: https://github.com/OWASP/www-project-developer-guide/pulls
[proactive10]: https://owasp.org/www-project-proactive-controls/

\newpage