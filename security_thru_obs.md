# Security Through Obscurity
- It is the practice of trying to protect a system by keeping its design, implementation, or configuration secret. The idea is that if attackers don't know how something works, they can't exploit it,
like:
1. hiding a web admin panel at a non-standard URL like /secret-admin-xyz123 instead of /admin
2. keeping the source code of your application completely private

**But**, Security through obscurity is generally considered weak as a primary security measure because secrets can be discovered through reverse engineering and leaks    
Once the secret is out, your entire security model collapses     
It provides a false sense of security     
**Althouth**, it's acceptable as a supplementary layer on top of proper security measures. For instance, changing default ports won't stop a determined attacker, but it might reduce automated scanning attacks.

The principle here is: never rely on secrecy of your methods as your main protection. Good security should work even if the attacker knows exactly how your system operates (Kerckhoffs's principle in cryptography says this).
