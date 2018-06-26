+++
title = "DevOps Days MSP 2018"
outputs = ["Reveal"]

[reveal_hugo]
theme = "moon"
+++

## They Didn't Stop To Think If They Should: Machine Learning And The Internet Of Unpatched Things

### Tim Gross

#### Machinist Labs | @0x74696d

---

(image of "NTSB self-driving Uber did not have emergency braking turned on")

{{% note %}}
https://www.washingtonpost.com/news/dr-gridlock/wp/2018/05/24/ntsb-self-driving-uber-did-not-have-emergency-braking-turned-on/
{{% note %}}

---

(image of "Twitter taught Microsoft's AI chatbot to be a racist asshole in less than a day")

{{% note %}}
https://www.theverge.com/2016/3/24/11297050/tay-microsoft-chatbot-racist
{{% note %}}

---

(image of "NHS hospitals randomware hack wannacry")

{{% note %}}
https://www.theverge.com/2017/5/12/15630354/nhs-hospitals-ransomware-hack-wannacry-bitcoin
{{% note %}}

---

(image of "Tesla car that crashed and killed driver was running on Autopilot, firm says")

{{% note %}}
https://www.theguardian.com/technology/2018/mar/31/tesla-car-crash-autopilot-mountain-view
{{% note %}}

---

(image of "how target figured out teen girl was pregnant")

{{% note %}}
https://www.forbes.com/sites/kashmirhill/2012/02/16/how-target-figured-out-a-teen-girl-was-pregnant-before-her-father-did/#5e6d24926668
{{% note%}}

---

(image of "Google sorry for racist auto tag photo app")

{{% note %}}
https://www.theguardian.com/technology/2015/jul/01/google-sorry-racist-auto-tag-photo-app
https://www.theguardian.com/technology/2015/may/20/flickr-complaints-offensive-auto-tagging-photos
{{% note %}}

---

(image of "defeat the baby")

{{% note %}}
https://twitter.com/yipe/status/1005555741153902592
{{% note %}}

---

(image of alexa eavesdropping)

{{% note %}}
https://www.wsj.com/articles/amazon-alexa-powered-device-recorded-and-shared-users-conversation-without-permission-1527203250~

https://www.huffingtonpost.com/entry/alexa-eavesdropping-portland-familiy_us_5b0727cae4b0fdb2aa51b23e
{{% note %}}


---

## Machine Learning and IoT as a problem of scale:

## quantity has its own quality

{{% note %}}
these are the speaker notes
{{% note %}}

---

- scope is so large that creating meaningful consent is difficult
- ex. while ML "models" are probably reasonably well-understood by the elite developers of the best organizations, most users of ML treat the models as binary blobs -- a black box into which numbers go and decisions come out

https://www.theatlantic.com/technology/archive/2013/10/avoid-facial-detection-algorithms-with-a-t-shirt/280253/

https://cdn.vox-cdn.com/uploads/chorus_asset/file/9969109/Screen_Shot_2018_01_03_at_3.05.16_PM.png

https://www.theverge.com/2018/1/3/16844842/ai-computer-vision-trick-adversarial-patches-google

https://www.theverge.com/2016/11/3/13507542/facial-recognition-glasses-trick-impersonate-fool

---

https://thenewstack.io/camouflaged-graffiti-road-signs-can-fool-machine-learning-models/

> The team found that with this approach, they were able to confuse a machine 100 percent of the time into classifying a stop sign as a 45-mile-per-hour speed limit sign, and a right-turn sign as a stop sign.

---

ex. IoT "secure boot" is typically considered optional (without which *any* device can be rooted)

---

http://www.eclipse.org/hawkbit/documentation/images/hawkbit_logo.png

https://m.media-amazon.com/images/G/01/DeveloperBlogs/AmazonDeveloperBlogs/legacy/AWS_IoT23._CB520207442_.png


- ex. existing solutions for IoT Over-the-Air updates (OTA) are mostly research projects at best (ex. Hawkbit) or require trust delegation and put secure boot at risk

---

## Industry abdication of responsibility invites political and legal remedy


---

https://www.brookings.edu/wp-content/uploads/2016/06/congress006-1.jpg

{{% note %}}

legal remedy is likely to be ham-fisted...
{{% note %}}

---

https://imgur.com/gallery/2mIObIu

{{% note %}}
...particularly here in the US where almost all our lawmakers are incompetent...
{{% note %}}

---

https://www.engadget.com/2017/05/18/fcc-chairman-net-neutrality-1996/

{{% note %}}
... or are entirely co-opted by hostile interests
    {{% note %}}

---

software is typically sold w/o warantee for fitness for any particular use; this could change --> do you want to be *personally liable* for bugs in your code?!

---

GPL:

> 15. Disclaimer of Warranty.
> THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM “AS IS” WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.

> 16. Limitation of Liability.
> IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.

---

Apache:

> 7. Disclaimer of Warranty. Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.

> 8. Limitation of Liability. In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.

> 9. Accepting Warranty or Additional Liability. While redistributing the Work or Derivative Works thereof, You may choose to offer, and charge a fee for, acceptance of support, warranty, indemnity, or other liability obligations and/or rights consistent with this License. However, in accepting such obligations, You may act only on Your own behalf and on Your sole responsibility, not on behalf of any other Contributor, and only if You agree to indemnify, defend, and hold each Contributor harmless for any liability incurred by, or claims asserted against, such Contributor by reason of your accepting any such warranty or additional liability.

---

(GDPR childishness)
https://apility.io/2018/05/25/gdpr-lazy-block-european-users-cloudflare-workers/

https://twitter.com/internetofshit/status/999619364541394944

https://techcrunch.com/2018/05/05/unroll-me-to-close-to-eu-users-saying-it-cant-comply-with-gdpr/

https://news.ycombinator.com/item?id=16954306

---

Salesforce CEO Marc Benioff thinks America needs "a national privacy law... that probably looks a lot like GDPR."

"This is going to help our industry... It's going to set the guardrails around trust, around safety. It's going to provide the ability for the customers to interact with great next generation technologies in a safe way."

Benioff went on to say that as artificial intelligence is used in customer service, "that starts to cross the line on what is trust. And that's where our industry really has to come forward and say we're going to make sure that these technologies are trust-based. And I think the Europeans definitely got that figured out."


https://www.theregister.co.uk/2018/05/30/salesforce_q1_2019/?


---

https://twitter.com/soniagupta504/status/1011591288003575808


---

# Consent

{{% note %}}
Flaws of the Consent Model as a Solution
consent is the *only* workable guiding model when we're talking about relationships between individual people. I consent to
{{% note %}}

---

# Individual vs Community Consent

{{% note %}}
every culture has different boundaries here.
ex. in the EU they protect individual consent strongly...
{{% note %}}

---

## Businesses are being treated as a "community consent" situation rather than an "individual consent" one

{{% note %}}
... whereas in the US we have a mixed bag where businesses get the power of community consent to override the will of individuals, but very little of the responsibility of individual consent.
{{% note %}}

---

https://img.washingtonpost.com/news/volokh-conspiracy/wp-content/uploads/sites/14/2015/05/Kelo-House-Frontal-view-same-as-cover-of-LPH-e1432877841421.jpg

https://www.washingtonpost.com/news/volokh-conspiracy/wp/2015/05/29/the-story-behind-the-kelo-case-how-an-obscure-takings-case-came-to-shock-the-conscience-of-the-nation/

---

## Externalities

![externality](img/externality-definition.png)
*https://www.google.com/search?q=externality*

{{% note %}}
also, are these results being manipulated? the *canonical* example is pollution!
{{% note %}}

---

- ethical definitions vary b/c values vary (ex. balance of community vs individual consent varies significantly between Europe and the US)

---

![gdpr-tumblr](img/tumblr-gdpr.png)
*https://twitter.com/Millstab/status/999762424994594817*

{{% note %}}
informed consent is rare, but "consent" is manipulated by dark UX patterns
{{% note %}}

---

# Professional Ethics

---

- history of professional organizations (ex. AMA, AIA, ASME, bar associations)
- government licensing requirements are typically delegated to the professional organizations
- professional organizations mostly act to counter information asymmetry rather than create monopoloy power (ref http://www.nber.org/papers/w10467.pdf), but...
- professional organizations inherently act against the direction we want to take our industry wrt inclusion, ability to bootstrap into the middle class
- professional certification w/o regulation or consequences is toothless and worthless (ex. CompTIA or ICS^2 or Project Management Institute)
- professional organizations ethical requirements are typically about fair dealing and bare minimum safety guidelines

---

- an advantage of a professional organization's ethical framework is that it at least gives a shared baseline: right now we're all trying to figure this out for ourselves.
- we should hold each other to task
- we should also cut each other some slack (e.g. ensure your own mask is secure before helping others)

---

4. what can be done? individual action:

- influence the community
- ex. talk about this stuff!
- ex. what organizations do we work for?

---

- influence the organization:
- ex. Google employees protest of military contracts
- ex. Microsoft employees protest of ICE contracts
- ex. D&I efforts
- ex. hiring practices

https://arstechnica.com/tech-policy/2018/06/microsoft-staff-call-on-company-to-end-ice-contract/

https://www.reuters.com/article/uk-alphabet-defense/google-to-scrub-u-s-military-deal-protested-by-employees-source-idUKKCN1IX5YC

https://gizmodo.com/amazon-workers-demand-jeff-bezos-cancel-face-recognitio-1827037509


---

- direct action at an engineering level:
- ex. immutable event data storage
- ex. dark UX patterns
- ex. choosing model inputs that reflect the population

---

- ex. secure-by-default; bypass business analysts opinions that are purely technical; "no one was ever fired for using best practices" --> these things typically don't make it into a JIRA story on their own; you're a professional, act like it!

---

- align engineering ethics with business needs (ex. "if we pick machine vision training data that reflects real demographics, we can avoid the embarassment for our organization of having to explain why our software acts racist.")
- we can't rely on project managers or business analysts to take the lead on designing our systems ethically because they simply may not understand the side-effects. you're the technical professional: they're expecting you to take the lead on this!
