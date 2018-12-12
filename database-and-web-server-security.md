# Database and Web Server Security

## SQL Injection
Achieved by inserting malicious statements into an SQL query.

Usually takes advantage of logical conditions adding a statement like ` ' OR 1 = 1; #` to the logic of a query.

You can insert whatever malicious commands you would like to at that point.

Example of query that has had SQL Injected.

```SQL
select userName from users where userName='john' and userPass='' or 1=1 #'
```

SQL Comment can be `#` or `--`. `#` is preferable for `MySql`.

## SQL Injection Mitigation
* Give appropriate roles to users.
  * IE Have a webuser account that only has query permissions.
* Filter out threats
  * If a single quote: `'` is filtered out it can't be used to terminate a string. Consider doubling up single quotes for SQL Queries.
  * Data Integrity needs to be accounted for.
* Limit Input Sizes.
  * With less room for input there is less room for malicious code.
  *  Will usernames and/or passwords be more than ten characters? (I should hope so...)
* Forms should post and not get
  * Does this even need to be said? Isn't that just super obvious?
  * Prevents malicious tampering with url.
* Ensure valid datatypes with filters.
* Database abstraction: IE PDO will use prepared statements that will handle injections.
* Add line breaks to your SQL statements. This prevents the amount of code that can be commented out and at the very least the likelihood that an exception will be thrown.

## Cross Site Scripting: XSS
Three main categories:
* Non-persistent or reflected vulnerability (most common)
* DOM-Based or Local XSS. Can have extra javascript vulnerabilities in old versions of IE
* Stored, persistent or second-order vulnerability. Vulnerability is stored and displayed back without validation.

## Non-persistent Vulnerability

Example given states URL crafted to use `Javascript` to pass sensitive session/cookie information.

## DOM Based

Maliciously constructed page that can run commands on the source computer.

## Stored or Persistent Vulnerability

Unfiltered input is displayed back allowing for scripts to embedded.

## Impact of XSS
* Session can be stolen and continued (fairly easy to mitigate)
* Manipulating victim's file system/network. This is bad.
* Keylogging.
* Probing intranet.
* Launching other attacks: botnet, DDOS.
* Bruteforce password cracking.

## XSS Mitigation
* Filter all input.
* Escape all Output in whatever format it is to be displayed. IE HTML safe for HTML.
* Only allow safe content if field is conducive for it. This can be difficult with names.