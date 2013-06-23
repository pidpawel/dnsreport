dnsreport
=========

Dnsreport is a simple tool to query DNS servers not only about the "first level" of records but also the deeper ones.

[License CC-BY-SA 3.0](http://creativecommons.org/licenses/by-sa/3.0/)

Authors: 
* [pidpawel](http://pidpawel.eu)
* [aysorth](http://aysorth.net)

### Example output:
```
$ dnsreport github.com
github.com using nameserver default
├─ SOA
│  ╰─ns1.p16.dynect.net. hostmaster.github.com. 1371943718 3600 600 604800 60
├─ A
│  ╰─204.232.175.90
│    ╰─github.com.
├─ AAAA
├─ MX
│  ├─20 ALT1.ASPMX.L.GOOGLE.com.
│  ├─10 ASPMX.L.GOOGLE.com.
│  ├─20 ALT2.ASPMX.L.GOOGLE.com.
│  ├─30 ASPMX3.GOOGLEMAIL.com.
│  ╰─30 ASPMX2.GOOGLEMAIL.com.
├─ SRV
├─ TXT
│  ╰─"v=spf1 include:_spf.google.com include:support.zendesk.com include:sendgrid.net include:mailgun.org a:smtp1-ext.rs.github.com ~all"
├─ DNAME
├─ NS
│  ├─ns2.p16.dynect.net.
│  ├─ns4.p16.dynect.net.
│  ├─ns1.p16.dynect.net.
│  ╰─ns3.p16.dynect.net.
├─ SPF
│  ╰─"v=spf1 include:_spf.google.com include:support.zendesk.com include:sendgrid.net include:mailgun.org a:smtp1-ext.rs.github.com ~all"
├─ PTR
├─ RP
╰─ CNAME
```
