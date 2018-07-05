+++
title = "DevOps Days MSP 2018"
outputs = ["Reveal"]

[reveal_hugo]
custom_theme = "./css/devopsdays.css"
highlight_theme = "solarized-dark"

+++

# They Didn't Stop To Think If They Should

#### Tim Gross | Machinist Labs

{{% note %}}
My name is Tim Gross from Machinist Labs, and my talk is titled "They Didn't Stop to Think If They Should"
{{% /note %}}

---

## or...
## Machine Learning And The Internet Of Unpatched Things

{{% note %}}
an alternate title could be...
{{% /note %}}

---

## or...
## Because Eternal Vigilance is the Price of Liberty, We Have to Talk About Ethics of the Tech Industry Again

---

> We've updated our privacy policy!

> The opinions expressed in this talk are the speaker's alone and do not reflect the view of this conference, your employer, or my mom. Any reference to or citation of any person or organization does not constitute or imply an endorsement or recommendation of the content of this talk. The speaker is grossly unqualified to tell you how to live you life. Your mileage may vary. Not to be used in the manufacture of nuclear weapons. By attending this talk the speaker hereby grants you an irrevocable, perpetual, non-exclusive, transferable, worldwide license to be excellent to each other.

{{% note %}}
why is it especially important to talk about ethics when we start talking about ML and IoT? What makes these things special? What makes them different from other software? Why do we as engineers even need to discuss this stuff? "Ethics is hard!" "C'mon, I just want to code!" Who am I, anyways? basically nobody. I'm not an ethicist w/ a PhD, and even though I've worked on ML and IoT projects, I'm not some guru. and that's important because we *all* need to be talking about this stuff.
{{% /note %}}

---

![uber-self-driving](img/uber-accident.png)

*[Michael Laris, Washington Post, 24 May 2018](https://www.washingtonpost.com/news/dr-gridlock/wp/2018/05/24/ntsb-self-driving-uber-did-not-have-emergency-braking-turned-on/)*


{{% note %}}
Back in March a self-driving car operated by Uber killed a pedestrian. The NTSB investigation is still ongoing, but what is clear is that the vehicle had no business being operated without direct supervision. The sensing system had lots of false positives that caused it to brake erratically. So they turned the braking system off. But apparently that message never got to the folks who'd turned off the vehicles' own automatic braking nor to the attendee of the vehicle. So the vehicle "saw" the pedestrian and did nothing.
{{% /note %}}

---

![microsoft-chatbot](img/microsoft-chatbot.png)

*[James Vincent, The Verge, 24 Mar 2016](https://www.theverge.com/2016/3/24/11297050/tay-microsoft-chatbot-racist)*

{{% note %}}
A couple years ago, MSFT demonstrated their ML capabilities with the Tay chatbot. They let it loose to learn from whatever racist trolls wanted to teach it. The experiment was stopped and the whole debacle embarrassed MSFT. Now clearly the horrible Internet people are primarily to blame here, but the researchers failed to anticipate the "side channel" attacks inherent to their system
{{% /note %}}

---

![uk-ransomware](img/uk-ransomware.png)

*[Russell Brandom, The Verge, 12 May 2017](https://www.theverge.com/2017/5/12/15630354/nhs-hospitals-ransomware-hack-wannacry-bitcoin)*

{{% note %}}
in an IoT example, last year countless devices in UK hospitals were taken over by Wannacry ransomware. patient lives were put at risk not just because of poor patch hygiene but because of the design flaws that allowed access to the devices in the first place and because of warped incentives in the government programs that produced the stolen malware in the first place.
{{% /note %}}

---

![tesla-autopilot](img/tesla-autopilot.png)

*[The Guardian, 31 Mar 2018](https://www.theguardian.com/technology/2018/mar/31/tesla-car-crash-autopilot-mountain-view)*

{{% note %}}
Tesla's autopilot has been implicated in the deaths of several drivers at this point. We (and Tesla stockholders, apparently) are constantly reassured that these are the result of improper handling and not rushing these systems into the real world before they're ready.
{{% /note %}}

---

![target-pregnant](img/target-pregnant.png)

*[Kashmir Hill, Forbes, 16 Feb 2012](https://www.forbes.com/sites/kashmirhill/2012/02/16/how-target-figured-out-a-teen-girl-was-pregnant-before-her-father-did/)*

{{% note %}}
Machine learning algorithms may know more about us and our loved ones than we do ourselves. Target was able to determine from customer purchases not just when customers are pregnant but at what stage of their pregnancy they were (buying unscented products during late stages, for example).
{{% /note %}}

---

![google-racist-autotag](img/google-racist-autotag.png)

*[Jana Kasperkevic, The Guardian, 1 Jul 2015](https://www.theguardian.com/technology/2015/jul/01/google-sorry-racist-auto-tag-photo-app)*

{{% note %}}
ML is simultaneously unconsciously encoding our biases. (This one was so bad that I cropped it out of this picture.)
{{% /note %}}

---
![defeat-the-baby](img/defeat-the-baby.png)
  *
*https://twitter.com/yipe/status/1005555741153902592*

{{% note %}}
we've invited these systems into our homes... (and ok, yeah this is funny)
{{% /note %}}

---

![alexa-eavesdropping](img/alexa-eavesdropping.png)

*[Laura Stevens, Huffington Post, 24 May 2018](https://www.huffingtonpost.com/entry/alexa-eavesdropping-portland-familiy_us_5b0727cae4b0fdb2aa51b23e)*

{{% note %}}
... with almost no oversight into what they're doing. We have unaccountable closed source microphones in our homes, who do who-knows-what with that information
{{% /note %}}

---

![marco](img/marco-rogers.png)

{{% note %}}
what all these stories have in common is that like any other failure there's almost certainly no "root cause"; it's unlikely that anyone at these companies set out with awful intentions. It's a complex combination of socio-technical systems and the incentives they set up. But at the end of the day, it's people in our industry -- the people in this room -- who are the ones who execute and implement these systems
{{% /note %}}

---

# a problem of scale

{{% note %}}
the problem we have here is not just that these systems all have serious real-world consequences; we can look at the Therac-25 accidents in the 80's for examples of that. the problem is that those consequences are multiplied by the scale of these systems.
{{% /note %}}

---

## quantity has its own quality

{{% note %}}
a huge part of the value proposition of IoT and ML is the scale of the data involved: collecting massive amounts of data from edge computing devices, and processing massive amounts of data in ML models.
{{% /note %}}

---

## no meaningfully informed consent

{{% note %}}
but the scope of machine learning and IoT is incomprehensible to ordinary users. when you can determine through a ML model of someone's purchases not just that they are pregnant but that they're in the 3rd trimester, this isn't a piece of data that the consumer willingly and knowingly shared with you. creating informed and meaningful consent is all but impossible
{{% /note %}}

---

![in_X_lines](img/in_X_lines_01.png)
{{% fragment %}}![in_X_lines](img/in_X_lines_02.png){{% /fragment %}}
{{% fragment %}}![in_X_lines](img/in_X_lines_03.png){{% /fragment %}}
{{% fragment %}}![in_X_lines](img/in_X_lines_04.png){{% /fragment %}}
{{% fragment %}}![in_X_lines](img/in_X_lines_05.png){{% /fragment %}}
{{% fragment %}}![in_X_lines](img/in_X_lines_06.png){{% /fragment %}}
{{% fragment %}}![in_X_lines](img/in_X_lines_07.png){{% /fragment %}}

{{% note %}}
what also makes ML and IoT especially problematic is that their inherent complexity is not being respected, only their results. amateurish engineering: "easy machine learning in 100 lines of Python!". maybe ML tools are reasonably well-understood by the elite developers of the best organizations, but *many* users of ML treat the tools as magic and the models as binary blobs: a black box into which numbers go and decisions come out.
{{% /note %}}

---

![ugly-t-shirt](img/ugly-t-shirt.jpg)

*[Robison Meyer, The Atlantic, 3 Oct 2013](https://www.theatlantic.com/technology/archive/2013/10/avoid-facial-detection-algorithms-with-a-t-shirt/280253/)*


{{% note %}}
because ML is poorly understood, attacks on it can have open-ended results. maybe today someone is using a William Gibson's Ugly T-Shirt to protect their identity from ubiquitous law enforcement use of facial recognition...
{{% /note %}}

---

![face-recognition-glasses](img/face-recognition-glasses.png)

*[James Vincent, The Verge, 3 Nov 2016](https://www.theverge.com/2016/11/3/13507542/facial-recognition-glasses-trick-impersonate-fool)*

{{% note %}}
... but it doesn't take much imagination to see someone using this same system to "SWAT" unsuspecting targets
{{% /note %}}

---

![adversarial-toaster](img/adversarial-toaster.png)

*[James Vincent, The Verge, 3 Jan 2018](https://www.theverge.com/2018/1/3/16844842/ai-computer-vision-trick-adversarial-patches-google)*

{{% note %}}
what happens when a banana looks, not like a toaster, but a bomb or weapon? when an "accident" of that kind occurs, do the engineers of the system bear responsibility for failing to protect against this kind of "side channel" attack?
{{% /note %}}

---

![road-signs](img/road-signs.png)

*[Kimberly Mok, The New Stack, 14 Sep 2017](https://thenewstack.io/camouflaged-graffiti-road-signs-can-fool-machine-learning-models/)*

{{% note %}}
the flaws of self-driving vehicles and the organizations operating them seem terrifying enough without adding adversarial environments into the mix
{{% /note %}}

---

> The team found that with this approach, they were able to confuse a machine 100 percent of the time into classifying a stop sign as a 45-mile-per-hour speed limit sign, and a right-turn sign as a stop sign.

*[Kimberly Mok, The New Stack, 14 Sep 2017](https://thenewstack.io/camouflaged-graffiti-road-signs-can-fool-machine-learning-models/)*

{{% note %}}
unremarkable graffiti was used to confuse a ML algorithm *100%* of the time
{{% /note %}}

---

## embedded industry stuck in archaic threat model

{{% note %}}
if you thought the enterprise was bad: they're still shipping devices with shared private keys and hard-coded passwords. we used to say things like "well if you have physical possession then it's game over" but that's *always* the case with IoT devices. But we have answer to that: "secure boot" using TPM to sign the bootloader and OS updates (without which any device can be rooted). But this is treated as an expensive add-on rather than the default
{{% /note %}}

---

![hawkbit](img/hawkbit-logo.png)

*http://www.eclipse.org/hawkbit/*

{{% note %}}
existing solutions for IoT Over-the-Air updates (OTA) are mostly research projects at best (ex. Hawkbit, which depending on how you look at it is either an insecure-by-default toy, or an overcomplicated kit-of-parts)...
{{% /note %}}

---

![aws-iot](img/aws-iot.png)

*[Robert McCauley, Alexa Blogs, 3 May 2016](https://developer.amazon.com/de/blogs/post/Tx3828JHC7O9GZ9/Using-Alexa-Skills-Kit-and-AWS-IoT-to-Voice-Control-Connected-Devices)*

{{% note %}}
... or require trust delegation to third parties like AWS IoT that throw-away the guarantees about provenance that put secure boot at risk
{{% /note %}}


---

## Our abdication of responsibility invites political remedy

{{% note %}}
the problem with our complacency on this as an industry is that it invites someone to "do something" about it.
{{% /note %}}

---

![congress](img/congress.jpg)

*https://www.brookings.edu/wp-content/uploads/2016/06/congress006-1.jpg*

{{% note %}}
when these geniuses decide to act, the legal remedy is likely to be ham-fisted
{{% /note %}}

---

## "We have to do something!"
## "This is something"
## "We must do it!"

{{% note %}}
we've seen this over and over again. look at the evergreen fights over encryption, where the government thinks they can somehow make math available only to Good People
{{% /note %}}

---

![series-of-tubes](img/series-of-tubes.png)

*https://imgur.com/gallery/2mIObIu*

{{% note %}}
This is particularly a problem here in the US where virtually all our lawmakers are incompetent...
{{% /note %}}

---

![ajit-pai](img/ajit-pai.png)

*[Terrence O'Brien, engadget, 18 May 2017](https://www.engadget.com/2017/05/18/fcc-chairman-net-neutrality-1996/)*

{{% note %}}
... or they (and their minions) are entirely co-opted by hostile interests
{{% /note %}}

---

> Disclaimer of Warranty. Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.

*https://www.apache.org/licenses/LICENSE-2.0*

{{% note %}}
today much of our work is protected by saying "hey we don't warranty this for fitness for any particular use." this is the Apache license but other OSS licenses are similar, as are most EULAs. we've been allowed to get away with this, but that could change.
{{% /note %}}

---

## Do you want to be personally liable for bugs in your code?

{{% note %}}
everyone here want to carry malpractice insurance?
{{% /note %}}

---

![gdpr-block](img/gdpr-block.png)

*https://apility.io/2018/05/25/gdpr-lazy-block-european-users-cloudflare-workers/*

{{% note %}}
but even in the face of reasonable privacy law like the GDPR, we've seen our industry act with utter lack of professionalism. After 2 *years* notice, this "I'm taking my ball home" is the best that orgs can do?
{{% /note %}}

---

![gdpr-hackernews](img/gdpr-hackernews.png)

*https://news.ycombinator.com/item?id=16954306*

{{% note %}}
top post on The Orange Site: "what many posters here miss is that a big group of tech people have no interest in dealing with legal matters." aw, poor baby! you don't get to be part of a world-impacting profession and pretend there are no real world consequences. childishness!
{{% /note %}}

---

![gdpr-internet-of-shit](img/gdpr-internet-of-shit.png)

*https://twitter.com/internetofshit/status/999619364541394944*

{{% note %}}
on the other hand, if this is what organizations are doing...
{{% /note %}}

---

![gdpr-unrollme](img/gdpr-unrollme.png)

*[Natasha Lomas, Tech Crunch, 5 May 2018](https://techcrunch.com/2018/05/05/unroll-me-to-close-to-eu-users-saying-it-cant-comply-with-gdpr/)*

{{% note %}}
...then maybe it's all working as intended!
{{% /note %}}

---

# feature, not bug

{{% note %}}
if you can't do your job to protect the privacy of users and have to close up shop: Mission. Accomplished.
{{% /note %}}

---

> Salesforce CEO Marc Benioff thinks America needs "a national privacy law... that probably looks a lot like GDPR.

> "This is going to help our industry... It's going to set the guardrails around trust, around safety. It's going to provide the ability for the customers to interact with great next generation technologies in a safe way."

*[Simon Sharwood, The Register, 30 May 2018](https://www.theregister.co.uk/2018/05/30/salesforce_q1_2019/?)*

{{% note %}}
But it doesn't have to be that way. In this interview with Marc Benioff he points out this can be good for our industry. It'll "set the guardrails"
{{% /note %}}

---

> Benioff went on to say that as artificial intelligence is used in customer service, "that starts to cross the line on what is trust. And that's where our industry really has to come forward and say we're going to make sure that these technologies are trust-based. And I think the Europeans definitely got that figured out."

*[Simon Sharwood, The Register, 30 May 2018](https://www.theregister.co.uk/2018/05/30/salesforce_q1_2019/?)*

{{% note %}}
And this is deeply important because we as an industry have failed to set those guardrails for ourselves. And the larger society (our users) are starting to see this. It's not too late. What can we do?
{{% /note %}}

---

# Consent

{{% note %}}
[10:00]
consent is the *only* workable guiding model when we're talking about relationships between individual people. I consent to being in a relationship with you. You consent to being in a relationship with me. When you decide you don't want to be in that relationship you can withdraw consent and I'm supposed to respect that. We *hopefully* all understand this by now?
{{% /note %}}

---

# Individual vs Community Consent

{{% note %}}
But consent has some limits once we get a lot more people involved. Although individual consent is the basis of liberal democracy, there are some times when we decide that the will of the community overrides the consent of an individual.
{{% /note %}}

---

![vaccines](img/vaccines.jpg)

*[Steve Sack, Star Tribune, 27 Jan 2015](http://www.startribune.com/sack-cartoon-vaccinations/289998831/)*

{{% note %}}
We expect everyone to pay their taxes. We ask that people are vaccinated. And the boundaries of individual vs community consent vary by culture. ex. in the EU they protect individual consent strongly...
{{% /note %}}

---

![kelo-house](img/kelo-vs-new-london.png)

*[Ilya Somin, Washington Post, 29 May 2015](https://www.washingtonpost.com/news/volokh-conspiracy/wp/2015/05/29/the-story-behind-the-kelo-case-how-an-obscure-takings-case-came-to-shock-the-conscience-of-the-nation/)*

{{% note %}}
whereas in the US we have a mixed bag where businesses (which are supposed to be individuals) are often given the power of the community to override individual consent, but very little of the responsibility of consent.
{{% /note %}}

---

![gdpr-tumblr](img/tumblr-gdpr.png)

*https://twitter.com/Millstab/status/999762424994594817*

{{% note %}}
this is the flaw of the consent model as a solution. we saw that side-channel information leaks make consent nearly impossible to understand. and dark UX patterns can manipulate consent. "you agreed to this!"
{{% /note %}}

---

![externality](img/externality-definition.png)

*https://www.google.com/search?q=externality*

{{% note %}}
we see failure of consent at play when we look at the Uber accident. the woman who was killed didn't consent to be part of Uber's experimental driving program. she wasn't behind the wheel. what does "consent" mean when other human lives are treated as an externality? aside: are these results being manipulated? the *canonical* example is pollution! what coal industry PR team infiltrated this into Google's results?
{{% /note %}}

---

# values vary

{{% note %}}
ethical definitions vary b/c values vary (ex. that balance of community vs individual consent varies significantly between Europe and the US). but we're not the first people to have this problem! so how do other professions solve this problem...?
{{% /note %}}

---

![sonia-1](img/sonia-1.png)

*https://twitter.com/soniagupta504/status/1011591288003575808*

{{% note %}}
Sonia (who was up here on stage last night): "Lawyers and doctors enter their professions knowing, from the outset, just how heavy their burdens are. They hold human rights and life in their hands."
{{% /note %}}

---

![sonia-2](img/sonia-2.png)

*https://twitter.com/soniagupta504/status/1011591288003575808*

{{% note %}}
highly impactful professions know that their limits must be more stringent
{{% /note %}}

---

## "With great power comes great responsibility"

{{% note %}}
or as all the comic book nerds in the room know it: "with great power comes great responsibility"
{{% /note %}}

---

# professional ethics

{{% note %}}
this is the basis of professional ethics
{{% /note %}}

---

# licensing as
# self-regulation

{{% note %}}
historically licensing and professional organizations (ex. AMA, AIA, ASME, bar associations) have arisen from the professions themselves rather than being imposed clumsily from the outside. government licensing requirements are typically delegated to the professional organizations
{{% /note %}}

---

# licensing requires monopoly

{{% note %}}
professional certification w/o the consequences of regulation is basically toothless. we see lots and lots of useless rent-seeking certifications today already (CompTIA, Project Management Institute). it's worth considering what the side-effects of regulation-supported monopoly would be.
{{% /note %}}

---

> We do not believe that it is merely a coincidence that the entry and standards of practice are most strictly regulated for physicians, dentists, and veterinarians... where the costs of receiving poor services could be high or sometimes even catastrophic.

*[ref http://www.nber.org/papers/w10467.pdf](http://www.nber.org/papers/w10467.pdf)*

{{% note %}}
study by Marc Law & Sukkoo Kim of National Bureau of Economic Research shows that professional organizations have acted mostly as a counter to information asymmetry rather than creating monopoly power. consumers of our services generally don't understand what they're buying, and so professional bodies provide an answer to the question of whether the product is acceptable. professional organizations ethical requirements are typically about fair dealing and bare minimum safety guidelines.
{{% /note %}}

---

# gatekeeping

{{% note %}}
... so in other words they serve as gatekeepers. well, that's a little problematic isn't it? we have enough barriers to entry in our profession as it is. we still have a *lot* of work to do, but this profession is one that can help bootstrap people firmly into the middle-class. so adding new barriers like "you must have *this* degree" or "you must have this many years experience working under a licensed developer" seem like they'd work against the direction we want to take our industry, right?
{{% /note %}}

---

# shared ethical baseline

{{% note %}}
but an advantage of a professional organization's ethical framework is that it at least gives a shared baseline: right now we're all trying to figure this out for ourselves. and we should hold each other to task
{{% /note %}}

---

# what is to be done?

{{% note %}}
[20:00]
waiting for "the industry" to fix it isn't working. we all, individually, are the industry. need to take individual action:
- influence the community
- ex. talk about this stuff!
- ex. what organizations do we work for?
{{% /note %}}

---

![microsoft-employees-ice](img/microsoft-employees-ice.png)

*[Peter Bright, Ars Technica, 20 Jun 2018](https://arstechnica.com/tech-policy/2018/06/microsoft-staff-call-on-company-to-end-ice-contract/)*

{{% note %}}
we can influence the organization. we see Microsoft employees pushing for change in what customers their organization serves
{{% /note %}}

---

![google-employees-military](img/google-employees-military.png)

*[Paresh Dave and Heather Somerville, Reuters, 1 Jun 2018](https://www.reuters.com/article/uk-alphabet-defense/google-to-scrub-u-s-military-deal-protested-by-employees-source-idUKKCN1IX5YC)*

{{% note %}}
we've seen successful protest by Googlers motivated by their conscience
{{% /note %}}

---

![amazon-employees-law-enforcement](img/amazon-employees-law-enforcement.png)

*[Kate Conger, Gizmodo, 21 Jun 2018](https://gizmodo.com/amazon-workers-demand-jeff-bezos-cancel-face-recognitio-1827037509)*

{{% note %}}
and we've seen Amazon employees pushing for change
{{% /note %}}

---

# what about...?

{{% note %}}
"whataboutism": because "values vary" it isn't constructive to see e.g. Microsoftees protesting ICE but then turn around and say "what about their military contracts?" or "what about that time when MSFT's CEO from 17 years ago said meanie-head things about open source?" This is not helpful.
{{% /note %}}

---

# Who's hiring?

{{% note %}}
the labor market for our profession gives us enormous power right now. we can push hard for better hiring policies. we can push hard for D&I efforts. we can push hard for our organizations to be better
{{% /note %}}

---

# ensure your own mask is secure

{{% note %}}
that being said, we should also cut each other some slack. you don't know much about the circumstances of any particular person. so while we should be holding each other to task, individuals need to make their own decisions about where they work and that doesn't make them The Enemy. (unless they work at Palantir, just sayin')
{{% /note %}}

---

# direct action

{{% note %}}
what is available to everyone regardless of our work conditions, and perhaps more effective than anything else we can do, is direct action at an engineering level. what choices do we make as technologists?
{{% /note %}}

---

## Immutable?

![kafka](img/Kafka.png)

[Jay Kreps, Cloudera, 11 June 2015](https://vision.cloudera.com/apache-kafka-a-platform-for-real-time-data-streams-part-1/)

{{% note %}}
the pipelines we use to ingest data in many orgs are using immutable event stores. this means that once data is written it's never really erased. if you're keeping the entire commit history then you're going to have a lot of problems with GDPR. (did you remember your backups?)
{{% /note %}}

---

## "Immutable"

![kafka](img/Kafka-per-user.png)

{{% note %}}
but with changes at the application level, we can make this work. for example, we can use per-user encryption keys for a stream. this way we have encryption at rest, which is great, but we've also made our immutable event infrastructure compatible with the "right to be forgotten": you delete the per-user key from the key store and the data is forever unreadable.
{{% /note %}}

---

```python
def should_brake(road):
    if road.contains(object.HUMAN):
        print("oh shit!")
        # TODO: this is causing erratic driving on false
        # positive detection. Uncomment this once we have
        # that solved. Someone should remind the field
        # engineers to tell the test drivers they need to
        # pay attention to the road.
        # return True
    return False
```

{{% note %}}
we need to take responsibility for quality proportional to the risks involved with the software. certainly this is obvious in directly-life-impacting software like self-driving cars. we need to be part of the chain of safety around these systems.
{{% /note %}}

---

# secure boot

{{% note %}}
we need to take responsibility for having deep understanding of how the security of our systems are bootstrapped. and we need to make decisions about that aligned with our values.
{{% /note %}}

---

![secure-boot](img/secureboot.jpg)

*https://www.iconlabs.com/prod/products/device-protection/floodgate-secure-boot*

{{% note %}}
in the case of IoT one of the options is secure boot.  you'll provide the factory where the product is assembled with the public keys you want to have loaded into your chip's trusted platform module. This makes it so that only *your* signed bootloader and OS can be loaded onto the device

{{% /note %}}

---

![Hashicorp Vault logo](img/vault.png)

{{% note %}}
this means ensuring that your organization has PKI infrastructure in place to sign the bootloader and OS. get familiar with secret stores like Hashicorp Vault to build the foundation of this infrastructure
{{% /note %}}

---

![john_deere](img/john_deere.png)

*[Jason Koebler, Motherboard, 21 Mar 2017](https://motherboard.vice.com/en_us/article/xykkkd/why-american-farmers-are-hacking-their-tractors-with-ukrainian-firmware)*

{{% note %}}
but there's a tradeoff here. if you have secure boot that means your users will find it that much more difficult (if not impossible) to modify and repair the device firmware. this is a business decision and a decision about values; not making a decision one way or another means abdicating your responsibility as an engineer
{{% /note %}}

---

# secure communication

{{% note %}}
when we deploy IoT devices we need to ensure we're taking advantage of modern TLS options. you wouldn't transmit the login form for your web application over plain text, right? (right?!)
{{% /note %}}

---

![cloudflare-blog-tls-1.3](img/cloudflare_tls_1-3.png)

{{% note %}}
IoT devices typically have limited compute power, so folks avoid encryption. but we can solve this with modern choices: TLS1.3 reduces round-trips and elliptic curve keys use less memory than RSA keys. likewise, although you can cram MQTT into TLS, modern protocols like CoAP include mutually authenticated TLS.
{{% /note %}}

---

# ML models

{{% note %}}
what about our engineering decisions in ML?
{{% /note %}}

---

![neural-net](img/neural_network.png)

https://commons.wikimedia.org/wiki/File:Neural_network_bottleneck_achitecture.svg

{{% note %}}
let's look at one ML process called Convolutional Neural Net. each of the nodes in this diagram is just a function that takes a vector (an array) and runs a filter function over it (typically the filter itself will take a subset of the vector at a time).
{{% /note %}}

---

![iris-dataset-scatterplot](img/iris_dataset.png)

https://commons.wikimedia.org/wiki/File:Iris_dataset_scatterplot.svg

{{% note %}}
iterating on the weights of those inputs allows us to extract "features" from the training inputs that result in "interesting" classifications (decisions).
{{% /note %}}

---

![deep-neural-net](img/deep_neural_network.png)

https://cdn.edureka.co/blog/wp-content/uploads/2017/05/Deep-Neural-Network-What-is-Deep-Learning-Edureka.png

{{% note %}}
each layer builds on the layers that came before it. but these classifications are just regions in mathematical space here
{{% /note %}}

---

```python
def save(model, filename):
    pickle.dump(model, open(filename, 'wb'))
```

{{% note %}}
and then when we're done training, we take the result of all those weights and call it our model and just serialize the whole damn thing and ship it to prod. we can pass real world data in through the same model and out comes the classifications.
{{% /note %}}

---

# ML models are state

{{% note %}}
our entire industry has unified around our worries about statefulness. "run your applications as stateless containers! with k8s! let your cloud provider lock-in -- I mean securely host -- all your stateful applications!" But ML is the ultimate stateful application. you're using software to generate these software models and you ship those models. let's get the Functional Programming crowd in a twist: the entire application is a side-effect! how can we influence those side-effects?
{{% /note %}}

---

![machine-learning-tech-debt](img/machine-learning-tech-debt.png)

*https://ai.google/research/pubs/pub43146*

{{% note %}}
we desperately need better tooling to design-out unexpected behaviors in ML. We have undeclared consumers, hidden "strange loops" of feedback, and entangled data dependencies. These represent a source of technical debt. and it's the worst kind of technical debt -- it's what John Allspaw and the SNAFUcatchers call "shadow debt" that's taken on unknowingly.
{{% /note %}}

---

> To make great products:

> do machine learning like the great engineer you are, not like the great machine learning expert you aren't.

> ...

> Insofar as well-being and company health is concerned, human judgement is required to connect any machine learned objective to the nature of the product you are selling and your business plan.

*[Martin Zinkevich (Google), Rules of Machine Learning: Best Practices for ML Engineering](https://developers.google.com/machine-learning/rules-of-ml/)*

{{% note %}}
we need to remember with any ML project that human judgement is required to connect the learned objectives to their impact with the real world -- our business, our industry, and the community as a whole
{{% /note %}}

---

# SQL > ML

{{% note %}}
first rule should always be: why are we choosing ML over some well-tuned SQL or other algorithm? why are we choosing to use a method with chaotic feedback mechanisms instead of something that's simple and deterministic? is this simply because of resume-driven development?
{{% /note %}}

---

## models should be testable and human-interpretable

{{% note %}}
when we do choose ML, we should choose our approach carefully. simple linear or logarithmic regression models are easier to debug, calibrate, and avoid unexpected feedback loops than models that try to optimize their own accuracy. remove unused features (which represent both technical debt and side-channel opportunities), and quantify any observed undesirable behavior and build tests for it. these pieces of technical debt all represent avenues for adversarial input
{{% /note %}}

---

# align training data with real world demographics

{{% note %}}
choose ML training inputs that reflect the population. this is a fortunate case where we can easily align engineering ethics with business needs (ex. "if we pick machine vision training data that reflects real demographics, we can avoid the embarrassment for our organization of having to explain why our software acts racist.") win-win, eh?
{{% /note %}}

---

# technical leadership

{{% note %}}
we can't rely on project managers or business analysts to take the lead on designing our systems ethically because they simply may not understand the side-effects. you're the technical professional: they're expecting you to take the lead on this!
{{% /note %}}

---

# "best practice is..."

{{% note %}}
"the best thing about best practices is there are so many of them to choose from." you don't need to ask permission from your business analysts and project managers on opinions that are purely technical
{{% /note %}}

---

![jira-clock-puncher](img/jira-clock-puncher.png)
{{% fragment %}}![jira-clock-puncher](img/jira-clock-puncher.png){{% /fragment %}}
{{% fragment %}}![jira-clock-puncher](img/jira-clock-puncher.png){{% /fragment %}}
{{% fragment %}}![jira-clock-puncher](img/jira-clock-puncher.png){{% /fragment %}}
{{% fragment %}}![jira-clock-puncher](img/jira-clock-puncher.png){{% /fragment %}}
{{% fragment %}}![jira-clock-puncher](img/jira-clock-puncher.png){{% /fragment %}}
{{% fragment %}}![jira-clock-puncher](img/jira-clock-puncher.png){{% /fragment %}}
{{% fragment %}}![jira-clock-puncher](img/jira-clock-puncher.png){{% /fragment %}}
{{% fragment %}}![jira-clock-puncher](img/jira-clock-puncher.png){{% /fragment %}}
{{% fragment %}}![jira-clock-puncher](img/jira-clock-puncher.png){{% /fragment %}}
{{% fragment %}}![jira-clock-puncher](img/jira-clock-puncher.png){{% /fragment %}}
{{% fragment %}}![jira-clock-puncher](img/jira-clock-puncher.png){{% /fragment %}}
{{% fragment %}}![jira-clock-puncher](img/jira-clock-puncher.png){{% /fragment %}}
{{% fragment %}}![jira-clock-puncher](img/jira-clock-puncher.png){{% /fragment %}}
{{% fragment %}}![jira-clock-puncher](img/jira-clock-puncher.png){{% /fragment %}}

{{% note %}}
formal Agile methodologies contribute to the problem. "act ethically" doesn't have any story points in this epic. But you're supposed to be a professional, not a JIRA clock puncher. act like it!
{{% /note %}}

---

> We aren't a craft anymore. We might feel like artisans with laptops but what we produce could potentially be in front of a significant chunk of the human race by lunchtime. We're not hand-crafting dovetail joints here.

*[Anne Currie, The Register, 1 Mar 2018](https://www.theregister.co.uk/2018/03/01/ethics_yeah_thats_great_but_do_they_scale/)*

{{% note %}}
leave you with...
{{% /note %}}

---

# let's get to work
