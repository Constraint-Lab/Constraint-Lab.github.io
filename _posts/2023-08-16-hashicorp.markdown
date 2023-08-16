---
title: Is HashiCorp a Broken Brand?
tags: hashicorp branding
excerpt: Is HashiCorp's decision to change their software license a breaking of their brand promise, similar to Halston's fatal deal with JCPenney? This article delves into the implications of HashiCorp's shift from MPL 2.0 to BSL, comparing it to other tech companies like MongoDB and Elastic. Analyzing key factors such as switching costs, scale economies, branding, and network economies, it examines whether HashiCorp's move is a strategic misstep or a well-calculated business decision.
---

> What it means to have a brand is you’ve made a promise to people. - Seth Godin

In 1983, Halston signed a one billion dollar deal with JCPenney.

[That deal was the beginning of the end for Halston.][halston]

Halston started as a fashion designer in the 1960s, eventually being described as "the top of the fashion show-biz heap." He designed the pillbox hat that first lady Jacqueline Kennedy wore to her husband's inauguration, made uniforms for the U.S. Olympic teams, and created costumes for a famous ballet. He was seen with a group of models so often that they became known as "the Halstonettes."
In short, he was the picture of glamor and exclusivity.

His deal with JCPenney was self-described as being "for the American people."

And, while noble perhaps, it was not what he had promised.

[HashiCorp's decision to change their license][hashi license] looks like a similar breaking of a promise.

HashiCorp changed their license from Mozilla Public License v2.0 (MPL 2.0) to Business Source License (BSL). The key result is their software is no longer free if competitors use it to compete with HashiCorp. Regardless of what business sense this makes (or not), the open source community takes the principles of open source software (OSS) seriously. A vocal group has come out in opposition to the change, believing that HashiCorp has profited off OSS only to abandon it once inconvenient.

Is this a significant misstep from HashiCorp in the vein of Halston?

Even if this choice is a breaking of the brand promise, it might not matter because of several potential HashiCorp strengths.

If the cost of switching from HashiCorp's offerings is too high, it doesn't matter in the short term if trust is broken. And given the current high cost of capital, the appetite for paying that switching cost is lower than recent past. The high capital cost also means fewer new startups that can choose a different product from the start.

There is also no 800 lb. gorilla competitor with the resources to easily fork the project into a similar offering. Making the change now makes such an event more unlikely as time goes on.

Current direct competitors immediately face pressure to either work out a licensing deal or create a fork (HashiCorp's advantages with a licensing deal are obvious). Not only does creating a fork create an immediate drain on competitors' resources, but they are all competing with each other and at a significant disadvantage to HashiCorp owning the main branch. Even if HashiCorp's customers are turned off by the broken brand promise, they'd still need to believe a) another company will figure out a "true" OSS business model, and b) they are able to figure out which company that is up front.

If we look at past history to determine the wisdom of the decision, Mongodb and Elastic are two companies that are especially interesting comparisons. Both companies share relevant similarities:

* Changed licenses to add restrictions on commercial usage after going public.
* AWS released a similar product ([DocumentDB for Mongodb][documentdb], [OpenSearch for ElasticSearch][opensearch]).

However, their trajectories are significantly different. Mongodb is up ~464% since their license change (Oct 18 - Aug 23) while Elastic is down ~63% since theirs (Jan 21 - Aug 23).

<figure>
<img src="/resources/elastic-stock.png" alt="Elastic Stock">
<figcaption>Elastic Stock Price Jan 21 - Aug 23</figcaption>
</figure>
<figure>
<img src="/resources/mongo-stock.png" alt="Mongodb Stock">
<figcaption>Mongodb Stock Price Oct 18 - Aug 23</figcaption>
</figure>

If we use stock price as a way to judge the results of their decision, we can say that simply breaking the OSS brand promise is not a significantly bad decision, even when there is a readily available and trusted alternative.

Given those considerations, I think HashiCorp has made a good business decision. What it means to be OSS is a regular debate, so it's not even clear that a significant portion of the customer base feels that HashiCorp broke a promise (or that they had any other options). And even if that group is significant, HashiCorp's positioning appears strong enough to weather the criticism.

If I were to further explore the decision, here are a few threads I'd follow:
* What were the competitive environments for Mongo and Elastic, and how similar were they to HashiCorp's?
* What other strategic decisions might explain the difference between Mongo and Elastic, and what similar options are available for HashiCorp?
* HashiCorp lists other companies that have made similar license changes. Apply similar analysis to those companies to help understand the best HashiCorp strategy moving forward.

[Powers at play][powers]:
* **Switching Costs**: Changing infrastructure _that is working adequately_ is a hard sell, especially given the current high cost of capital.
* **Scale Economies**: HashiCorp has the cost of OSS built into their model. Competitors that were simply building _on_ OSS now have to add that cost. This is enhanced by the current high cost of capital.
* **Branding**: HashiCorp is negatively affected as mentioned previously, but they also enjoy the benefit of owning the main fork. Customers that choose a branch are introducing uncertainty. HashiCorp might also get a bump in trustworthiness if customers are satisfied that they now have a sustainable business model.
* **Network Economies**: The network exists between companies and engineers. The more engineers that use HashiCorp, the easier it is to hire. And the more companies that use HashiCorp, the easier it is to get hired.

[halston]: https://www.fastcompany.com/90637111/what-happened-to-halston-the-rise-and-fall-of-an-american-fashion-icon
[hashi license]: https://www.hashicorp.com/blog/hashicorp-adopts-business-source-license
[documentdb]: https://techcrunch.com/2019/01/09/aws-gives-open-source-the-middle-finger/
[opensearch]: https://aws.amazon.com/blogs/opensource/introducing-opensearch/
[powers]: https://www.amazon.com/7-Powers-Foundations-Business-Strategy/dp/0998116319
