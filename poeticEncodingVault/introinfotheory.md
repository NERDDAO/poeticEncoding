## Introduction
From the very beginning of information theory, researchers were tempted to apply
it, even if informally or metaphorically, to literary texts, especially poetry. In his
groundbreaking paper, Claude Shannon (1948) wrote: Two extremes of redundancy in English prose are represented by Basic English [Wikipedia (2018) – DM] and by James Joyce’s book “Finigan’s Wake” [sic – DM]. The Basic English vocabulary is limited to 850 words and the redundancy is very high. This is reflected in the expansion that occurs when a passage is translated into Basic English. Joyce on the other hand enlarges the vocabulary and is alleged to achieve a compression of semantic content. Poetry is commonly described in terms of “economy of language,” “compression of meaning,” and so on. This notion even occurs in dictionary definitions, such as this one from the Merriam-Webster’s dictionary: “writing that formulates a concentrated imaginative awareness of experience in language” (Merriam-Webster online, 2018). So it seems that information theory must be able to contribute something to this intuitive notion that a work of literature can pack a lot of punch
in a short stretch of text. Indeed, the theory defines a measure of content, and if one
could demonstrate that poetry has more content per unit length (information density
or entropy) than nonliterary, utilitarian language, then that would be a proof of its
elevated expressive power. Shannon’s definition of information operationalized some of the intuitive notions that had been expressed long before. Without getting into technical subtleties, the amount of information in a sequence of symbols is a measure of its unexpectedness.  The amount of information per symbol (entropy or information density) 
where pi is the probability for the ith symbol to occur. If every symbol can be  predicted with certainty, the sequence has no information in it, in agreement with the intuitive notion. The way to increase the amount of information is to compose the message out of unexpected elements. For example, if we consider each word in the text as a “symbol,” the greater the vocabulary, the smaller these probabilities are on average, so the amount of information increases. Compare this with how Aristotle in his Poetics recognized the importance of unexpected elements: “That diction [. . . ] is lofty and raised above the commonplace which employs unusual words.” and “It is precisely because such phrases are not part of the current idiom that they give distinction to the style” (Aristotle, 2008, Part
XXII). As another reference point in modernity, consider Viktor Shklovsky’s theory of defamiliarization (ostranenie).

A writer and scholar of the Russian formalism school, Shklovsky, contended that our perception is dulled by habituation, and the goal of literature is to refresh it by presenting things in an unfamiliar, estranged way, in particular with language (Shklovsky, 2015): The language of poetry is difficult, laborious language which puts the brakes on perception. In some particular cases, the language of poetry approaches the language of prose, but this does not violate the law of difficulty. [. . . ] For Pushkin’s contemporaries, Derzhavin’s elevated diction was the usual language of poetry, so that Pushkin’s style was unexpectedly difficult for them in its ordinariness. Recall that Pushkin’s contemporaries were horrified by his vulgar expressions. Pushkin used the vernacular as a device to arrest attention [. . . ] Shannon’s definition allows us to actually compute some measure of unexpect- edness of a text’s language: either by using word frequency as an approximation to its probability or by asking human subjects to predict the next word (or letter) and estimating probability from the success rate on this task. There have been some attempts to do that early on. Shannon himself conducted the first experiments (Shannon, 1951), where a respondent was asked to guess the next letter in randomly chosen fragments of a Jefferson biography. Shannon was mostly interested in estimating the information rate itself and didn’t study differences between texts. Later, a number of researchers repeated and elaborated Shannon’s experiments.  Fónagy (1961) compared guess rate of the next character in three different texts: a poem, a newspaper article, and a “conversation of two young girls.” Apparently, he
used a simplified method, where each letter was guessed only once (in contrast to
Shannon’s guessing until the correct answer is obtained), which doesn’t provide a way to compute entropy estimates. But the guess rates of 40% in poetry, 67% in
newspaper, and as high as 71% in conversation suggested an elevated entropy for the poetry.


Other estimates of the natural language entropy, both using Shannon-style experiments and statistical text analysis, can be found in Burton and Licklider (1955), Paisley (1966), Kolmogorov (1968), Cover and King (1978), Kontoyiannis (1996/1997), Pereira et al. (1996), Teahan and Cleary (1996), Moradi et al. (1998). In some of these works, attempts have been made to correlate information-
theoretical characteristics of texts with their style and literary quality. However, for the most part, such studies were motivated by practical applications like text
compression. The only systematic study of entropy as a function of style, period, and author that I am aware of is Paisley (1966). Though it employed a very crude
entropy estimate (by frequencies of two-letter sequences), a systematic difference
was found between prose and poetry texts, the latter having higher entropy, i.e., information density, in agreement with expectations. 

However, if we attempt to naively apply information-theoretic concepts to poetry, two paradoxes immediately arise. First, the constraints of poetic form, such as meter,
alliteration, and rhyme, restrict the pool of words that can fill a given place in the line and so should decrease unpredictability and entropy, rather than increase it. Call
this The Form Paradox. Second, according to Shannon’s theory, the highest entropy is found in a completely random character sequence, where all characters occur with equal frequency and independently of each other. But a random sequence of letters (or words) can’t form a meaningful text, so it’s not even clear in what sense it can be treated as containing information. Call this The Nonsense Paradox.