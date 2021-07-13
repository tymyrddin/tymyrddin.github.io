---
title: "Grey areas"
modified: 2021-05-07T00:14:00+00:00
categories:
  - Elephants
tags:
  - Elephants
  - Trends
---

The creation of legal grey areas, per three examples, using the example of sexual consent for clarity and because that is where the "consent" concept originated and is expanding from in every day life for digital consent:

- [Sexual consent](#sexual-consent)
- [General Data Protection Regulation](#general-data-protection-regulation)
- [Federated Learning of Cohorts](#federated-learning-of-cohorts)

## Sexual consent

I don't think "sexual consent" exists other than as a legal term. If I "consent", it means "I voluntarily agree to engage in a certain sexual activity". Further let's assume I had both the freedom and capacity to consent, then the question is whether I agree to the activity by choice, not by coercion or force. A grey area.

If the other person "did not reasonably believe" that I consented and continued to engage in sexual behaviour despite me saying "no", he or she committed a sexual offence.

This makes rape victims the key element in the issues surrounding consent and where common notions of victim-blaming often come into play: "The clothing she wore was an invitation", "She was drunk", "We live together", and "We've had sex before", etc. As far as I know, wearing clothes, having a drink, living together with someone, or having mutually consenting sex, are not criminal activities.

Ofcourse there are those who want pleasurable and mutual consensual sexuality to move away from the old "no means no" mindset towards the concept of "affirmative consent": "yes means yes" because if promises more pushing of will. Affirmative consent is not just about getting permission, but about making sex based on mutual desire and enthusiasm. A wonderful ideal to strive for. But re-inventing the wheel by using "yes means yes" instead of "no means no" does not remove the grey area.

With 'yes means yes' we imply that every person has the power to say what they want when it comes to consent. This ignores the reality that [people say 'yes' sometimes out of fear, and sometimes as a result of coercion]({{ site.url }}{{ site.baseurl }}/elephants/legitimisation-patterns/). 

How about no forcing of will or coercion to push will on others, period.

## General Data Protection Regulation

Digital consent follows similar patterns.

The [GDPR (General Data Protection Regulation)]({{ site.url }}{{ site.baseurl }}/elephants/gdpr) is, in summary, a series of protocols that creates rules for businesses that do business in Europe on how to process and maintain data collected from European residents. At first glance, the GDPR champions the rights of and consent of everyday internet users and targets a supposed grey-area black hat tactics that have exploited unsuspecting people browsing the internet.

But it wasn't a grey area, it was a black area, and by regulating the collection of data it actually legitimises the processing and maintenance of data from European residents and creates a grey area in which users can give consent or opt-in or opt-out, and have to apply to have their data removed and/or to be forgotten. 

Hours after the GDPR came into force users were confronted with consent-or-be-gone types of messages and large suits against Facebook and Google appeared, accusing them of "coercing" users into accepting their data collection policies.

And as a "side note", the legislation was purely for the private sector in order to "protect the public". What about the public institutions funded by taxes from the people that are protected under the GDPR? What impact does the GDPR have on  governing institutions? What do governments in Europe have to do because of the GDPR? 

Apparently nothing: __"under EU law, the right to privacy and the right to protection of personal data are two distinct fundamental human rights."__

The European Parliament distances itself from national authorities collecting and processing citizens private data by allocating all such activities to the nation alone, __The Court of Justice of the EU does not have jurisdiction over cases that involve surveillance conducted by national authorities in order to safeguard the internal security of the EU Members.__ 

How about no collection of data, period.

## Federated Learning of Cohorts

Third-party cookies are going extinct now that many browsers block third-party cookies, but that doesn’t mean Google (and similar others) will respect our privacy. Google started an experiment called FLoC (Federated Learning of Cohorts). It runs in Google’s Chrome browser and tracks a user’s online behaviour.

Supposedly FLoC will allow personalized ads without the collection of data that can be tied to specific people. By assigning each browser an anonymised ID and then adding that ID into a large group, a cohort, where only the overall patterns are accessible to advertisers, the idea is that our privacy will remain intact, while Google and its advertising partners use it for widespread tracking and personalisation of ads.

Marshall Vale, the product manager of Google’s privacy sandbox: __"Before a cohort becomes eligible, Chrome analyzes it to see if the cohort is visiting pages with sensitive topics, such as medical websites or websites with political or religious content, at a high rate. If so, Chrome ensures that the cohort isn’t used, without learning which sensitive topics users were interested in."__

Sounds awesome, but what is really happening and possible in this grey area?

A user’s browser, a tool to interact with the internet, is supposed to be sacred. FLoC turns it into a real-time tracking tool collecting the most sensitive information about an individual user’s browsing habits without the user being able to circumvent or opt out of this data collection.

And when the FLoC data set is big enough, [deanonymisation will become easy](https://github.com/tymyrddin/orchard/tree/main/threat-modelling/DA-threat-model). For example, cohorts of users sharing the same location data, shop in the same neighbourhood, are active in the same time zone, [can be easily be grouped together](https://tymyrddin.gitbook.io/orchard/threat-modelling/DA-threat-model/attack-vectors/Classification-analysis.md) by demographics, and if the data is combined with other tracking mechanisms such as social media analytics or data sets purchased from [data brokers](https://tymyrddin.gitbook.io/orchard/threat-modelling/DA-threat-model/adversaries/Data-brokers.md), fingerprinting users based on age, class, ethnicity, political parties becomes trivial.

[Google announced](https://developer.chrome.com/blog/privacy-sandbox-update-2021-jan/) that in Chrome version 89 they will forcibly enable and trial their FLoC data-collection initiative without the consent of users or webmasters. 

Our options are reduced to “You either have old tracking or new tracking”?
Not entirely, because [users](https://tymyrddin.gitbook.io/orchard/mitigations/data/browsing/FLoC.md) and [webserver adminstrators and webmasters](https://tymyrddin.gitbook.io/orchard/mitigations/data/webapplication/FloCed-sites.md) can jump through hoops, again. 

It is annoying, very annoying, these constant attacks on our privacy. How about no tracking, period.

And as a "side note": Wouldn't it be good if algorithms that keep users engaged for maximising revenues by recommending (political, sensasionalist, hateful, false) content, simply did not exist? 