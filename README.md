# My Git Practice README

## Interesting Article

[LLM-based feature generation from text for interpretable machine learning](https://link.springer.com/article/10.1007/s10994-025-06867-1)
— Balek, Sýkora, Sklenák & Kliegr, *Machine Learning* (2025)

I found this article interesting because it tackles a problem I've run into
directly: text representations like embeddings or TF-IDF are great for
predictive accuracy but terrible for interpretability — you can't easily
explain *why* a model made a decision when its input is a 768-dimension
vector. The authors use an LLM (Llama2) to turn raw text into a small set
of human-readable features instead, like `rigor = high` or
`replicability = yes`, extracted straight from an abstract. These features
can then feed into simple, explainable models like rule learners, instead
of black-box classifiers.

What stood out most was their use of **action rules** — rules that don't
just classify an article, but suggest a specific, actionable change (e.g.
"if replicability goes from no → yes, evaluation moves from bad → good").
That's a genuinely useful bridge between prediction and recommendation,
and it made me think about how similar LLM-extracted, interpretable
features could apply to other domains, like flagging risky pull requests
or explaining code review feedback in plain language instead of just a
similarity score.

<<<<<<< HEAD
## Comment by Rania Aamer

I think being able to understand why a model makes a decision is really important. Features like rigor and replicability seem easier to understand than a long list of numbers. I also wonder what happens if the LLM extracts a feature incorrectly. Would the final explanation still sound convincing even though it is based on a mistake? It would be interesting to see how the authors check the accuracy of these features.
=======
## Sean Kim's Thoughts

I thought that your article was interesting because it focuses on practicality and making large hard to understand numerical values more easier to process. I also like the idea of interpretable features for more than just predictions.
>>>>>>> pr-1
