<link rel="stylesheet" href="proj-css/talk.css">

<!--Cover Slide-->

<span style="font-size: 5rem; color: #9b6bcc">
  <!--<a href="https://twitter.com/purpleteamlabs" target="_blank"><i class="fab fa-twitter"></i> purpleteamlabs</a>-->
  <a href="https://twitter.com/purpleteamlabs" target="_blank"><i class="fab fa-twitter"></i> purpleteamlabs</a>
</span>

----  ----

<!-- .element: data-background-image="proj-img/shirt.png" data-background-opacity="0.8" -->

# What is OWASP?

Note:
* PurpleTeam is a security regression testing CLI (front-end) and SaaS (back-end) targeting Web applications and APIs, specifically built for Developers
* The CLI is specifically targeted at sitting within your build pipelines (run headless) but can also be run manually (with a CUI)
* You can choose from either `local` and/or `cloud` environments
  * If `local`: You need to set-up both front-end (CLI) & back-end micro-services
  * If `cloud`: All you need to do is get the CLI on the system you want to run it from, configure it and create a _Job_ file 

----

<!-- .element: data-background-image="proj-img/OWASP_PT.png" data-background-opacity="0.7" -->

## The Journey

</br></br></br></br></br></br></br>

Note:
Discuss: the 4 year journey that has brought PurpleTeam from a proof of concept (PoC) to where it is now.

* Finished writing book series to help Developers up-skill their security
* Lots of workshops with the PoC to elicit Developer feedback and confirm that what I wrote about was actually true
* Most of that time has been 7 days a week, two full time jobs
* I donated PurpleTeam `local` to OWASP in Q1 2021
* PurpleTeam `cloud` went to market in Q4 of 2021
* I couldn't get the publicity that was needed to get enough customers on-board to make `cloud` financially viable plus family relationships were getting strained. So I donated `cloud` to OWASP in Q1 2022
* So now the community gets to reap the benefits of a production ready hosted security regression testing SaaS that you can plug into your build pipelines to continuously test your web apps and APIs


Building a tool that helps Developers write secure code is a great way to learn about security.
If you want to learn more about information security, We'll assign you a mentor, and you can help your self and the community by building PurpleTeam.

----

![PurpleTeam Cloud Architecture](proj-img/purpleteam_cloud_2021-08-min.png) <!-- .element: class="borderless" -->

Note:
Discuss

----

![PurpleTeam Local Architecture](proj-img/purpleteam_local_2021-08-min.png) <!-- .element: class="borderless" -->

Note:
Discuss

----  ----

# Why?

Note:
(3 min - 3 min section)

* How does PurpleTeam help us as Developers?
* How does PurpleTeam help us as a business that creates software?
* Why would I want PurpleTeam in my build pipelines?

To answer these questions, I'm going to take you back to a section that's in a number of my previous talks.

----

## Traditionally

How have we found bugs in software?

<p><span class="fragment">Um... </span><span class="fragment">We haven't really</span></p>

Note:
Traditionally, how have we found security bugs in the software we write?

1. Basically,
2. we haven't really, or we've done it really late  

----

<p>The catch all <span class="fragment highlight-red">Red Team</span>ing Exercise </p>

Note:
* So...

---

1. Our red team has a week or two to find all the defects we've be conscientiously adding for months

----

<p>The catch all <font color="#ff2c2d">Red Team</font>ing Exercise </p>

* <!-- .element: class="fragment fade-right" style="text-align:left" --> ≈$20k per week
* <!-- .element: class="fragment fade-right" style="text-align:left" --> ≈Engagement: two weeks
* <!-- .element: class="fragment fade-right" style="text-align:left" --> ≈Software project before release: six months
* <!-- .element: class="fragment fade-right" style="text-align:left" --> ≈$40k per six months - per project
* <!-- .element: class="fragment fade-right" style="text-align:left" --> Found: 5 crit, 10 high, 10 med, 10 low severity bugs
* <!-- .element: class="fragment fade-right" style="text-align:left" --> Many bugs left unfound waiting to be exploited
* <!-- .element: class="fragment fade-right" style="text-align:left" --> Business decides to only fix the 5 criticals
* <!-- .element: class="fragment fade-right" style="text-align:left" --> Each bug avg cost of 15+ x fixed when introduced
* <!-- .element: class="fragment fade-right" style="text-align:left" --> 5 bugs x 15 x $320 = $24000

Note:

----

<!-- .element: data-transition="none" -->

<p><font color="#ff2c2d">Red Team</font>ing</p>

<div class="intro">
  <div>
    <br><br><br><br>
    <p>Bottom line:</p>
  </div>
  <div>
    <img data-src="proj-img/Elephant.png" class="borderless">
  </div>
</div>

<ul>
  <li>6 months (2 week engagement): <font color="#ff2c2d">$40’000</font></li>
  <li>Only 5 Red Team bugs fixed: cost: <font color="#ff2c2d">$24000</font></li>
</ul>

<br>

Note:

----

<!-- .element: data-transition="none" -->

<p><font color="#ff2c2d">Red Team</font>ing</p>

<div class="intro">
  <div>
    <br><br><br><br>
    <p>Bottom line:</p>
  </div>
  <div> 
    <img data-src="proj-img/Elephant.png" class="borderless"> 
  </div>
</div>

* Too expensive
* Too late
* Too many bugs left unfixed

Note:
* Too expensive
* Too late
* Too many bugs left unfixed because it’s too late in the SDLC and each bug now costs 15* +

----

<!-- .element: data-background-image="proj-img/OWASP_PT.png" data-background-opacity="0.7" -->

Note:
* Instead of deferring the finding and fixing of security defects to a traditional red teaming exercise, PurpleTeam helps us find and fix our defects as we're creating them
* How? PurpleTeam runs against our Web Apps and APIs as we're creating them, informing us of the security defects we're introducing... in close to real-time
* PurpleTeam reports show us how to reproduce the attacks that found a given vulnerability, with tips on how not to introduce the same vulnerability again

So now we know we need PurpleTeam...

----  ----

# `local` set-up

Head to the <a href="https://purpleteam-labs.com/doc/local/set-up/" target="_blank">set-up</a> page

<table>
  <tbody>
    <tr>
      <td><a href="https://purpleteam-labs.com/doc/local/set-up/#docker-network" target="_blank">Docker Network</a></td>
      <td><a href="https://purpleteam-labs.com/doc/local/set-up/#testers" target="_blank">Testers</a></td>
    </tr>
    <tr>
      <td><a href="https://purpleteam-labs.com/doc/local/set-up/#your-system-under-test-_sut_" target="_blank">SUT</a></td>
      <td>&nbsp;&nbsp;&nbsp;&nbsp;<a href="https://purpleteam-labs.com/doc/local/set-up/#application-scanner" target="_blank">App Scanner</a></td>
    </tr>
    <tr>
      <td><a href="https://purpleteam-labs.com/doc/local/set-up/#lambda-functions" target="_blank">Lambda Functions</a></td>
      <td>&nbsp;&nbsp;&nbsp;&nbsp;<a href="https://purpleteam-labs.com/doc/local/set-up/#tls-scanner" target="_blank">Tls Scanner</a></td>
    </tr>
    <tr>
      <td><a href="https://purpleteam-labs.com/doc/local/set-up/#stage-two-containers" target="_blank">S2 Containers</a></td>
      <td>&nbsp;&nbsp;&nbsp;&nbsp;<a href="https://purpleteam-labs.com/doc/local/set-up/#server-scanner" target="_blank">Server Scanner</a></td>
    </tr>
    <tr>
      <td><a href="https://purpleteam-labs.com/doc/local/set-up/#orchestrator" target="_blank">Orchestrator</a></td>
      <td><a href="https://purpleteam-labs.com/doc/local/set-up/#purpleteam-cli" target="_blank">CLI</a></td>
    </tr>
  </tbody>
</table>

Note:
(6 min - 3 min section)

For `local`: discus

----

# `cloud` set-up

CLI

Note:
Just install the CLI, the rest is done for you

----

## CLI Install Options

* <a href="https://github.com/purpleteam-labs/purpleteam#clone-the-git-repository" target="_blank">Clone the git repository</a>
* <a href="https://github.com/purpleteam-labs/purpleteam#npm-install-locally" target="_blank">NPM install locally</a>
* <a href="https://github.com/purpleteam-labs/purpleteam#npm-install-globally" target="_blank">NPM install globally</a>

&nbsp;

## Configure CLI

Note:
* Clone the git repository option
  * If you are planning on running/debugging purpleteam standalone (with UI)
* NPM install locally
  * If you are planning on running/debugging purpleteam as a spawned NodeJS sub process, for example from your NodeJS build pipelines
* NPM install globally
  * If you are planning on running/debugging purpleteam from a build pipeline written in a different language

Configure the CLI

----  ----

# Run CLI

* <a href="https://github.com/purpleteam-labs/purpleteam#clone-the-git-repository-option" target="_blank">Clone the git repository</a>
* <a href="https://github.com/purpleteam-labs/purpleteam#npm-install-locally-option" target="_blank">NPM install locally</a>
* <a href="https://github.com/purpleteam-labs/purpleteam#npm-install-globally-option" target="_blank">NPM install globally</a>

Note:
(9 min - 16 min section)

The following are some ways that PurpleTeam can be run and utilised from the perspective of the CLI which is what drives the back-end:

* Clone the git repository option
  * If you are planning on running/debugging purpleteam standalone (with UI)
* NPM install locally
  * If you are planning on running/debugging purpleteam as a spawned NodeJS sub process, for example from your NodeJS build pipelines
* NPM install globally
  * If you are planning on running/debugging purpleteam from a build pipeline written in a different language

----  ----

# `cloud`

Note:
If you're using `cloud`, job done.

----  ----

# `local`

Note:
If you're using local, then there's a bit more to know about running the back-end components.

----

<h2><a href="https://purpleteam-labs.com/doc/local/workflow/" target="_blank">back-end components workflow</a></h2>

* Emulating the AWS Lambda service `local`y
* Debugging
* Full system run

Note:
Discuss: headings

Stop video capture now.

----

<!-- .element: data-background-iframe="https://www.youtube.com/embed/ACuaP-ZToKw" data-background-interactive -->

Note:
Discuss: Talk through videos

1. Start docker stats (optional)
2. Start docker-compose-ui
3. Host lambda functions
4. Start SUT
5. Bring S1 containers up
6. Start CLI

----

<!-- .element: data-background-image="proj-img/OWASP_PT.png" data-background-opacity="0.7" -->

<span style="font-size: 5rem; color: #9b6bcc">
  <!--<a href="https://twitter.com/purpleteamlabs" target="_blank"><i class="fab fa-twitter"></i> purpleteamlabs</a>-->
  <a href="https://twitter.com/purpleteamlabs" target="_blank"><i class="fab fa-twitter"></i> purpleteamlabs</a>
</span>

</br></br></br></br></br></br></br></br>

Note:
We're looking for contributors to come and join the OWASP PurpleTeam core team.

T-shirt?

* What's the biggest win that PurpleTeam can provide?
* What's the cheapest place to find and fix your security defects and how much more will it cost to find and fix at Post-Release?
   https://f0.holisticinfosecforwebdevelopers.com/chap06.html#leanpub-auto-cheapest-place-to-deal-with-defects


