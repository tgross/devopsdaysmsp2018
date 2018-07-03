+++
title = "DevOps Days MSP 2018"
outputs = ["Reveal"]

[reveal_hugo]
custom_theme = "./css/devopsdays.css"
highlight_theme = "solarized-dark"

+++

# They Didn't Stop To Think If They Should

#### Tim Gross | Machinist Labs | @0x74696d

---

## or...
## Machine Learning And The Internet Of Unpatched Things

{{% note %}}
an alternate title could be...
{{% /note %}}

---

## or...
## Because Eternal Vigilance is the Price of Liberty, We Have to Talk About Ethics Again

---

> We've updated our privacy policy!

> The opinions expressed in this talk are the speaker's alone and do not reflect the view of this conference, your employer, or my mom. Any reference to or citation of any person or organization does not constitute or imply an endorsement or recommendation of the content of this talk. The speaker is grossly unqualified to tell you how to live you life. Your mileage may vary. Not to be used in the manufacture of nuclear weapons. By attending this talk the speaker hereby grants you an irrevocable, perpetual, non-exlusive, tranferable, worldwide license to be excellent to each other.

{{% note %}}
why is it especially important to talk about ethics when we start talking about ML and IoT? What makes these things special?
{{% /note %}}

---

![uber-self-driving](img/uber-accident.png)

*[Michael Laris, Washington Post, 24 May 2018](https://www.washingtonpost.com/news/dr-gridlock/wp/2018/05/24/ntsb-self-driving-uber-did-not-have-emergency-braking-turned-on/)*


{{% note %}}
Back in March a self-driving car operated by Uber killed a pedestrian
{{% /note %}}

---

![microsoft-chatbot](img/microsoft-chatbot.png)

*[James Vincent, The Verge, 24 Mar 2016](https://www.theverge.com/2016/3/24/11297050/tay-microsoft-chatbot-racist)*

{{% note %}}
MSFT embarrassed itself with the Tay chatbot a couple years ago
{{% /note %}}

---

![uk-ransomware](img/uk-ransomware.png)

*[Russell Brandom, The Verge, 12 May 2017](https://www.theverge.com/2017/5/12/15630354/nhs-hospitals-ransomware-hack-wannacry-bitcoin)*

{{% note %}}
last year countless devices in UK hospitals were taken over by Wannacry ransomeware, putting patient lives at risk
{{% /note %}}

---

![tesla-autopilot](img/tesla-autopilot.png)

*[The Guardian, 31 Mar 2018](https://www.theguardian.com/technology/2018/mar/31/tesla-car-crash-autopilot-mountain-view)*

{{% note %}}
Tesla's autopilot has been implicated in the deaths of several drivers at this point
{{% /note %}}

---

![target-pregnant](img/target-pregnant.png)

*[Kashmir Hill, Forbes, 16 Feb 2012](https://www.forbes.com/sites/kashmirhill/2012/02/16/how-target-figured-out-a-teen-girl-was-pregnant-before-her-father-did/)*

{{% note %}}
Machine learning algorithms may know more about us and our loved ones than we do ourselves...
{{% /note %}}

---

![google-racist-autotag](img/google-racist-autotag.png)

*[Jana Kasperkevic, The Guardian, 1 Jul 2015](https://www.theguardian.com/technology/2015/jul/01/google-sorry-racist-auto-tag-photo-app)*

{{% note %}}
... while simultaneously unconsciously encoding our biases
{{% /note %}}

---
![defeat-the-baby](img/defeat-the-baby.png)

*https://twitter.com/yipe/status/1005555741153902592*

{{% note %}}
we've invited these systems into our homes...
{{% /note %}}

---

![alexa-eavesdropping](img/alexa-eavesdropping.png)

*[Laura Stevens, Huffington Post, 24 May 2018](https://www.huffingtonpost.com/entry/alexa-eavesdropping-portland-familiy_us_5b0727cae4b0fdb2aa51b23e)*

{{% note %}}
... with almost no oversight into what they're doing
{{% /note %}}

---

![marco](img/marco-rogers.png)

{{% note %}}
and at the end of the day, it's people in our industry -- the people in this room -- who are the ones who execute it.
{{% /note %}}

---

# a problem of scale

{{% note %}}
the problem we have here is not just that these systems all have serious real-world consequences; we can look at the Therac-25 accidents in the 80's for examples of that.
the problem is that those consequences are multiplied by the scale of these systems
{{% /note %}}

---

## quantity has its own quality

{{% note %}}
a huge part of the value proposition of IoT and ML is the
scale of the data involved: collecting massive amounts of data
from edge computing devices, and processing massive amounts of
data in ML models.
{{% /note %}}

---

## no meaningfully informed consent

{{% note %}}
but the scope of machine learning and IoT is incomprensible to
ordinary users; creating informed and meaningful consent is all
but impossible
{{% /note %}}

---

![machine-learning-tech-debt](img/machine-learning-tech-debt.png)

*https://ai.google/research/pubs/pub43146*

{{% note %}}
while ML "models" are probably reasonably well-understood by the elite developers of the best organizations, most users of ML treat the models as binary blobs -- a black d a simple neural network in 9 lines of Python code
work to Play FlappyBird
JULY 10, 2016

200 lines of python code to demonstrate DQN with Keras

box into which numbers go and decisions come out. "in 100 lines of Python"
{{% /note %}}

---

![in_X_lines](img/in_X_lines_01.png)
{{% fragment %}}![in_X_lines](img/in_X_lines_02.png){{% /fragment %}}
{{% fragment %}}![in_X_lines](img/in_X_lines_03.png){{% /fragment %}}
{{% fragment %}}![in_X_lines](img/in_X_lines_04.png){{% /fragment %}}
{{% fragment %}}![in_X_lines](img/in_X_lines_05.png){{% /fragment %}}
{{% fragment %}}![in_X_lines](img/in_X_lines_06.png){{% /fragment %}}
{{% fragment %}}![in_X_lines](img/in_X_lines_07.png){{% /fragment %}}

---

![ugly-t-shirt](img/ugly-t-shirt.jpg)

*[Robison Meyer, The Atlantic, 3 Oct 2013](https://www.theatlantic.com/technology/archive/2013/10/avoid-facial-detection-algorithms-with-a-t-shirt/280253/)*


{{% note %}}
the consequences of this are open-ended.
when someone uses a William Gibson's Ugly TShirt...
{{% /note %}}

---

![face-recognition-glasses](img/face-recognition-glasses.png)

*[James Vincent, The Verge, 3 Nov 2016](https://www.theverge.com/2016/11/3/13507542/facial-recognition-glasses-trick-impersonate-fool)*

{{% note %}}
or face-recognition fooling glasses to mislead systems not simply to protect their own identity but to summon a SWAT team in hopes of an "accident", do the systems bear any responsibility?
{{% /note %}}

---

![adversarial-toaster](img/adversarial-toaster.png)

*[James Vincent, The Verge, 3 Jan 2018](https://www.theverge.com/2018/1/3/16844842/ai-computer-vision-trick-adversarial-patches-google)*

{{% note %}}
or when a banana looks, not like a toaster, but a bomb or weapon?
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

---

## embedded industry stuck in archaic threat model

{{% note %}}
if you thought the enterprise was bad...
- still shipping devices with private keys and hard-coded passwords
- "secure boot" (without which any device can be rooted) is an expensive add-on rather than the default
{{% /note %}}

---

![hawkbit](img/hawkbit-logo.png)

*http://www.eclipse.org/hawkbit/*

{{% note %}}
existing solutions for IoT Over-the-Air updates (OTA) are mostly research projects at best (ex. Hawkbit)...
{{% /note %}}

---

![aws-iot](img/aws-iot.png)

*[Robert McCauley, Alexa Blogs, 3 May 2016](https://developer.amazon.com/de/blogs/post/Tx3828JHC7O9GZ9/Using-Alexa-Skills-Kit-and-AWS-IoT-to-Voice-Control-Connected-Devices)*

{{% note %}}
... or require trust delegation and put secure boot at risk
{{% /note %}}


---

## Our abdication of responsibility invites political remedy

{{% note %}}
the problem with out complacency on this as an industry is that it invites someone to "do something" about it.
{{% /note %}}

---

![congress](img/congress.jpg)

*https://www.brookings.edu/wp-content/uploads/2016/06/congress006-1.jpg*

{{% note %}}
legal remedy is likely to be ham-fisted...
{{% /note %}}

---

## "We have to do something!"
## "This is something"
## "We must do this!"

---

![series-of-tubes](img/series-of-tubes.png)

*https://imgur.com/gallery/2mIObIu*

{{% note %}}
... particularly here in the US where almost all our lawmakers are incompetent...
{{% /note %}}

---

![ajit-pai](img/ajit-pai.png)

*[Terrence O'Brien, engadget, 18 May 2017](https://www.engadget.com/2017/05/18/fcc-chairman-net-neutrality-1996/)*

{{% note %}}
... or are entirely co-opted by hostile interests
{{% /note %}}

---

> Disclaimer of Warranty. Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.

*https://www.apache.org/licenses/LICENSE-2.0*

{{% note %}}
this is the Apache license but other OSS licenses are similar, as are most EULAs.
software is typically sold w/o warantee for fitness for any particular use; this could change
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
the childishness and utter lack of professionalism we've seen with GDPR
{{% /note %}}

---

![gdpr-hackernews](img/gdpr-hackernews.png)

*https://news.ycombinator.com/item?id=16954306*

{{% note %}}
aw, poor baby!
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
...then it's all working as intended!
{{% /note %}}

---

# feature, not bug

---

> Salesforce CEO Marc Benioff thinks America needs "a national privacy law... that probably looks a lot like GDPR.

> "This is going to help our industry... It's going to set the guardrails around trust, around safety. It's going to provide the ability for the customers to interact with great next generation technologies in a safe way."

*[Simon Sharwood, The Register, 30 May 2018](https://www.theregister.co.uk/2018/05/30/salesforce_q1_2019/?)*


---

> Benioff went on to say that as artificial intelligence is used in customer service, "that starts to cross the line on what is trust. And that's where our industry really has to come forward and say we're going to make sure that these technologies are trust-based. And I think the Europeans definitely got that figured out."

*[Simon Sharwood, The Register, 30 May 2018](https://www.theregister.co.uk/2018/05/30/salesforce_q1_2019/?)*

---

# Consent

{{% note %}}
consent is the *only* workable guiding model when we're talking about relationships between individual people. I consent to
{{% /note %}}

---

# Individual vs Community Consent

---

![vaccines](img/vaccines.jpg)

*[Steve Sack, Star Tribune, 27 Jan 2015](http://www.startribune.com/sack-cartoon-vaccinations/289998831/)*

{{% note %}}
every culture has different boundaries here.
ex. in the EU they protect individual consent strongly...
{{% /note %}}

---

![kelo-house](img/kelo-vs-new-london.png)

*[Ilya Somin, Washington Post, 29 May 2015](https://www.washingtonpost.com/news/volokh-conspiracy/wp/2015/05/29/the-story-behind-the-kelo-case-how-an-obscure-takings-case-came-to-shock-the-conscience-of-the-nation/)*

{{% note %}}
... whereas in the US we have a mixed bag where businesses get the power of community consent to override the will of individuals, but very little of the responsibility of individual consent.
{{% /note %}}

---

![externality](img/externality-definition.png)

*https://www.google.com/search?q=externality*

{{% note %}}
aside: are these results being manipulated? the *canonical* example is pollution!
{{% /note %}}

---

# values vary

{{% note %}}
Flaws of the Consent Model as a Solution
- ethical definitions vary b/c values vary (ex. balance of community vs individual consent varies significantly between Europe and the US)
- how do other professions solve this problem...?
{{% /note %}}

---

![sonia-1](img/sonia-1.png)

*https://twitter.com/soniagupta504/status/1011591288003575808*

{{% note %}}
Sonia (who was up here on stage last night):
"Lawyers and doctors enter their professions knowing, from the outset, just how heavy  their burdens are. They hold human rights and life in their hands."
{{% /note %}}

---

![sonia-2](img/sonia-2.png)

*https://twitter.com/soniagupta504/status/1011591288003575808*

{{% note %}}
highly impactful professions know that their limits must be more stringent
{{% /note %}}

---

## "With great power comes great responsibility"

---

# professional ethics

---

# licensing as
# self-regulation

{{% note %}}
historically licensing and professional organizations (ex. AMA, AIA, ASME, bar associations) have arisen from the professions themselves rather than being imposed clumsily from the outside.
government licensing requirements are typically delegated to the professional organizations
{{% /note %}}

---

# licensing requires monopoly

{{% note %}}
- professional certification w/o regulation or consequences is toothless and worthless (ex. CompTIA or ICS^2 or Project Management Institute)
- professional organizations ethical requirements are typically about fair dealing and bare minimum safety guidelines
{{% /note %}}

---

> We do not believe that it is merely a coincidence that the entry and standards of practice are most strictly regulated for physicians, dentists, and veterinarians... where the costs of receiving poor services could be high or sometimes even catastrophic.

*[ref http://www.nber.org/papers/w10467.pdf](http://www.nber.org/papers/w10467.pdf)*

{{% note %}}
study by Marc Law & Sukkoo Kim of National Bureau of Economic Research shows that professional organizations have acted mostly as a counter to information assymmetry rather than creating monopoly power...
{{% /note %}}

---

# gatekeeping

{{% note %}}
... so in other words they serve as gatekeepers.
well, that's a little problematic isn't it? currently our barriers to entry are *relatively* low relative to other professions that provide the ability to bootstrap into the middle class. (although we still have a *lot* of work to do!) so adding gatekeeping mechanisms seems like it'd work against the direction with want to take our industry wrt inclusion
{{% /note %}}

---

# shared ethical baseline

{{% note %}}
but an advantage of a professional organization's ethical framework is that it at least gives a shared baseline: right now we're all trying to figure this out for ourselves.
we should hold each other to task
{{% /note %}}

---

# what is to be done?

{{% note %}}
waiting for "the industry" to fix it isn't working.
we all, individually, are the industry. need to take individual action:
- influence the community
- ex. talk about this stuff!
- ex. what organizations do we work for?
{{% /note %}}

---

![microsoft-employees-ice](img/microsoft-employees-ice.png)

*[Peter Bright, Ars Technica, 20 Jun 2018](https://arstechnica.com/tech-policy/2018/06/microsoft-staff-call-on-company-to-end-ice-contract/)*

{{% note %}}
influence the organization
we see Microsoft employees pushing for change in what customers their organization serves
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
the labor market for our profession gives us enormous power right now.
- we can push hard for better hiring policies
- we can push hard for D&I efforts
- we can push hard for our organizations to be better
{{% /note %}}

---

# ensure your own mask is secure

{{% note %}}
that being said, we should also cut each other some slack. you don't know much about the circumstances of any particular person. so while we should be holding each other to task, individuals need to make their own decisions about where they work and that doesn't make them The Enemy. (unless they work at Oracle, just sayin')
{{% /note %}}

---

# direct action

{{% note %}}
what is available to everyone regardless of our work conditions, and perhaps more effective than anything else we can do, is direct action at an engineering level
what choices do we make as technologists?
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
we need to take responsibility for quality proportional to the risks involved with the software. while this is obvious in self-driving cars, we need to design-out unexpected behaviors in ML.
{{% /note %}}

---

![gdpr-tumblr](img/tumblr-gdpr.png)

*https://twitter.com/Millstab/status/999762424994594817*

{{% note %}}
push back against dark UX patterns
{{% /note %}}

---

## Immutable?

![kafka](img/Kafka.png)

[Jay Kreps, Cloudera, 11 June 2015](https://vision.cloudera.com/apache-kafka-a-platform-for-real-time-data-streams-part-1/)

{{% note %}}
many orgs are using immutable event stores
{{% /note %}}

---

## "Immutable"

![kafka](img/Kafka-per-user.png)

{{% note %}}
... per user encryption keys can be used to allow immutable infrastructures that are compatible with the "right to be forgotten"
{{% /note %}}

---

# ML models are state

{{% note %}}
speaking of immutability...
our entire industry has unified around our worries about statefulness, but...
ML is the ultimate stateful application
the entire model is a side-effect, so you can't design-out side-channel attacks.
{{% /note %}}

---

# align training data with real world demographics

{{% note %}}
- choosing ML model inputs that reflect the population
- align engineering ethics with business needs (ex. "if we pick machine vision training data that reflects real demographics, we can avoid the embarassment for our organization of having to explain why our software acts racist.")
{{% /note %}}

---

# technical leadership

{{% note %}}
- we can't rely on project managers or business analysts to take the lead on designing our systems ethically because they simply may not understand the side-effects. you're the technical professional: they're expecting you to take the lead on this!
{{% /note %}}


---

# "best practice is..."

{{% note %}}
"the best thing about best practices is there are so many of them to choose from"
bypass business analysts and project managers on opinions that are purely technical
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
formal Agile methodologies contribute to the problem. "act ethically" doesn't have any story points in this epic.
But you're supposed to be a professional, not a JIRA clock puncher. act like it!
{{% /note %}}

---

> We aren't a craft anymore. We might feel like artisans with laptops but what we produce could potentially be in front of a significant chunk of the human race by lunchtime. We're not hand-crafting dovetail joints here.

*[Anne Currie, The Register, 1 Mar 2018](https://www.theregister.co.uk/2018/03/01/ethics_yeah_thats_great_but_do_they_scale/)*

---

# let's get to work
