# Paper Review: On the dangers of stochastic parrots: Can language models be too big?

## Overview

### Background

One of the biggest trends in natural language processing (NLP) has been the increasing size of language models (LMs) as measured by the number of parameters and size of training data. Both datasize and parameter are experiencing explosive growth. But our hardware are not growing that fast.The graph below shows this trend.


<img width="1285" alt="image" src="https://user-images.githubusercontent.com/69759816/161464139-92c1b423-c34d-46e8-b017-d08662477b26.png">



### What are the risks?

- Environmental and financial costs
- Unmanageable training data
- Research trajectories
- Potential harms of synthetic language

### Environmental costs & financial inaccessibility

- Average human across the globe responsible for 5t of CO2 emissions per year*
- Transformer model training procedure on GPUs 284t of CO2 emissions
- 0.1 BLUE score increase en-de results in increase of ~$150,000 in compute cost
- Encourage reporting training time and sensitivity to hyperparameters
- Suggest more equitable access to compute clouds through government

**Current mitigation efforts:**

- Renewable energy sources
- Prioritize computationally efficient hardware
- Document energy and carbon metrics


**Large LMs, particularly those in English and other high-resource languages, benefit those who have the most in society**
- Marginalized communities around the world impacted most by climatechange
- Maldives threatened by rising sea levels (Anthoff et al 2010)
- But these communities are rarely able to see benefits of language technology because LLMs aren’t built for their languages.

### Unmanageable Training Data

**A large dataset is not necessarily diverse**
Who has access to the Internet and is contributing?
- Younger people and those from developed countries
Who is being subject to moderation?
-Twitter - accounts receiving death threats more likely to be suspended than those issuing threats
What parts of the Internet are being scraped?
- Reddit - US users 67% men and 64% are ages 18-29
- Wikipedia - only 8.8-15% are women or girls
- Not many sites with fewer incoming and outgoing links, like blogs

**Static data/Changing social views**

**Bias**

![image](https://user-images.githubusercontent.com/69759816/161466587-9cfc26ab-4581-4cf8-99c4-48d1c2e5247c.png)


### Research Trajectories

- Focus on LMs and achieving new state-of-the-art(SOTA) on leaderboards, particularly NLU
- But LMs have been shown to excel due to spurious dataset artifacts (Niven & Kao 2019, Bras et al 2020)
- LMs trained only on linguistic form don’t have access to meaning (Bender & Koller 2020)
- Are we actually learning about machine language understanding?

### Potential harms of synthetic language

- Human-human interaction is co-constructed and leads to a shared model of the world (Reddy 1979, Clark 1996)
- An LM is a system for haphazardly stitching together linguistic forms from its vast training data, without any reference to meaning: a stochastic parrot.
- Nonetheless, humans encountering synthetic text make sense of it
- Denigration, stereotype threat, hate speech: harms to reader, harms to bystanders
- Cheap synthetic text can boost extremist recruiting (McGuffie & Newhouse 2020)

### Risk management strategies

**Allocate valuable research time carefully**
- Incorporate energy and compute efficiency in planning and model evaluations
- Select datasets intentionally
- ‘Feeding AI systems on the world’s beauty, ugliness, and cruelty, but expecting it to reflect only the beauty is a fantasy.’ (Birhane and Prabhu 2021, after Benjamin)
- Document process, data, motivations, and note potential users and stakeholders
- Pre-mortem analyses: consider worst cases and unanticipated causes
- Value sensitive design: identify stakeholders and design to support their values




## Critical Analysis

I disagree with this article in general because
- The rapid growth shows that the limit is far from being reached, so there is a lot of room for growth.
- We can't negate more advantages because of potential drawbacks.
- I agree with part of it in overfitting and bias. But I don't think stereotypes and racism have connection with model size.
- Why Explore Space?

![image](https://user-images.githubusercontent.com/69759816/161469459-c1f8c1e2-bbe5-4df0-bc09-ac03055950e5.png)

In 1970, a nun wrote to Dr. Stuhlinger, the associate director of science at NASA’s Marshall Space Flight Center, in response to his ongoing research into a piloted mission to Mars. Specifically, she asked how he could suggest spending billions of dollars on such a project at a time when so many children were starving on Earth.

The voyage to Mars will certainly not be a direct source of food for the hungry. However, it will lead to so many new technologies and capabilities that the spin-offs from this project alone will be worth many times the cost of its implementation.

## Discussion

### Topic 1:

How big is too big?

### Topic 2:

Are ever larger language models (LMs) inevitable or necessary?

### Topic 3:

How can we pursue the research direction while reduciing its associated risks?

## Resource Links

Paper: https://dl.acm.org/doi/10.1145/3442188.3445922

Repo & Video: https://www.turing.ac.uk/events/dangers-stochastic-parrots

## Other Resources

* [When is a neural net too big for production?](https://neal-lathia.medium.com/when-is-a-neural-net-too-big-for-production-4315452193ef)

* [Large Language Models: A New Moore's Law?](https://huggingface.co/blog/large-language-models)

* [Why Explore Space?](https://lettersofnote.com/2012/08/06/why-explore-space/)

## Video Recording

https://youtu.be/knO4dpdAzCk

## Code Demo

https://openai.com/blog/better-language-models/

Since this article is about theory, i.e. ethics rather than technique. Thus, my demo code is to show that there still is a lot of room for improvement in Big LMs.
