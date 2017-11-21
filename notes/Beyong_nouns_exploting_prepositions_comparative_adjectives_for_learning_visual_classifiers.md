
Authrors propose a system for training the correspondence problem by exploiting additional language constructs to improve the learning process from weakly labeled data.
i consider both “prepositions” and “comparative adjectives” which
are used to express relationships between objects. If the models of such
relationships can be determined, they help resolve correspondence ambiguities.
However, learning models of these relationships requires solving
the correspondence problem. We simultaneously learn the visual features
defining “nouns” and the differential visual features defining such
“binary-relationships” using an EM-based approach.

1. It allows us to learn classifiers
(i.e models) for a vocabulary of prepositions and comparative adjectives. These
classifiers are based on differential features extracted from pairs of regions in an
image

2. Simultaneous learning of nouns and relationships reduces correspondence ambiguity and leads to better learning performance

3. Learning priors on relationships that exist between nouns constrains the annotation problem and
leads to better labeling and localization performance on the test dataset.
