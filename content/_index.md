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
I'm Tim Gross. This is my twitter handle, which seemed like a good idea at the time. "They Didn't Stop to Think If They Should"
{{% /note %}}

---

## or...
## Machine Learning And The Internet Of Unpatched Things

{{% note %}}
an alternate title could be... "Machine Learning And The Internet Of Unpatched Things"
{{% /note %}}

---

## or...
## Because Eternal Vigilance is the Price of Liberty, We Have to Talk About Ethics Again

{{% note %}}
or maybe... "Because Eternal Vigilance is the Price of Liberty, We Have to Talk About Ethics Again"
{{% /note %}}

---

> We've updated our privacy policy!

> Any reference to or citation of any person or organization does not constitute or imply an endorsement or recommendation of the content of this talk. The opinions expressed in this talk are the speaker's alone and do not reflect the view of this conference, your employer, or my mom. The speaker is grossly unqualified to tell you how to live your life. Your mileage may vary. Not to be used in the manufacture of nuclear weapons. By attending this talk the speaker hereby grants you an irrevocable, perpetual, non-exclusive, transferable, worldwide license to be excellent to each other.

{{% note %}}
"Is this guy gonna talk about the trolley problem? C'mon, I just want to code! And who is this guy, anyways? He's not an ethicist with a PhD!" Why do we as engineers need to discuss this stuff? And why is it especially important to talk about ethics when we start talking about ML and IoT? What makes these things special? What makes them different from other software? the reason we *all* need to be talking about this, is because as Sharon Kennedy Vickers told us yesterday: "what we do has impact"
{{% /note %}}

---

![Washington Post: NTSB finds self-driving Uber did not have emergency braking turned on](img/uber-accident.png)

*[Michael Laris, Washington Post, 24 May 2018](https://www.washingtonpost.com/news/dr-gridlock/wp/2018/05/24/ntsb-self-driving-uber-did-not-have-emergency-braking-turned-on/)*


{{% note %}}
Back in March a self-driving car operated by Uber killed a pedestrian. The NTSB investigation is still ongoing, but what is clear is that the vehicle had no business being operated without direct supervision. The collision detection system had lots of false positives that caused it to brake erratically. So they turned the braking system off. But apparently that message never got to the folks who'd turned off the vehicles' own automatic braking nor to the attendee of the vehicle. So the vehicle "saw" the pedestrian and did nothing.
{{% /note %}}

---

![The Verge: Twitter taught Microsoft's Tay Chatbot to be a racist asshole in less than a day](img/microsoft-chatbot.png)

*[James Vincent, The Verge, 24 Mar 2016](https://www.theverge.com/2016/3/24/11297050/tay-microsoft-chatbot-racist)*

{{% note %}}
A couple years ago, MSFT demonstrated their ML capabilities with the Tay chatbot. They let it loose to learn from whatever racist trolls wanted to teach it. The experiment was stopped and the whole debacle embarrassed MSFT. Now clearly the horrible Internet people are primarily to blame here, but the researchers failed to anticipate the vulnerabilities inherent to their system
{{% /note %}}

---

![The Verge: UK hospitals hit with massive ransomware attack](img/uk-ransomware.png)

*[Russell Brandom, The Verge, 12 May 2017](https://www.theverge.com/2017/5/12/15630354/nhs-hospitals-ransomware-hack-wannacry-bitcoin)*

{{% note %}}
in an IoT example, last year countless devices in UK hospitals were taken over by Wannacry ransomware. patient lives were put at risk not just because of poor patch hygiene but because of the architectural flaws and because of warped incentives in the US government program that produced the malware in the first place.
{{% /note %}}

---

![The Guardian: Tesla car that crashed and killed driver was running on Autopilot, firm says](img/tesla-autopilot.png)

*[The Guardian, 31 Mar 2018](https://www.theguardian.com/technology/2018/mar/31/tesla-car-crash-autopilot-mountain-view)*

{{% note %}}
Tesla's autopilot has been implicated in the deaths of several drivers at this point. We (and Tesla stockholders, apparently) are constantly reassured that these are the result of improper handling and not rushing these systems into the real world before they're ready.
{{% /note %}}

---

![Forbes: How Target Figured Out a Teen Girl Was Pregnant Before Her Father Did](img/target-pregnant.png)

*[Kashmir Hill, Forbes, 16 Feb 2012](https://www.forbes.com/sites/kashmirhill/2012/02/16/how-target-figured-out-a-teen-girl-was-pregnant-before-her-father-did/)*

{{% note %}}
You didn't think I was going to leave the home team out? Machine learning algorithms may know more about us and our loved ones than we do ourselves. Target was able to determine from customer purchases not just when customers are pregnant but at what stage of their pregnancy they were (buying unscented products during late stages, for example).
{{% /note %}}

---

![The Guardian: Google says sorry for racist auto-tag in photo app](img/google-racist-autotag.png)

*[Jana Kasperkevic, The Guardian, 1 Jul 2015](https://www.theguardian.com/technology/2015/jul/01/google-sorry-racist-auto-tag-photo-app)*

{{% note %}}
ML is encoding our biases. Not just dehumanizing people online, but we saw yesterday how it can reinforce structures of power and privilege: access to mortgages, sentencing guidelines
{{% /note %}}

---
![@yipe on Twitter: "Alexa: remind me to feed the baby" (response: "Defeat the baby")](img/defeat-the-baby.png)

*https://twitter.com/yipe/status/1005555741153902592*

{{% note %}}
we've invited these systems into our homes... (and ok, yeah this is funny)
{{% /note %}}

---

![Huffington Post: Amazon Alexa-Powered Device Recorded and Shared User's Conversation Without Permission](img/alexa-eavesdropping.png)

*[Laura Stevens, Huffington Post, 24 May 2018](https://www.huffingtonpost.com/entry/alexa-eavesdropping-portland-familiy_us_5b0727cae4b0fdb2aa51b23e)*

{{% note %}}
... with almost no oversight into what they're doing. We have unaccountable closed source microphones in our homes, who do who-knows-what with that information
{{% /note %}}

---

![@polotek on Twitter: "Kalanick keeps asking for unethical/illegal things, but at some point we have to talk about how engineers at Uber keep saying yes."](img/marco-rogers.png)

{{% note %}}
what all these stories have in common is that like any other failure there's almost certainly no "root cause". these failures are the result of complex sociotechnical systems and the incentives they set up. it's unlikely that anyone at these companies set out with awful intentions. But as Lanice Sims told us yesterday, your intentions ain't shit. at the end of the day, it's people in our industry -- the people in this room -- who are the ones who execute and implement these systems
{{% /note %}}

---

# a problem of scale

{{% note %}}
the problem isn't just that these systems all have real-world consequences; software always has. we can go back to the 80's and look at the Therac-25 accidents, where software flaws in radiation machines killed 3 people. the problem is that those consequences are multiplied by the scale of these systems.
{{% /note %}}

---

## quantity has its own quality

{{% note %}}
a huge part of the value proposition of IoT and ML is the scale of the data involved: collecting massive amounts of data from edge computing devices, and processing massive amounts of data in ML models.
{{% /note %}}

---

## no meaningfully informed consent

{{% note %}}
but the scope of machine learning and IoT is incomprehensible to ordinary users. if you can determine through a ML model of someone's purchases not just that they are pregnant but that they're in the 3rd trimester, this isn't a piece of data that the consumer willingly and knowingly shared with you, or have any way of knowing you could get. creating informed and meaningful consent is all but impossible
{{% /note %}}

---

!["in X lines of Python"](img/in_X_lines_01.png)
{{% fragment %}}!["in X lines of Python"](img/in_X_lines_02.png){{% /fragment %}}
{{% fragment %}}!["in X lines of Python"](img/in_X_lines_03.png){{% /fragment %}}
{{% fragment %}}!["in X lines of Python"](img/in_X_lines_04.png){{% /fragment %}}
{{% fragment %}}!["in X lines of Python"](img/in_X_lines_05.png){{% /fragment %}}
{{% fragment %}}!["in X lines of Python"](img/in_X_lines_06.png){{% /fragment %}}
{{% fragment %}}!["in X lines of Python"](img/in_X_lines_07.png){{% /fragment %}}

{{% note %}}
what also makes ML especially problematic is that its inherent complexity is not being respected, only its results. "easy machine learning in 100 lines of Python!". *many* users of ML treat the tools as magic and the models as binary blobs: a black box into which numbers go and decisions come out.
{{% /note %}}

---

![picture of a ugly t-shirt that fools facial recognition](img/ugly-t-shirt.jpg)

*[Robison Meyer, The Atlantic, 3 Oct 2013](https://www.theatlantic.com/technology/archive/2013/10/avoid-facial-detection-algorithms-with-a-t-shirt/280253/)*


{{% note %}}
because ML's chaotic behavior is poorly understood, attacks on it can have open-ended results. maybe today someone is using a William Gibson's Ugly T-Shirt to protect their identity from ubiquitous law enforcement use of facial recognition...
{{% /note %}}

---

![Verge: These glasses trick facial recognition software into thinking you're someone else](img/face-recognition-glasses.png)

*[James Vincent, The Verge, 3 Nov 2016](https://www.theverge.com/2016/11/3/13507542/facial-recognition-glasses-trick-impersonate-fool)*

{{% note %}}
... but could I give you an innocuous object that makes that system see you as a wanted terrorist to "SWAT" unsuspecting targets?
{{% /note %}}

---

![picture of an adversarial sticker that fools machine vision into thinking any object is a toaster](img/adversarial-toaster.png)

*[James Vincent, The Verge, 3 Jan 2018](https://www.theverge.com/2018/1/3/16844842/ai-computer-vision-trick-adversarial-patches-google)*

{{% note %}}
what happens when a banana looks, not like a toaster, but a bomb or weapon? when an "accident" of that kind occurs, do the engineers of the system bear responsibility for failing to protect against this kind of "side channel" attack?
{{% /note %}}

---

![New Stack: Camouflaged Graffiti on Road Signs Can Fool Machine Learning Models](img/road-signs.png)

*[Kimberly Mok, The New Stack, 14 Sep 2017](https://thenewstack.io/camouflaged-graffiti-road-signs-can-fool-machine-learning-models/)*

{{% note %}}
the flaws of self-driving vehicles and the organizations operating them seem terrifying enough without adding adversarial environments into the mix. this is unremarkable graffiti...
{{% /note %}}

---

> The team found that with this approach, they were able to confuse a machine 100 percent of the time into classifying a stop sign as a 45-mile-per-hour speed limit sign, and a right-turn sign as a stop sign.

*[Kimberly Mok, The New Stack, 14 Sep 2017](https://thenewstack.io/camouflaged-graffiti-road-signs-can-fool-machine-learning-models/)*

{{% note %}}
but it was used to confuse a machine vision algorithm *100%* of the time. these attacks are unreasonably effective!
{{% /note %}}

---

## embedded industry stuck in archaic threat model

{{% note %}}
embedded industry stuck in archaic threat model. they're still shipping devices with shared private keys and hard-coded passwords. we used to say things like "well if you have physical possession then it's game over" but that's *always* the case with IoT devices. But we have answer to that: "secure boot" using TPM to sign the bootloader and OS updates. But this is treated as an expensive add-on rather than the default
{{% /note %}}

---

![Hawkbit logo](img/hawkbit-logo.png)

*http://www.eclipse.org/hawkbit/*

{{% note %}}
existing solutions for IoT Over-the-Air updates (OTA) are mostly research projects at best (ex. Hawkbit, which depending on how you look at it is either an insecure-by-default toy, or an overcomplicated kit-of-parts)...
{{% /note %}}

---

![diagram of AWS IoT products](img/aws-iot.png)

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

![stock image photo of US Congress](img/congress.jpg)

*https://www.brookings.edu/wp-content/uploads/2016/06/congress006-1.jpg*

{{% note %}}
like these geniuses. and when they decide to act, the legal remedy is likely to be ham-fisted
{{% /note %}}

---

## "We have to do something!"
## "This is something"
## "We must do this!"

{{% note %}}
we've seen this over and over again. look at the evergreen fights over encryption, where the government thinks they can somehow make math available only to "Good People"
{{% /note %}}

---

![caption of Senator Ted Stevens "series of tubes" remarks](img/series-of-tubes.png)

*https://imgur.com/gallery/2mIObIu*

{{% note %}}
This is particularly a problem here in the US where virtually *all* our lawmakers at the federal level are either incompetent...
{{% /note %}}

---

![intentionally unflattering picture of FCC Chairman Ajit Pai](img/ajit-pai.png)

*[Terrence O'Brien, engadget, 18 May 2017](https://www.engadget.com/2017/05/18/fcc-chairman-net-neutrality-1996/)*

{{% note %}}
... or they (and their minions) are entirely co-opted by interests that are hostile to the greater public
{{% /note %}}

---

> Disclaimer of Warranty. Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.

*https://www.apache.org/licenses/LICENSE-2.0*

{{% note %}}
today much of our work is protected by saying "hey we don't warranty this for fitness for any particular use." (this is the Apache license but other OSS licenses are similar, as are most EULAs.) these agreements aren't magic talismans; we've been *allowed* to get away with this, but that could change.
{{% /note %}}

---

## Do you want to be personally liable for bugs in your code?

{{% note %}}
anyone here want to carry malpractice insurance?
{{% /note %}}

---

![Apibility: GDPR for lazy people: block all European users with Cloudflare workers](img/gdpr-block.png)

*https://apility.io/2018/05/25/gdpr-lazy-block-european-users-cloudflare-workers/*

{{% note %}}
but even in the face of reasonable privacy law like the GDPR, we've seen our industry act with utter lack of professionalism. After 2 *years* notice, this "I'm taking my ball home" is the best that orgs can do?
{{% /note %}}

---

![screenshot of childish HackerNews comment](img/gdpr-hackernews.png)

*https://news.ycombinator.com/item?id=16954306*

{{% note %}}
top post on The Orange Site: "what many posters here miss is that a big group of tech people have no interest in dealing with legal matters." aw, poor baby! you don't get to be part of a world-impacting profession and pretend there are no real world consequences. childish!
{{% /note %}}

---

![@internetofshit on Twitter: "Hi just letting you know you can't use your lights anymore because we're slathering your data around and GDPR is here"](img/gdpr-internet-of-shit.png)

*https://twitter.com/internetofshit/status/999619364541394944*

{{% note %}}
on the other hand, if this is what organizations are doing...
{{% /note %}}

---

![TechCrunch: Unroll.me to close to EU users saying it can't comply with GDPR](img/gdpr-unrollme.png)

*[Natasha Lomas, Tech Crunch, 5 May 2018](https://techcrunch.com/2018/05/05/unroll-me-to-close-to-eu-users-saying-it-cant-comply-with-gdpr/)*

{{% note %}}
...then maybe it's all working as intended
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
It doesn't have to be that way. In this interview with Marc Benioff he points out this can be good for our industry. It'll "set the guardrails"
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
consent is the *only* workable guiding model when we're talking about relationships between individual people. ex. I consent to being part of your research. You consent to engaging in conversation with me. When you decide you don't want to be in a relationship you can withdraw consent and your partner respects that. We *hopefully* all understand this by now?
{{% /note %}}

---

# Individual Consent vs The Community

{{% note %}}
But consent has some limits once we get a lot more people involved. Although individual consent is the basis of liberal democracy, there are some times when we decide that the will of the community overrides the consent of an individual.
{{% /note %}}

---

![cartoon of anti-vaxxer releasing a monster](img/vaccines.jpg)

*[Steve Sack, Star Tribune, 27 Jan 2015](http://www.startribune.com/sack-cartoon-vaccinations/289998831/)*

{{% note %}}
We expect everyone to pay their taxes. We ask that people are vaccinated. And the boundaries of individual vs community consent vary by culture. ex. in the EU they protect individual consent strongly...
{{% /note %}}

---

![Washington Post: The story behind Kelo v City of New London](img/kelo-vs-new-london.png)

*[Ilya Somin, Washington Post, 29 May 2015](https://www.washingtonpost.com/news/volokh-conspiracy/wp/2015/05/29/the-story-behind-the-kelo-case-how-an-obscure-takings-case-came-to-shock-the-conscience-of-the-nation/)*

{{% note %}}
whereas in the US we have a mixed bag where businesses (which are supposed to be individuals) are often given the backing of the community to override individual consent, without all the responsibility of consent.
{{% /note %}}

---

![@Millstab on Twitter: "Some seriously unethical UX design from @tumblr - forcing anyone to untick 350+ boxes in order to prevent EACH INDIVIDUAL AD COMPANY from using our data. Taking the piss."](img/tumblr-gdpr.png)

*https://twitter.com/Millstab/status/999762424994594817*

{{% note %}}
we talked earlier about how unexpectedly-derived data makes consent nearly impossible to understand. dark UX patterns make this worse by manipulating consent. "you agreed to this!"
{{% /note %}}

---

![Google-supplied definition of externality](img/externality-definition.png)

*https://www.google.com/search?q=externality*

{{% note %}}
we see flaws of consent at play when we look at the Uber accident. the woman who was killed didn't consent to be part of Uber's experimental driving program. she wasn't behind the wheel. what does "consent" mean when other human lives are treated as an externality? aside: what coal industry PR team infiltrated this into Google's results?
{{% /note %}}

---

# foundational values?

{{% note %}}
the dynamic of community vs individual consent points to a problem defining foundational values (ref Bryan Cantrill's Monktober talk distinguishes between "principles" and "values"). if we can disagree on things like the balance of individual vs community (ex. EU vs US), how do we define shared values? we're not the first people to have this problem! so how do other professions solve this problem...?
{{% /note %}}

---

![@soniagupta504 on Twitter: "Lawyers and doctors enter their professions knowing, from the outset, just how heavy their burdens are. They hold human rights and life in their hands."](img/sonia-1.png)

*https://twitter.com/soniagupta504/status/1011591288003575808*

{{% note %}}
Sonia Gupta (who was up here on stage last night): "Lawyers and doctors enter their professions knowing, from the outset, just how heavy their burdens are. They hold human rights and life in their hands."
{{% /note %}}

---

![@soniagupta504 on Twitter: "highly impactful professions know that their limits must be more stringent"](img/sonia-2.png)

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
historically licensing and professional organizations (ex. AMA, AIA, ASME, bar associations) have arisen from the professions themselves rather than being imposed clumsily from the outside. they've asked for the protection of regulation. government licensing requirements are typically delegated to the professional organizations
{{% /note %}}

---

# licensing requires monopoly

{{% note %}}
certifications do exist. we see lots and lots of useless rent-seeking certifications today already (CompTIA, Project Management Institute). but professional certification w/o the consequences of regulation is basically toothless.  so before we get the government involved, it's worth considering what the side-effects of regulation-supported monopoly would be.
{{% /note %}}

---

> We do not believe that it is merely a coincidence that the entry and standards of practice are most strictly regulated for physicians, dentists, and veterinarians... where the costs of receiving poor services could be high or sometimes even catastrophic.

*[ref http://www.nber.org/papers/w10467.pdf](http://www.nber.org/papers/w10467.pdf)*

{{% note %}}
study from the National Bureau of Economic Research shows that professional organizations have acted mostly as a counter to information asymmetry rather than creating monopoly power. consumers of our services generally don't understand what they're buying, and so professional bodies provide an answer to those questions. I'm not a doctor but I rely on the boards to tell me my doctor has met minimum standards of fair dealing, competence, and safety
{{% /note %}}

---

# gatekeeping

{{% note %}}
... so in other words they serve as gatekeepers. well, that's a little problematic isn't it? we have enough barriers to entry in our profession as it is. we still have a *lot* of work to do. so adding new barriers like "you must have *this* degree" or "you must have this many years experience working under a licensed developer" seem like they'd work against the direction we want to take our industry, right?
{{% /note %}}

---

# shared ethical baseline

{{% note %}}
but an advantage of a professional organization's ethical framework is that it at least gives a shared baseline: right now we're all trying to figure this out for ourselves. and we should hold each other to task
{{% /note %}}

---

# what is to be done?

{{% note %}}
[15:00]
waiting for regulation seems like a bad idea. relying on consent hasn't really worked out. professional organizations seem fraught. but waiting for "the industry" to fix it isn't working. we all, individually, are the industry. need to take individual action.

---

![@containersoluti on Twitter: Very excited to announce that our conference on tech ethics @coedethics is sold out!](img/coed-ethics.png)

*https://twitter.com/containersoluti/status/1016624243868667904*

{{% note %}}
we can talk about this stuff. COED:Ethics in London happening today, sponsored by the great folks at ContainerSolutions like Anne Currie and Jamie Dobson
{{% /note %}}

---

![Tech Workers Coalition: Worker Power in the Tech Industry](img/techworkerscoalition.png)

*https://techworkerscoalition.org/*

{{% note %}}
we can influence the community. there are activist organizations that have sprung up in the last few years looking to push for broader change across many organizations, like the Tech Workers Coalition
{{% /note %}}

---

![arstechnica: Microsoft staff call on company to end ICE contract](img/microsoft-employees-ice.png)

*[Peter Bright, Ars Technica, 20 Jun 2018](https://arstechnica.com/tech-policy/2018/06/microsoft-staff-call-on-company-to-end-ice-contract/)*

{{% note %}}
we can influence our organizations. we see Microsoft employees pushing for change in what customers their organization serves
{{% /note %}}

---

![Reuters: Google to scrub US military deal protested by employees](img/google-employees-military.png)

*[Paresh Dave and Heather Somerville, Reuters, 1 Jun 2018](https://www.reuters.com/article/uk-alphabet-defense/google-to-scrub-u-s-military-deal-protested-by-employees-source-idUKKCN1IX5YC)*

{{% note %}}
we've seen successful protest by Googlers motivated by their conscience
{{% /note %}}

---

![Gizmodo: Amazon Workers Demand Jeff Bezos Cancel Face Recognition Contracts With Law Enforcement](img/amazon-employees-law-enforcement.png)

*[Kate Conger, Gizmodo, 21 Jun 2018](https://gizmodo.com/amazon-workers-demand-jeff-bezos-cancel-face-recognitio-1827037509)*

{{% note %}}
and we've seen Amazon employees pushing for change
{{% /note %}}

---

# what about...?

{{% note %}}
"whataboutism": because we have a restricted set of common values, it isn't constructive to see e.g. Microsoftees protesting ICE but then turn around and say "what about their military contracts?" or "what about that time when MSFT's CEO from 17 years ago said meanie-head things about open source?" This is not helpful. At least they're doing something instead of snarking about it on twitter
{{% /note %}}

---

# Who's hiring?

{{% note %}}
the labor market for our profession gives us enormous power right now. we can push hard for better hiring policies. we can push hard for D&I efforts. we can push hard for our organizations to be better
{{% /note %}}

---

# ensure your own mask is secure

{{% note %}}
that being said, we should also cut each other some slack. you don't know much about the circumstances of any particular person (do they have health problems? family to take care of?). so while we should be holding each other to task, individuals need to make their own decisions about where they work and that doesn't make them The Enemy. (unless they work at Palantir, just sayin')
{{% /note %}}

---

# direct action

{{% note %}}
what is available to everyone regardless of our work conditions, and perhaps more effective than anything else we can do, is direct action at an engineering level. what choices do we make as technologists?
{{% /note %}}

---

## Immutable?

![diagram of Apache Kafka commit log and typical consumers](img/Kafka.png)

[Jay Kreps, Cloudera, 11 June 2015](https://vision.cloudera.com/apache-kafka-a-platform-for-real-time-data-streams-part-1/)

{{% note %}}
the pipelines we use to ingest data in many orgs are using immutable event stores. this means that once data is written it's never really erased. if you're keeping the entire commit history then you're going to have a lot of problems with GDPR. (did you remember your backups?)
{{% /note %}}

---

## "Immutable"

![diagram of Apache Kafka commit log and typical consumers, with per-user encryption keys](img/Kafka-per-user.png)

{{% note %}}
but with changes at the application level, we can make this work. for example, we can use per-user encryption keys for a stream. this way we have encryption at rest, which is great, but we've also made our immutable event infrastructure compatible with the "right to be forgotten": you delete the per-user key from the key store and the data is forever unreadable.
{{% /note %}}

---

```python
def should_brake(road):
    if road.contains(object.HUMAN):
        log.warn("oh shit!")
        # TODO: this is causing erratic driving on false
        # positive detection. Uncomment this once we have
        # that solved. Someone should remind the field
        # engineers to tell the test drivers they need to
        # pay attention to the road.
        # return True
    return False
```

{{% note %}}
we need to take responsibility for quality proportional to the risks involved with the software. certainly this is obvious in directly-life-impacting software like self-driving cars, but it extends to every piece of software with real world impact. we need to be part of the chain of safety around these systems.
{{% /note %}}

---

# secure by design

{{% note %}}
we need to take responsibility for having deep understanding of how the security of our systems are bootstrapped. and we need to make decisions about that aligned with our values.
{{% /note %}}

---

![diagram showing secure boot stages](img/secureboot.jpg)

*https://www.iconlabs.com/prod/products/device-protection/floodgate-secure-boot*

{{% note %}}
in the case of IoT one of the options is secure boot.  you'll provide the factory where the product is assembled with the public keys you want to have loaded into your chip's trusted platform module. This makes it so that only *your* signed bootloader and OS can be loaded onto the device

{{% /note %}}

---

![Hashicorp Vault logo](img/vault.png)

{{% note %}}
this means ensuring that your organization has PKI infrastructure in place to sign the bootloader and OS. getting familiar with secret stores like Hashicorp Vault to build the foundation of this infrastructure is a good practice
{{% /note %}}

---

![Motherboard: Why American Farmers Are Hacking Their Tractors With Ukranian Firmware](img/john_deere.png)

*[Jason Koebler, Motherboard, 21 Mar 2017](https://motherboard.vice.com/en_us/article/xykkkd/why-american-farmers-are-hacking-their-tractors-with-ukrainian-firmware)*

{{% note %}}
but there's a tradeoff here. if you have secure boot that means your users will find it that much more difficult (if not impossible) to modify and repair the device firmware. this is a business decision *and* a decision about values; maybe the answer is different if the end user is a consumer vs a business? not making a decision one way or another means abdicating your responsibility as an engineer
{{% /note %}}

---

# secure communication

{{% note %}}
when we deploy IoT devices we need to ensure we're taking advantage of modern TLS options. you wouldn't transmit the login form for your web application over plain text, right? (right?!)
{{% /note %}}

---

![CloudFlare blog: TLS1.3 is going to save us all, and other reasons why IoT is still insecure](img/cloudflare_tls_1-3.png)

{{% note %}}
IoT devices typically have limited compute power, so folks avoid encryption. but we can solve this with modern choices: TLS1.3 reduces round-trips and elliptic curve keys use less memory than RSA keys. likewise, although you can cram MQTT into TLS, modern protocols like CoAP include mutually authenticated TLS. TLS isn't "end-user facing" in IoT (unlike a browser), but secure communication isn't about user optics but actually protecting the user.
{{% /note %}}

---

# ML models

{{% note %}}
what about our engineering decisions in ML?
{{% /note %}}

---

![diagram of a simple neural network](img/neural_network.png)

https://commons.wikimedia.org/wiki/File:Neural_network_bottleneck_achitecture.svg

{{% note %}}
let's look at one ML process called Neural Net (or Convolutional NN). each of the nodes in this diagram is just a function that takes a vector (an array) and runs a filter function over it (typically the filter itself will take a subset of the vector at a time).
{{% /note %}}

---

![scatterplot of the classic public Iris dataset](img/iris_dataset.png)

https://commons.wikimedia.org/wiki/File:Iris_dataset_scatterplot.svg

{{% note %}}
iterating on the weights of those inputs allows us to extract "features" from the training inputs that result in "interesting" classifications (decisions). this is the classic iris dataset
{{% /note %}}

---

![diagram of a deep neural net with multiple stages shown](img/deep_neural_network.png)

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
our entire industry has unified around our worries about statefulness. "run your applications as stateless containers! with k8s! let your cloud provider lock-in -- I mean securely host -- all your stateful applications!" But ML is the ultimate stateful application. you're using software to generate these software models and you ship those opaque blobs. let's get the Functional Programming crowd in a twist: the entire application is a side-effect! how can we influence those side-effects?
{{% /note %}}

---

![Google AI whitepaper: Machine Learning, the High Interest Credit Card of Technical Debt](img/machine-learning-tech-debt.png)

*https://ai.google/research/pubs/pub43146*

{{% note %}}
we desperately need better tooling to design-out unexpected behaviors in ML. We have undeclared consumers/dependencies and hidden "strange loops" of feedback. These represent a source of technical debt. and it's the worst kind of technical debt -- it's what John Allspaw and the SNAFUcatchers call "shadow debt" that's taken on unknowingly.
{{% /note %}}

---

> To make great products:

> do machine learning like the great engineer you are, not like the great machine learning expert you aren't.

> ...

> Insofar as well-being and company health is concerned, human judgement is required to connect any machine learned objective to the nature of the product you are selling and your business plan.

*[Martin Zinkevich (Google), Rules of Machine Learning: Best Practices for ML Engineering](https://developers.google.com/machine-learning/rules-of-ml/)*

{{% note %}}
we need to remember with any ML project that human judgement is required to connect the algorithms to their impact with the real world -- our business, our industry, and the community as a whole
{{% /note %}}

---

# SQL > ML

{{% note %}}
first rule should always be: why are we choosing ML over some well-tuned SQL or other algorithm? why are we choosing to use a method with chaotic feedback mechanisms instead of something that's simple and deterministic? imagine explaining to your CTO why you chose a web framework that allowed for undefined behavior on hostile inputs! is this simply because of resume-driven development?
{{% /note %}}

---

## models should be testable and human-interpretable

{{% note %}}
when we do choose ML, we should choose our approach with interpretability in mind. simple linear or logarithmic regression models are easier to debug and avoid unexpected feedback loops than models that self-optimize. remove unused features. quantify any unexpected behavior and build tests for it. these behaviors are both technical debt and avenues for adversarial input
{{% /note %}}

---

# align training data with real world demographics

{{% note %}}
choose ML training inputs that reflect the population. this is a fortunate case where we can easily align engineering ethics with business needs in a way the business understands (ex. "if we pick machine vision training data that reflects real demographics, we can avoid the embarrassment for our organization of having to explain why our software acts racist.") win-win, eh?
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

![cartoon punching a clock with a JIRA ticket](img/jira-clock-puncher.png)
{{% fragment %}}![cartoon punching a clock with a JIRA ticket](img/jira-clock-puncher.png){{% /fragment %}}
{{% fragment %}}![cartoon punching a clock with a JIRA ticket](img/jira-clock-puncher.png){{% /fragment %}}
{{% fragment %}}![cartoon punching a clock with a JIRA ticket](img/jira-clock-puncher.png){{% /fragment %}}
{{% fragment %}}![cartoon punching a clock with a JIRA ticket](img/jira-clock-puncher.png){{% /fragment %}}
{{% fragment %}}![cartoon punching a clock with a JIRA ticket](img/jira-clock-puncher.png){{% /fragment %}}
{{% fragment %}}![cartoon punching a clock with a JIRA ticket](img/jira-clock-puncher.png){{% /fragment %}}
{{% fragment %}}![cartoon punching a clock with a JIRA ticket](img/jira-clock-puncher.png){{% /fragment %}}
{{% fragment %}}![cartoon punching a clock with a JIRA ticket](img/jira-clock-puncher.png){{% /fragment %}}
{{% fragment %}}![cartoon punching a clock with a JIRA ticket](img/jira-clock-puncher.png){{% /fragment %}}
{{% fragment %}}![cartoon punching a clock with a JIRA ticket](img/jira-clock-puncher.png){{% /fragment %}}
{{% fragment %}}![cartoon punching a clock with a JIRA ticket](img/jira-clock-puncher.png){{% /fragment %}}
{{% fragment %}}![cartoon punching a clock with a JIRA ticket](img/jira-clock-puncher.png){{% /fragment %}}
{{% fragment %}}![cartoon punching a clock with a JIRA ticket](img/jira-clock-puncher.png){{% /fragment %}}
{{% fragment %}}![cartoon punching a clock with a JIRA ticket](img/jira-clock-puncher.png){{% /fragment %}}

{{% note %}}
formal Agile methodologies contribute to the problem. "act ethically" doesn't have any story points in this epic. But you're not a assembly line worker punching out JIRA tickets, you're a professional engineer! act like it!
{{% /note %}}

---

> We aren't a craft anymore. We might feel like artisans with laptops but what we produce could potentially be in front of a significant chunk of the human race by lunchtime. We're not hand-crafting dovetail joints here.

*[Anne Currie, The Register, 1 Mar 2018](https://www.theregister.co.uk/2018/03/01/ethics_yeah_thats_great_but_do_they_scale/)*

{{% note %}}
leave you with this from Anne Currie at ContainerSolutions. "We aren't a craft anymore. We might feel like artisans with laptops but what we produce could potentially be in front of a significant chunk of humanity by lunchtime."
{{% /note %}}

---

# let's get to work

{{% note %}}
what we do has impact. let's get to work. thanks, folks!
{{% /note %}}
