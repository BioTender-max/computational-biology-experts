# Bernhard Schölkopf — Anti-Patterns

Failure modes that Schölkopf's work explicitly or implicitly argues against.

## 1. Correlation as causation
Concluding that correlated variables are causally related without causal analysis. "The system does not recognize the cow since it only pays attention to correlations, ignoring causality." This is the fundamental failure mode of statistical learning.

## 2. i.i.d. assumption
Assuming the future looks like the past when distribution shifts are common. Statistical models trained on i.i.d. data fail under distribution shift. Causal models are robust to distribution shifts because they model the underlying mechanisms.

## 3. Hype extrapolation
Naively extrapolating from impressive results on benchmark problems to general intelligence. "Everything that's related to super-intelligence, I would say at this point, is hype." Genuine progress requires solving causal representation learning.

## 4. Industrial lab seduction
Abandoning academic independence for the short-term attractions of industry. "There's a reason why in the end many of the most surprising developments come from academia — I think it may be related to tenure." Industrial labs are less stable and less free.

## 5. Attention fragmentation
Allowing email and administration to crowd out deep thinking time. "I spend too much time on email. I would like to have longer uninterrupted stretches of time." Deep thinking requires long, uninterrupted stretches of time.

## 6. Narrow specialization
Working in only one field when machine learning is a universal tool. "You get to play in everyone's backyard." The mathematical framework is the same across domains; the applications are unlimited.

## 7. Statistical learning without causal structure
Building models that fail under distribution shift because they lack causal representations. The solution is causal representation learning — learning representations that correspond to the causal variables of the world.
