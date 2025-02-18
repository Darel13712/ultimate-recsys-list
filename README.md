# ultimate-recsys-list

Ultimate list of various problem formulations and subtasks in recommender systems

# Table of Contents

- [Top‑k Recommendations](#top-k-recommendations)
- [Rating Prediction](#rating-prediction)
- [Click‑Through Rate (CTR) Prediction](#click-through-rate-ctr-prediction)
- [Collaborative Filtering](#collaborative-filtering)
  - [Neighbourhood‑Based Collaborative Filtering](#neighbourhood-based-collaborative-filtering)
  - [Model‑Based Collaborative Filtering](#model-based-collaborative-filtering)
- [Content‑Based Recommendation](#content-based-recommendation)
- [Hybrid Recommendation](#hybrid-recommendation)
- [Multi‑Modal RS](#multi-modal-rs)
- [Ensemble‑Based RS](#ensemble-based-rs)
- [Graph Recommendation](#graph-recommendation)
- [Knowledge‑Based Recommendation](#knowledge-based-recommendation)
  - [Case‑Based Recommendation](#case-based-recommendation)
- [Constraint‑Based Recommendation](#constraint-based-recommendation)
- [Sequential Recommendation](#sequential-recommendation)
- [Package RS](#package-rs)
- [Next‑Basket Recommendation](#next-basket-recommendation)
- [Session‑Based Recommenders](#session-based-recommenders)
  - [Session‑Aware Recommendation](#session-aware-recommendation)
- [Interactive RS](#interactive-rs)
- [Conversational RS](#conversational-rs)
- [Recommendation Editing](#recommendation-editing)
- [Active Learning in RS](#active-learning-in-rs)
- [Group Recommendations](#group-recommendations)
- [Reciprocal Recommendations](#reciprocal-recommendations)
- [Diversification in RS](#diversification-in-rs)
- [Calibrated Recommendations](#calibrated-recommendations)
- [Multi‑Interest Recommendations](#multi-interest-recommendations)
- [Intent‑Aware Recommendations](#intent-aware-recommendations)
- [Cross‑domain RS](#cross-domain-rs)
- [Reinforcement Learning in RS](#reinforcement-learning-in-rs)
- [Multi‑Criteria RS](#multi-criteria-rs)
- [Multi‑Stakeholder Recommendations](#multi-stakeholder-recommendations)
- [Context‑Aware Recommendations](#context-aware-recommendations)
- [Risk‑Aware RS](#risk-aware-rs)
- [Mobile RS](#mobile-rs)
- [Location‑Based Recommendation](#location-based-recommendation)
- [Time‑Aware Recommendation](#time-aware-recommendation)
- [Emotion‑(Sentiment‑Based) Recommendation](#emotion-based-recommendation)
- [Social RS](#social-rs)
- [Trust‑Centric Recommendation](#trust-centric-recommendation)
- [Trigger‑Induced Recommendation](#trigger-induced-recommendation)
- [Trustworthy RS](#trustworthy-rs)
- [Adversarial RS](#adversarial-rs)
- [Privacy‑Aware Recommendation](#privacy-aware-recommendation)
- [Fairness‑Aware RS](#fairness-aware-rs)
- [Explainable Recommendations](#explainable-recommendations)
- [Upselling Recommendations](#upselling-recommendations)
- [Cross‑Selling Recommendations](#cross-selling-recommendations)
- [Quantum RS](#quantum-rs)
- [Other types by application](#other-types-by-application)
  - [Agriculture](#agriculture)
  - [HR](#hr)
  - [Tourism](#tourism)
  - [Fashion](#fashion)
  - [Food](#food)
  - [Music](#music)
    -  [Automatic Playlist Continuation](#automatic-playlist-continuation)
  - [Music Events](#music-events)
  - [Multimedia](#multimedia)


## Top-k Recommendations

Choose k most relevant from all unseen items. Order of items in the recommendation list matters. Most wide-spread default variant.



## Rating Prediction

Estimate the explicit rating a user would assign to an item, then rank items accordingly.

Less used today in favour of top-k recommendations, see "[Being Accurate is Not Enough: How Accuracy Metrics have hurt Recommender Systems](https://grouplens.org/site-content/uploads/accurate-CHI-20061.pdf)"



## Click-Through Rate (CTR) Prediction

Predict the probability that a user will click on (or interact with) an item.



## Collaborative Filtering

Is a family of methods that uses information about similarities between different users to generate recommendations. Most widespread variant. 



### Neighbourhood-Based Collaborative Filtering

Memory- or heuristic-based. Directly uses user-item ratings to predict rating for unseen items.



### Model-Based Collaborative Filtering

Trains a model to recommend unseen items.



## Content-Based Recommendation

Recommends items by matching item features (e.g., genre, text, metadata) with a user’s profile built from their past interactions.



## Hybrid Recommendation

Combines collaborative filtering, content‑based, and sometimes other techniques to offset the weaknesses of individual approaches.



## Multi-Modal RS

Incorporates different modalities (text, images, audio, etc.) along with user–item interactions to enrich recommendations.



## Ensemble-Based RS

Combine the outputs of multiple models (or algorithms) into a single, robust recommendation.



## Graph Recommendation

Models users, items, and their interactions as a graph, then leverages graph algorithms (or graph neural networks) to generate recommendations.



## Knowledge-Based Recommendation

Uses specific domain knowledge about item features, users needs and preferences.

### Case-Based recommendation

Matches current user needs with past “cases” or experiences.



## Constraint-Based Recommendation

Generates recommendations that satisfy explicit constraints (e.g., budget, technical specifications) often needed for complex or high‑involvement products such as financial services, cars or real-estate.

Example: [Constraint-Based Recommender Systems](https://web-ainf.aau.at/pub/jannach/files/BookChapter_Constraint-BasedRS_2015.pdf)



## Sequential Recommendation

Takes the order of user interactions into account to predict next item a user is likely to engage with.



## Package RS

Recommends not one product, but a combination of items.

Also known as **bundle recommendation**.

Example: [Package recommender systems: A systematic review](https://research-portal.uu.nl/en/publications/package-recommender-systems-a-systematic-review)



## Next-Basket Recommendation

Predicts the next “basket” or group of items a user will purchase, focusing on the sequential nature of shopping.



## Session-Based Recommenders

These recommender systems use only the interactions of a user within a session to generate recommendations. In contrast to traditional recommendations, users have very short item history and their preferences have to be learned on the fly. The user ID is not used because a session replaces a notion of a user.

In case, where we want to make recommendations for the session but also have the user ID and access to additional information it is called **Session-Aware Recommendation**.



## Interactive RS

Continuously update recommendations in real time as users interact with the system, adapting to immediate feedback.



## Conversational RS

Engage in a dialogue with the user (via chat or voice) to iteratively refine and generate recommendations.



## Recommendation Editing

Allows post‑processing adjustments to recommendation lists (e.g., removing unsuitable items) without retraining the whole model. Also known as **Critiquing-based** recommender.

Example: 
- [Better Late Than Never: Formulating and Benchmarking Recommendation Editing](https://arxiv.org/pdf/2406.04553)
- [Critiquing-based recommenders: survey and emerging trends](https://link.springer.com/article/10.1007/s11257-011-9108-6)



## Active Learning in RS

The system proactively queries users (e.g., asking for ratings or feedback on specific items) to improve its understanding of their preferences.

## Group Recommendations

Generates recommendations for a group by balancing and aggregating the diverse preferences of all members.



## Reciprocal Recommendations

Recommends users to one another (e.g., in dating or job matching) by taking into account the preferences and suitability of both sides.



## Diversification in RS

Used when the quality of recommendations is not the only thing we need, but we also want recommendations to be diverse.



## Calibrated Recommendations

A diversification method that adjusts recommendation lists so that the distribution of recommended item types (e.g., genres) matches the user’s diverse tastes.



## Multi-Interest Recommendations

Learns multiple representations (vectors) per user to capture the variety in their tastes.



## Intent-Aware Recommendations

Tailors recommendations based on the specific intent behind a user’s current session (e.g., “go fishing” vs. “buy a gift”).



## Cross-domain RS

Transfers user preferences learned in one domain (e.g., music) to improve recommendations in another (e.g., movies).



## Reinforecement Learning in RS

Treats recommendation as a sequential decision‑making problem, optimizing for long‑term engagement or reward signals.



## Multi-Criteria RS

Incorporates multiple factors (e.g., quality, price, style) into the recommendation process rather than a single overall score.



## Multi-Stakeholder Recommendations

Balances the sometimes conflicting interests of different parties (users, providers, advertisers, etc.) when making recommendations.



## Context-Aware Recommendations

Also known as Context-Based Recommendation. A class of recommendations that take additional information into account such as the time of day, location, device, mood etc. 



## Risk-aware RS

Incorporates risk factors (e.g., avoiding recommendations during inappropriate times) to minimize potential negative impacts on users.



## Mobile RS

Designed specifically for mobile environments, taking into account mobile-specific factors like location, screen size, and intermittent connectivity.



## Location based Recommendation

Uses geographic data to recommend items that are relevant to the user’s current or desired location.



## Time-aware Recommendation

Incorporates temporal dynamics—such as seasonality, trends, or time‑of‑day effects—into the recommendation process.



## Emotion-based Recommendation

Also known as **Sentiment-based recommendation**. Tailors recommendations based on the user’s current emotional state or sentiment, which can be inferred from text, speech, or facial expressions.



## Social RS

Leverage social network data — such as friendships, trust, or influence — to inform recommendations.



## Trust-centric Recommendation

Weights recommendations by incorporating trust metrics (e.g., trust scores between users) so that more trusted opinions have greater influence.



## Trigger-Induced Recommendation

Generates recommendations in immediate response to a specific user action or external event (e.g., post-purchase follow‑up).

Example: [Deep Evolutional Instant Interest Network for CTR Prediction in Trigger-Induced Recommendation](https://arxiv.org/abs/2401.07769)



## Trustworthy RS

Focus on transparency, fairness, robustness, and explainability to ensure the recommendations are not only accurate but also ethical and unbiased.

Example: [Trustworthy Recommender Systems](https://arxiv.org/abs/2208.06265)



## Adversarial RS

Also known as **attack-resistant** RS. Include defenses against attacks (e.g., shilling, spam) by detecting and mitigating adversarial behavior in the recommendation process.



## Privacy-Aware Recommendation

Protects a user privacy (e.g., through differential privacy or federated learning) from a malicous attacker trying to steal private information via recommendations.

Example: [Privacy-Aware Recommendation with Private-Attribute Protection using Adversarial Learning](https://arxiv.org/abs/1911.09872)



## Fairness-aware RS

Implement mechanisms to ensure equitable treatment across different user groups and mitigate biases in the recommendations.



## Explainable Recommendations

Provide clear explanations for why items were recommended, helping users trust and understand the system’s decisions.



## Upselling Recommendations

Suggest higher‑end or premium versions of products to boost revenue while still fitting user preferences.



## Cross-Selling Recommendations

Recommend complementary products to what a user has already selected, enhancing overall user experience and sales.



## Quantum RS

Explores quantum computing techniques for recommendations, potentially offering speedups or new modeling capabilities.

Example: [Quantum Recommendation Systems](https://arxiv.org/abs/1603.08675)



## Other types by application

- Agriculture
- HR
- Tourism
- Fashion
- Food
- Music
  - Automatic Playlist Continuation
- Music events
- Multimedia
