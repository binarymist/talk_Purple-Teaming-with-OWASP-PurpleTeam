<link rel="stylesheet" href="proj-css/talk.css">

<!--Cover Slide-->

## Community Topics

* Welcome
* InfoSecNZ Slack, OWASP Slack
* <!-- .element: class="fragment fade-right" --> Anything else people want to mention?
* <!-- .element: class="fragment fade-right" --> Tonights talk (Chris - Incident Response), (Me - Application Intrusion Detection)

Note:
* Hand over to Chris

----  ----

# Application Intrusion Detection

----  ----

HIDS, NIDS, AIDS?


Note:
Some TLAs

----  ----

1. Asset Identification
2. Identify Risks
3. Countermeasures
4. Risks that Solution Causes
5. Costs and Trade-offs

Note:
* As with everything security, let's threat model it
* As usual (same with all my books), I like to use the SSM

----  ----

1. SSM&nbsp;&nbsp;&nbsp;<span style="font-size: 4rem;">Asset Identification</span>

Note:
* What are the attackers after?
* The value of your assets will determin how much your attacker is willing to spend

----  ----

2. SSM&nbsp;&nbsp;&nbsp;<span style="font-size: 4rem;">Identify Risks</span>

----

* Lack of Visibility
  * Insufficient Logging (->) & Monitoring (<-)<br/>Covered in <a href="https://f1.holisticinfosecforwebdevelopers.com/chap06.html#leanpub-auto-insufficient-logging-and-monitoring" target="_blank">Holistic Info-Sec for Web Developers</a><br/><a href="https://owasp.org/www-project-top-ten/2017/A10_2017-Insufficient_Logging%2526Monitoring" target="_blank">No. 10</a> for OWASP Top 10
* Insufficient Attack Protection
  * Book -> <a href="https://f1.holisticinfosecforwebdevelopers.com/chap06.html#leanpub-auto-insufficient-attack-protection" target="_blank">Lack of Active Automated Prevention</a>

Note:
* Talk through my book
* Talk through OWASP A10: top & left panels
* Talk through "Lack of Active Automated Prevention"

----  ----

3. SSM&nbsp;&nbsp;&nbsp;<span style="font-size: 4rem;">Countermeasures</span>

----

* Lack of Visibility ...

_Detection works where prevention fails and detection is of no use without response_

Bruce Schneier

----

* Lack of Visibility</br>OWASP Top 10 - <a href="https://owasp.org/www-project-top-ten/2017/A10_2017-Insufficient_Logging%2526Monitoring" target="_blank">A10</a></br><a href="https://f1.holisticinfosecforwebdevelopers.com/chap06.html#leanpub-auto-insufficient-monitoring" target="_blank">Kim's book</a>
    * Insufficient Logging
    * Insufficient Monitoring

Note:
* Talk through the "How to Prevent" section of OWASP A10
* Talk through My book: Dark Cockpit, Statistics Graphing with the likes of statsd, collectd, graphite
* The tools you use depend largly on your environment  
  You'll need something to:
  * Capture and push the events
  * Collect, aggregate, display & alert on the events
    * SIEM (Security information & event management) type tools

----

* <a href="https://f1.holisticinfosecforwebdevelopers.com/chap06.html#web-applications-countermeasures-insufficient-attack-protection" target="_blank">Insufficient Attack Protection</a>
  * WAF
  * App Intrusion Detection & Response
  * Active Automated Prevention

Note:
* WAF is the last thing I like to apply,  
  They're like a band-aid, generally they don't have intimate knowledge of your application
* Talk through "Application Intrusion Detection and Response"
* Talk through "Active Automated Prevention"

----

App Intrusion Detection->Prevention is reactive

Note:
* This is fine as a layer of defense
* But we can do better/more
* How?

----

By being proactive -> 
<a href="https://owasp.org/www-community/Free_for_Open_Source_Application_Security_Tools" target="_blank">SAST, DAST</a>

Note:
* We can do better/more by removing your app vulnerabilities in the first place.  
  With concepts & tooling such as SAST & DAST as part of your Dev work-flows
* If you want to get serious about app-sec, you really need to apply defence in depth

----  ----

It's been <a href="https://owasp.org/www-chapter-new-zealand/#div-history" target="_blank">8 years</a>

* <!-- .element: class="fragment fade-right" --> <a href="https://purpleteam-labs.com" target="_blank">purpleteam</a> now in alpha and releases being published regularly
* <!-- .element: class="fragment fade-right" --> It's time to let someone else take over
* <!-- .element: class="fragment fade-right" --> Pete Nicholls is taking over from me
* <!-- .element: class="fragment fade-right" --> Next Meetup Last Wed of Sep - Pete & Toni - Ask anything panel

Note:
1. I've lead the Chch chapter for 8 years
2. I'm stepping down, but I'm leaving you with PurpleTeam
3. It's time to let someone else take over
4. You'll be in the safe hands of Pete Nicholls

