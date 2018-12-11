#  Interface Design

## Single Login

*  Single login or single sign-on (SSO) authenticates many systems with one login.
*  Reduces password fatigue.
*  Implementations
    *  LDAP (lightweight directory access protocol)
    *  Kerberos (Not Kerebos like he says in notes/tests ffs.)
    *  Windows Live ID
    *  Google Sign-in

>  **Web Implementations**
>
>  Becomes difficult to implement.  
>  Sessions/cookies?
>  *  Sessions are easier to manage
>  *  Cookies are domain specific.
>
> Oath (app solution more than web)

###  When Security Fails

*  Users can select the security options.
*  Users determine encryption keys.
*  Poor configuration of access control systems.

### Design Issues as Bugs
>If it affects how your applicaiton is used then bad design is a bug.
>
>Should be tracked by bug tracking software.

### Prototyping Interfaces
*  Vet designs.
*  User paper mock-ups.
*  Make sure plasticity is know.
