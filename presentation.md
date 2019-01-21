<!-- $size: 16:9 -->
<!-- page_number: false -->
<span style="float:right;"> ![45% center](images/miraiworm-torrified.png)

#
#
#
#
# Online Privacy: 
## The ![6%](images/tor-logo.png) Network


#
#
#
#
#

<span style="float:left;">[![120%](images/cc-by-sa.svg)](http://creativecommons.org/licenses/by-sa/4.0/)</span>
<!-- Creative Commons Attribution-ShareAlike -->

---
#
#
#
#
#

# <center>Sharing is Caring </center>
*<center>Please copy, share, and remix!</center>*
#
#
<center> grab a copy of the presentation: 
  
[github.com/francisco-core/tecnical-intro-to-tor/](https://github.com/seandiggity/citizen-foss)
</center>


#
#
#
#
<span style="float:left;">[![120%](images/cc-by-sa.svg)](http://creativecommons.org/licenses/by-sa/4.0/)</span>
<!-- Creative Commons Attribution-ShareAlike -->&nbsp;  This presentation is under the Creative Commons Attribution-ShareAlike License

---
<!-- page_number: true -->
<!-- Motivation -->

![center ](images/steiner-dog-cartoon.jpg)
## <center> On the Internet, nobody knows you're a dog.</center>

----

![center 150%](images/rememberwhencartoon.jpg) 

---

# *Why is there a need for privacy?*
<!-- $theme: default -->

---

# Privacy 
## gives people a safe place

---

<span style="float:right"> ![20%](images/panopticon.jpg)</span>


# If everything is recorded, you never know what is going to be used against you

&nbsp;<!-- whitespace -->

# You self-censor

> Observation changes behavior

---

<span style="float:right">![40%](images/mass-surveillance-free-society.jpg)<span>

#
#
#
#
#

# Privacy is essential 
# for a ==Free Society==

---

# But...
# The Internet is NOT a private place

---

# With no additional protection
## we are exposed
--- 


# IP addresses are geolocated
## and sent allong with each message 
<span style="float:left"> ![150%](images/ipgeolocation.jpg)</span>
<span style="float:right" > ![](images/ipheader.jpg)<span>

---

# ISPs know every website you visit / services you use

![150%](images/ISPs.png)
<!-- source: https://manurevah.com/blah/en/blog/ISP-vs-VPN-vs-Tor -->

---

# HTTPS wide deployment is very recent

![80%](images/https-increase.png)

<!-- source https://www.youtube.com/watch?v=py2qmGbyhlw -->

---

<span style="float:right">![](images/cookie-monster.jpg)</span>

# Cookies

#
**Cookies** have been preverted from their original function
and abused to **track people** online for marketing purposes.

<span style="padding-top:30px;float:left">![](images/cookies-consent.png)</span>

---

# Browser Fingerprinting

<span style="float:right">![](images/fingerprint.png)</span>
<span style="float:left">![65%](images/browser-uniqueness_anonymity-set.png)</span>


<span style="float:left">from a [*"How Unique Is Your Web Browser?"* by Peter Eckersley](https://panopticlick.eff.org/static/browser-uniqueness.pdf)</span>

---

# Passive Analysis of the Internet Backbone

<span style="float:left">![70%](images/upstream.png)</span>
<span style="float:right">![100% center](images/cables.png)</span>

----

# Surveillance Capitalism

> The business model where **data is money**

<!-- more info on surveillance capitalism can be found here: https://www.youtube.com/watch?v=Ya1eTbTUUvc (Facebook & Google: The Age of Surveillance Capitalism by Forever Computing) -->

&nbsp;<!-- whitespace -->

<span style="float:left">![230%](images/zuck-surveillance.jpg)</span>

&nbsp;<!-- whitespace -->
&nbsp;<!-- whitespace -->


> # <span style="float:right"> &nbsp;&nbsp; ==driving force==</span>
> # <span style="float:right"> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;of surveillance </span>



---

# <center> So, what do we do about it? </center>
#


> ## <center> We create an anonymity network on top </center>
>
> ## <center> of a non-anonymous one </center>
#
#
#
<center> yeah, Computer Science has wonders like these</center>
  
---

# Approaches to Privacy and Anonymity

###### There are various approaches to anonymity online, with different trade-offs. 

---

# Single Proxy / VPN

![](images/vpns-claim-anonymity.png)

---

# Single Proxy / VPN

![](images/single_relay.png)

---

# <center> Major Flaws </center>

&nbsp;<!-- whitespace -->

## <center>  1. **Trust**  </center>
## <center>  2. **Liability for the Provider**  </center>
## <center>  3. **Traffic Correlation**  </center>

---

# 1. We have to Trust

&nbsp;<!-- whitespace -->

<span style="float:left">privacy **by Policy** </span>
<span style="float:right">privacy **by Design**</span>

<span style="float:left">![40%](images/privacy-policy.jpg)</span>

<span style="float:right">![60%](images/privacy-by-design.png)</span>
<!-- privacy by design logo is from the Privacy by Design Foundation (https://privacybydesign.foundation/) -->

---

# 2. Liability for the Provider

![center](images/gag-order.png)

---

# 3. Traffic Correlation
![](images/single_relay.png)

---

# Our activities are linkable
> A lead can lead to everything else

---

# VPNs are Pseudonymous

Through fingerprinting it is possible to indentify users

---

# Anonymity is Hard

---

# Onion Routing

* ## use a chain of relays
* ## public key encryption for each of them

---

# Onion Routing

<!-- Well, there must be a think with food metaphors on computer networks, because we have *Hot Potato Routing* and now *Onion Routing* -->

![](images/onion-routing.png)

---

<!-- The onion part comes from the fact that the packets look like an onion and after each step, one layer is peeled way -->
# I don't see any onions there...

<span style="float:right">![47%](images/onion-logo.png)</span>
<span style="float:left">![90%](images/onion_diagram.png)</span>

&nbsp;<!-- whitespace -->


<span style="float:left"> The *onion pattern* also comes up when we think of internet packets and their layers</span>

---

## Tor implements Onion Routing as an ==overlay network==

> Designed to anonymize **any TCP-based applications**
>
> through transparent proxy settings

<!-- Note: Show proxy settings to send any application through the tor proxy -->

<span style="float:right">![130%](images/tcp-ip-tor-model.png) </span>

&nbsp;<!-- whitespace -->

<span style="float:left"> ![70%](images/onion-routing.png) </span>

<!--So, the tor network is actually a collection of nodes/relays which forward your traffic to the next node. In total, it typically forwards it through 3 -->

---

# Onion Circuit
![180% center](images/onion-circuit.svg)

## A circuit is a sequence of 3 nodes: *==Guard==, ==Middle==* and *==Exit==*

---

# Nodes are ran by ==Volunteers== all around the World

![80% center](images/tor-relay-count.png)

---

# Not all Volunteers have good intentions

Tor is resistant to ==**bad relays**== to a certain extent 
But if they are too many it harms the nework and some uses might get de-anonymised

---

# How to decide which nodes are part of the network?

---

# Consensus Mechanism 

![120% center](images/authorities.png)
<!-- taken from this article detailing the consensus mechanism: https://jordan-wright.com/blog/2015/05/14/how-tor-works-part-three-the-consensus/ -->
#
Anyone can see the votes of each relay by downloading `http://[directory_authority]/tor/status-vote/current/consensus/` 

#

Typically this is fetched trough http but now it can be fetched through tor, leaving less traces that the user is using tor.

The ==**consensus status**== can be found [here](https://consensus-health.torproject.org/consensus-health.html)

---

# Your computer chooses the circuit

<!-- explain to people that it's their computer that chooses the circuit and no-one else -->
<!-- 1. Retrieve the list of available nodes
2. Choose three nodes (Guard, Middle, Exit)
3. Establish Circuit -->

---

# Anonymity is Fragile

Everything we do is identifying:
* the pattern of our browsing habits
* the way we write text
* the way we code
* our typing speed, etc

#
#
###### This means that
## Tor alone is ==not enough==

<!-- Anonymity is the lack of identity, as opposed to simply pseudonymity where one keeps the identity hidden under an alias. The problem with the later is that there is a data trail of the stuff done under that alias and it is only needed one identifying detail or some association, to connect that identity with the irl person behind it. With perfect anonymity, you cannot be distinguished from any other anonymous person. Think of various people with the exact same closes, height, face, etc. While an alias is wearing a different mask, but always the same one.-->

<!-- # Anonymity is identifiability only in one's actions 
<!-- image and quote from here https://concurringopinions.com/archives/2011/01/privacy-vs-security-vs-anonymity.html-->

<!---![140% anonymity is identity in one's actions](/home/user/Storage/Projects/PrivacyGroup/Events/TechnicalIntroductionToTor/images/anonymity_actions.jpeg)-->

<!-- The Tor does allow you to be anonymous, but with no additional measures, it would be trivial to see you're the same person who visited this or that website last time, given enough resources.-->

--- 

# Tor Browser

A browser developed by the Tor Project that:
* sends traffic through the Tor network
* Implements additional measures to prevent the user to unwittingly giving away her/his identity
#
![80% center](images/tor-browser.png)

---

<span style="float:right;padding-top:30px"> ![106%](images/stream-isolation.jpg) </span>

# Stream Isolation

**Identity Correlation**: If the user is reading emails
at the same time of browsing the web the activities can be correlated and the user identified

To fight this Tor implements **Stream Isolation**
Creates a different circuit for each website / applic.

<!-- Since Anonymity requires unlink-ability we must separate as much as possible different sources of information. This is why we do **Stream Isolation** -->


<span style="float:left"> ![80%](images/onion-circuits.png) </span>

---

<span style="float:right">![50%](images/deep-web-propaganda.jpg)</span>


# Onion Services

> "End-to-End" Anonymity
>
> Aka. "" The Dark Web ""
#
The traffic never leaves the Tor network

Privacy for the user and the website operator.


<!-- Both parties benefit from the anonymity provided by the tor network. The messages never leave the TOR network. And there is no need for DNS of any sort. The addresses are something like http://sik5nlgfc5qylnnsr57qrbm64zbdx6t4lreyhpon3ychmxmiem7tioad.onion/ The address is in fact the public key of the onion, meaning that if you have the address right, then you are talking exactly to the right person. No domain hijacking can happen because the only person able to prove that that address is theirs is the person with the cryptographic private key, meaning the one who runs the server and no one else. Being that DNS is currently the weakest link in the whole Internet infrastructure, this is quite an improvement, given  that we don't mind the small delay introduced.-->

<!-- What if you want to run a website without having to reveal private information? You can do that with onion services. -->
#
#
#
<span style="float:right">example of **misinformation** </span>
<span style="float:right">about onion services</span>
#
###### <span style="float:right">(they only account for 3% of all tor traffic)</span>

---

# How does it look like?
Version 2: http://qubesos4rrrrz6n4.onion/
Version 3: http://sik5nlgfc5qylnnsr57qrbm64zbdx6t4lreyhpon3ychmxmiem7tioad.onion/

---

# Self Authentication

**No need** for Certificate Authorites


#
#
## The URL is the publick key
correct URL = correct website 

[http://sik5nlgfc5qylnnsr57qrbm64zbdx6t4lreyhpon3ychmxmiem7tioad.onion/](http://sik5nlgfc5qylnnsr57qrbm64zbdx6t4lreyhpon3ychmxmiem7tioad.onion/) 

---

<!-- more info on onion services can be found here: https://www.torproject.org/docs/onion-services -->

![center 140%](images/tor-onion-services-1.png)

---

![center 140%](images/tor-onion-services-2.png)

---

![center 140%](images/tor-onion-services-3.png)

---

![center 140%](images/tor-onion-services-4.png)

---

![center 140%](images/tor-onion-services-5.png)

---

# Censorship Resistance

A direct consequence of anonymity
#
> If I don't know who you are or where you go, 
> I cannot block you access based on that information

<!--If they don't know where you are, they cannot deny you access base on you're location. If they do, you just change it in a second. This works unless they block Tor specifically -->

---

# Resources

Where you can find more information about how Tor works:

* [A soft introduction to the Tor network written in Spanish](https://tor.derechosdigitales.org/torificate/)
* [Read the Orignal paper of tor](https://svn.torproject.org/svn/projects/design-paper/tor-design.pdf)
* Thirteen key design changes since the original 2004 paper: [part one](https://blog.torproject.org/blog/top-changes-tor-2004-design-paper-part-1), [part two](https://blog.torproject.org/blog/top-changes-tor-2004-design-paper-part-2), [part three](https://blog.torproject.org/blog/top-changes-tor-2004-design-paper-part-3). 
* [Tor Documentation](https://www.torproject.org/docs/documentation.html.en)

---

# Image credits
*Copyright of the images to their respective owner. Used for the purpose of illustration*
| image | credit |
|-------|--------|
|![10%](images/miraiworm-torrified.png)| Hard to credit but it seems to come from an article from [wired](https://www.wired.com/2016/12/botnet-broke-internet-isnt-going-away/). The image was based on that one, but modified to add all of tor and nsa's logos.|
| ![](images/steiner-dog-cartoon.jpg) | "On the Internet, nobody knows you're a dog" <br>The [famous cartoon](https://en.wikipedia.org/wiki/On_the_Internet%2C_nobody_knows_you're_a_dog) by Peter Steiner.

---

| image | credit |
|:-----:|--------|
|![](images/rememberwhencartoon.jpg)  | The 2015 upgrade to the decades-old cartoon made by  Kaamran Hafeez and published in The New Yorker on February 23, 2015<br><br>|
|![10%](images/panopticon.jpg) | A very nice illustration of the Panopticon prision concept.<br>Taken from an [NYtimes article](https://www.nytimes.com/2013/07/21/books/review/the-panopticon-by-jenni-fagan.html) |

----
| image | credit |
|:-----:|-------|
|  ![10%](images/mass-surveillance-free-society.jpg)     |   made by [Privacy International](https://privacyinternational.org/feature/2300/what-european-court-ruling-means-mass-spying-around-world)     |
|  ![30%](images/ISPs.png)   |  Taken from [this blog](https://manurevah.com/blah/en/blog/ISP-vs-VPN-vs-Tor)      |
| ![30%](images/privacy-by-design.png)| privacy by design logo is from the [Privacy by Design Foundation](https://privacybydesign.foundation/)|
| ![25%](images/onion-routing.png) | From Brian Ford's article ["Seeking Anonymity in an Internet Panopticon"](https://arxiv.org/abs/1312.5307)<br>

---

| image | credit |
|:-----:|--------|
|![10%](images/onion-logo.png)| [Tor's logo](https://torproject.org)|
|![25%](images/onion_diagram.png) | [Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Onion_diagram.svg)|
| ![20% center](images/tor-relay-count.png) | You can find more fancy graphics of on [tor metrics](https://metrics.torproject.org/) |
|![40% center](images/authorities.png)|Taken from [this article](https://jordan-wright.com/blog/2015/05/14/how-tor-works-part-three-the-consensus/) detailing the consensus mechanism

----

| image | credit |
|:-----:|--------|
| ![60%](images/onion-circuit.svg) | more similar diagrams [here](https://www.torproject.org/about/overview)|
| ![85%](images/onion-circuits.png) | [Onion Circuits](https://tails.boum.org/doc/anonymous_internet/tor_status/index.en.html) is an application for viewing the current open and build tor circuits. It's quite good for new people using tor as they can see all that is going on in the background without it being too technical.|
| ![20%](images/stream-isolation.jpg) | Image of stream isolation of [whonix](https://www.whonix.org/wiki/Stream_Isolation). Taken from their wiki. |
|![60%](images/cookie-monster.jpg) | Hard to credit, but easy to love.<br>It seems the oldest version of the image comes from [here](https://www.swzone.it/Garante-Privacy--norme-piu-severe-che-regolamentano-i-cookie-40115.html). |