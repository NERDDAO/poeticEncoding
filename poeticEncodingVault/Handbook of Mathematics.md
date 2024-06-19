Running in Shackles: The
Information-Theoretic Paradoxes of Poetry
34
Dmitri Manin
Contents
Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
The Form Paradox . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
The Nonsense Paradox . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
The Curious Case of Missing Synonyms . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
A Word in Its Place . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
Beyond Entropy . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
Conclusion . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
References . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .

## Abstract
Information theory developed by Claude Shannon in the 1940s provides a simple,
but powerful model for reasoning about communication that far transcends the relatively narrow technical domain of telecommunications, for which it was nitially developed. The use of language for exchanging messages is, arguably, the most distinctive feature of Homo sapiens as a species. Language is central for almost everything we do, and among many different ways language is used, poetry is perhaps the most enigmatic. Poetry is an ancient invention and never went out of fashion, but the reasons for its existence and the mechanisms of its impact remain elusive. Does information theory have anything to say about poetry? If poetry is often conceptualized as a message with highly concentrated
meaning, can it be proven that it has high information content? Attempts to answer these questions in the past 60 years that we review in this chapter are rich with important insights and nagging paradoxes.

## Keywords
Autoencoders · Entropy · Formal constraints · Information · Kolmogorov complexity · Meter · Metaphor · Poetry · Rhyme · Redundancy
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
Shannon’s guessing until the correct answer is obtained), which doesn’t provide a
way to compute entropy estimates. But the guess rates of 40% in poetry, 67% in
newspaper, and as high as 71% in conversation suggested an elevated entropy for
the poetry.


Other estimates of the natural language entropy, both using Shannon-style
experiments and statistical text analysis, can be found in Burton and Licklider
(1955), Paisley (1966), Kolmogorov (1968), Cover and King (1978), Kontoyiannis
(1996/1997), Pereira et al. (1996), Teahan and Cleary (1996), Moradi et al.
(1998). In some of these works, attempts have been made to correlate information-
theoretical characteristics of texts with their style and literary quality. However,
for the most part, such studies were motivated by practical applications like text
compression. The only systematic study of entropy as a function of style, period,
and author that I am aware of is Paisley (1966). Though it employed a very crude
entropy estimate (by frequencies of two-letter sequences), a systematic difference
was found between prose and poetry texts, the latter having higher entropy, i.e.,
information density, in agreement with expectations.


However, if we attempt to naively apply information-theoretic concepts to poetry,
two paradoxes immediately arise. First, the constraints of poetic form, such as meter,
alliteration, and rhyme, restrict the pool of words that can fill a given place in the
line and so should decrease unpredictability and entropy, rather than increase it. Call
this The Form Paradox. Second, according to Shannon’s theory, the highest entropy
is found in a completely random character sequence, where all characters occur with
equal frequency and independently of each other. But a random sequence of letters
(or words) can’t form a meaningful text, so it’s not even clear in what sense it can be
treated as containing information. Call this The Nonsense Paradox. We will consider
them in the following two sections.

## The Form Paradox

Fónagy (1961) noted that rhythmical and phonic organization of poetry should, it
seems, decrease unpredictability and entropy, contrary to his experimental results. In
the same collection where that article was published, we find a short, but insightful,
article by Abernathy (1961) where the same idea is put in this striking way:
“poetry uses a considerably circumscribed and impoverished language compared
to the everyday speech.” Abernathy proposed to resolve this paradox by ascribing a
subjective probability to each message and postulating that poems are characterized
by a drastically lower probability, i.e., higher unexpectedness, despite the fact
that they use “a considerably circumscribed” language. Unfortunately, this is a
rather nonconstructive approach, since it is not clear how to ascribe probabilities
to texts, and, more importantly, why or whether lower probability would result from
satisfying formal restrictions.

A much more detailed exploration of this paradox is due to A.N. Kolmogorov, a
great mathematician with a deep interest in literature. In a series of unpublished (at
the time) works popularized by Lotman (1977) (see also Kolmogorov, 1997; Yaglom
and Yaglom, 1983), he was developing a formalized approach based on considering
a set of all possible texts and a particular poem as a member of this set. A poet can
be seen as selecting or finding the text that expresses the desired meaning and at the
same time satisfies some formal constraints.  As an illustration, consider the set of all character sequences, say, no longer than War and Peace. It is a very large, but finite, number. There would be in this set a small subset of grammatically correct and meaningful Russian texts. In this highly idealized model, we don’t care what exactly the “meaning” is, but we postulate that each character sequence has either no meaning or exactly one, and that given any two “meanings” we can always say whether they are the same or different. Subdivide all texts into equivalence classes by synonymy, so that each class contains texts that all mean the same. In other words, each class would express in all possible ways
some content different from that of the other classes. Consider the synonymy class
in which all texts express the meaning of, say, Eugene Onegin. If this class is large
enough, one can find in it a text that is composed in Onegin stanzas, which is what
a poet does. Then the number of synonymy classes would be equal to the number of meanings expressible with texts no longer than War and Peace, and the average number of
texts in each class is essentially the number of different ways to express any given
meaning. According to Kolmogorov, the former quantity (or rather, its logarithm)
reflects the “content capacity entropy” of the language (h1 ), while the latter one
reflects its “flexibility entropy” (h2 ). If the flexibility entropy is large enough, i.e.,
if the given content can be expressed in a large enough number of ways, one can expect to find among those ways some that also satisfy the formal restrictions of
versification. Because formal constraints reduce the pool of admissible texts, they
can be characterized by a negative entropy (β), and Kolmogorov proposed that
versification is only possible in languages where β < h2 . Of course, one can’t get rid of the feeling that something is wrong in this picture.  Cf. the uncharacteristically impressionistic passage in a classical text on probability and information (Yaglom and Yaglom, 1983, p. 214):
However, in the compositions of many eminent poets the decrease in the information content of one text letter, related to the fulfilment of known formal rules, is apparently compensated for to a great extent by the enhanced radiance and unconventionality of language. Therefore, it can be well expected that here the redundancy of the language has the same order as that of a prose literary text.  I suppose Kolmogorov felt that way too, which is why he apparently never published his model. In fact, in an undated manuscript (Kolmogorov, 2002) first published by Uspensky (2002), he wrote: “Poetry admits somewhat freer use of word order unconventional in prose, which somewhat increases [the flexibility entropy].” This essentially means that the basic notion of the set of all admissible
texts is somewhat fuzzy: what is barely admissible in prose can be quite admissible
in poetry. But if the statistical population is not well defined, probability and,
hence, information are also ill-defined. One can even surmise that it was this train
of thought that eventually led Kolmogorov to propose his algorithmic complexity
theory. There is a telling remark in his groundbreaking paper (Kolmogorov, 1968)
after the introduction of what is now known as Kolmogorov complexity: “such
quantities as the ‘complexity’ of the text of ‘War and Peace’ can be assumed to
be defined with what amounts to uniqueness.”  Uspensky in his preface to the publication of Kolmogorov’s notes (Uspensky, 1997) also admits that “the very notion that the corpus of literary texts is only a subset of the corpus of meaningful texts” requires rethinking and gives an example of the famous nonsense line from a poem by the Russian modernist
poet Kruchenykh, consisting of three meaningless monosyllabics “Dyr bul shchyl”
(Perloff, 2017, p. 73). Note, however, that while Kolmogorov pointed out the
relaxation of syntactic norms in poetry, Uspensky’s example hints at the possible
relaxation of semantic norms. In fact, such relaxation is well-known to literary scholars. We are used to the notion of metaphor as a specific feature of poetry and literary prose, but most  metaphors are literally absurd phrases, inadmissible by the standard semantics of
the language, as one can see with any textbook example like “the curtain of the
night fell upon us” or “Juliet is the sun.” So it’s easy to see that metaphor (as well as
metonymy and other tropes) already serves to expand the space of admissible texts
in the semantic dimension. \

As for syntactic expansion, an obvious example is the word order violation often arising from the demands of poetic form. However, not all syntactic oddities arise for purely technical reasons. Many figures of speech known and meticulously catalogued at least since antiquity are particular ways to enhance expression by violating rules of syntax. Consider, for example, the opening of G.M. Hopkins’1006 D. Manin
poem “To His Watch”: “Mortal my mate. . . ” (Hopkins and Blaisdell, 2013, p. 84).
From the point of view of rhythm, the standard word order, “My mortal mate,”
wouldn’t be any inferior, but Hopkins forcefully emphasizes mortality, the theme of
the poem, by shifting the word to the syntactically awkward initial position.
To summarize, it appears that although poetic form does narrow down the
statistical population of all admissible texts, various poetic devices counteract
by expanding it and by pushing the boundaries of the standard language syntax
and semantics. In this way, they keep the language of poetry from becoming
“considerably circumscribed and impoverished” (Abernathy, 1961) and prevent
entropy reduction.
## The Nonsense Paradox

Suppose that armed with information theory we decided to construct a poem with
the highest possible information content. That requires each next element of the text
(whether we consider it composed of letters or words) to be the most unpredictable.
It’s easy to demonstrate that maximum entropy in a sequence is achieved when
every element is independently drawn from a uniform random distribution. But such
“text” would be nonsensical. How can nonsense have any information content, let
alone maximum information content?  To untangle this problem, recall that Shannon’s theory was formulated in the context of reversible transformations of symbolic sequences, such as encoding and decoding. If we compress the text of War and Peace using any standard algorithm like LZ77 (e.g., Dumas et al., 2015), we get a seemingly random character sequence where all characters appear at roughly the same rate and independently of each
other (in statistical terms). However, a decoding transformation exists that can be
applied to this sequence to recover the original text. That means that however one
defines the “content” of a text, it remains intact in the compressed form, and since
the compressed text is shorter than the original, its information content is higher.
What makes such compression possible is that the elements of a natural language
text are not equiprobable and, more importantly, not independent. Compression is
possible for a sequence whose entropy is lower than the maximum achievable with a
given alphabet. The relative deficit of entropy is called redundancy (Shannon, 1948).
An important role of redundancy, as also discovered by Shannon, is error correction,
i.e., redundancy makes it possible to reconstruct the signal, if it is distorted by noise.
Obviously, natural language needs a fair amount of redundancy, because it evolved
in an environment where quite literal noise often interferes with communication.
So, as is well-known, n nglsh txt wth ll vwls rmvd s stll mstl rdbl, because not all
letter combinations are pronounceable and not all pronounceable combinations are
meaningful words. Syntax also contributes to the redundancy of natural texts: some
word sequences (in fact, a great many of them) are grammatically invalid. And a
third major component of redundancy comes from semantics: most syntactically
correct sentences would be meaningless and so highly unlikely to occur in reality.
So, with reversible text transformations, there is no paradox. Problems begin
when we notice that not all interesting text transformations are strictly reversible.
For example, when Shannon discusses the translation of Finnegans Wake into Basic
English, it is fairly obvious that such a translation can’t be done in such a way as
to ensure that the reverse translation would exactly recover Joyce’s text. In fact, it’s
highly doubtful that such a translation is even possible. Consider a typical sentence
from the novel (Joyce, 2012, p. 6):  Hurrah, thereis but young gleve for the owl globe wheels in view which is tautaulogically the same thing. The word “tautaulogically” is a playful misspelling of “tautologically” that echoes its own meaning of pointless repetition by making the second syllable into a copy of the first one. It would be possible to reproduce the pun or create an equivalent one in a translation into a different, but similarly unrestricted language.
But writing in Basic English, by its very definition, precludes one from using words
beyond its 850-word lexicon. One could explain the pun in Basic English, but that’s
not the same as translating it, i.e., creating an equivalent text that could function in
the same way as the original one. Of course, James Joyce’s creation is an extreme example. But with respect to literary texts in general, it’s not uncommon to encounter the notion that they can’t be paraphrased, because changing any element would irreparably alter the text and change its meaning. That’s what Leo Tolstoy meant when he famously remarked
that in order to explain the message of Anna Karenina, he would have to write the
novel again. Semiotician and literary scholar Yuri Lotman wrote (Lotman, 1977):
the reader considers the text placed before him (if we speak of a perfect work of art) as the
only possible text; “you can’t throw a word out of a song”. For the reader the substitution
of a word in the text is not a variant of the content, but new content. Carrying this tendency
to its logical extreme, we can say that for the reader there are no synonyms.
Compare a very similar remark from a contemporary American introductory text
on poetics (Mandel, 1998): The selection of the right or best word or phrase in the right or best place is so delicate a task because — the exaggeration is minute — there are no synonyms. Let’s step back for a moment. The root of the Nonsense Paradox lies in the
different notions of “content” of a message in information theory vs our tentative
application. From the information-theoretic point of view, a character sequence is
the message, while with natural language, we have an intuitive notion of meaning
that is “contained” in the message and can be expressed in different ways. When
we consider writing a highly informative poem, we imply the most compact way
of expressing a meaning and so have to deal with the question of whether two
different texts express the same meaning. Information theory wasn’t designed to
deal with this notion of text synonymy. But note that we already encountered it
before, when we considered the Form Paradox: it arose in Komogorov’s model of
poetic composition. It’s worthwhile to look at it in more detail.


## The Curious Case of Missing Synonyms
The natural language possesses huge paraphrasing capabilities. The same meaning
can be expressed in many different ways (in particular, this sentence can be regarded
as a paraphrase of the previous one). This property seems to play an important role
in composing literary texts, especially poetry, by allowing us to select out of all texts
expressing the desired meaning, the one that also satisfies some requirements to its
form. Except, if we are to believe philologists, it doesn’t, because changing even
a single word would alter the meaning. Even making an allowance for the obvious
hyperbolicity of those claims (because, of course, some words in most poems can
be altered without completely changing the poem), it’s clear that there’s something
important lurking here. Where does the powerful paraphrasing ability of natural
language disappear, or at least, why is it significantly reduced, when we deal with
poetry? And, how is this related to the expressive power of poetic language?
According to Lotman (1977), the lack of textual synonymy plays a crucial role in
poetry: if every poetic text has a different meaning, that implies that they open up an
enormous space of new meanings. In terms of Kolmogorov’s model, if we reduce
the flexibility entropy to near zero (each synonymy class has only one element),
that increases the content entropy, if their sum is still equal to the total language
entropy. The value of poetry, then, is not that it can express any given meaning in an
especially economical way but that it can express meanings otherwise inexpressible.
The way Lotman explains this effect is by postulating that there are two different
ways to perceive a text: from the author’s and from the reader’s points of view. The
reader is given an immutable, finished work of art and tends to read significance into
every word choice, every sound of it. In that sense, the entire entropy of the text is
the content entropy. On the other hand, from the writer’s point of view, the artistic
freedom is virtually unlimited. In the extreme case, one could say that any word
can be substituted for any other, in the same sense as Carroll’s Humpty-Dumpty
claimed that “When I use a word, [. . . ] it means just what I choose it to mean—
neither more nor less.” So for the writer, the entire entropy of the language is the
flexibility entropy.
It is not clear whether this boldly impressionistic view can be given a precise
meaning, but let us note that underlying here is again the idea that the norms
of the standard language can and should be violated or altered in poetry. For
the writer, the standard semantics of words becomes malleable and customizable.
For the reader, normally non-semantic features, like the sound of words or their
grammatical relationships, become vehicles of meaning. Lotman demonstrated in
his analyses of specific poems how phonemes can take on semantic meaning (unique
for each poem) by virtue of their recurrence in meaningful positions. Likewise,
Roman Jakobson analyzed the semanticization of grammatical structures in poetry
(Jakobson et al., 1987).
Another way to look at the text synonymy problem is, in Lotman’s words
(Lotman, 1977, p. 24):
The fact is that in numerous instances the receiver must not only decipher a message with the
help of a particular code, but must determine the “language” in which the text is encoded
The claim is, essentially, that each poem defines its own language, overlapping with,
but not identical to the standard, base language in which it is written. This is done
by overriding some syntax and semantics of the base language and replacing them
with the text-specific syntax and semantics. If so, it’s not surprising that textual
synonymy is significantly reduced.
But is it possible to somehow substantiate this view in a more scientific manner?
We’ll address this question in the next section.
A Word in Its Place
The notion that literary texts possess some special rigidity of structure is actually
rather commonplace and widespread, as expressed in the form of the Russian
proverb “you can’t drop a word from a song.” One can find literally dozens of quotes
from different cultural contexts that all express this feeling of “the right word in the
right place” in a remarkably consistent way, for example:
• There’s no dropping a word out of a song (Russian proverb).
• Not a line is drawn without intention. . . As Poetry admits not a Letter that
is Insignificant so Painting admits not a Grain of Sand or a Blade of Grass
Insignificant much less an Insignificant Blur or Mark (Blake et al., 2008, p. 560).
• Every word must be mandatory (Kharms, 2002, book 38, sheet 3).
• The poet’s conviction that nothing is left to chance in poetry refutes the
puerile reasoning of some literary scholars who think that “a poem may contain
structures that are not connected with its literary function and impact” (Jakobson,
1987).
• The selection of the right or best word or phrase in the right or best place is
so delicate a task because—the exaggeration is minute—there are no synonyms
(Mandel, 1998, p. 192).
Just as the degree of unpredictability can be measured directly by asking subjects
to guess words or letters in a text, the degree of this rigidity (word irreplaceability)
can be measured by asking subjects to assess whether a given word belongs to the
text or had been replaced. This idea was recently realized experimentally (Manin,
2011, 2012) in the form of an online literary game (in Russian), which yielded a
large amount of data over a considerable corpus of text fragments, both verse and
prose.
The results show that word unpredictability of typical poetry and of literary prose
lies roughly in the same range, just as it was predicted by Yaglom and Yaglom
(1983) (quoted in section “The Form Paradox”). As discussed above, words in
poetry are harder to guess because of the greater freedom of word selection and
combination in poetry compared to prose, but they are at the same time easier
to guess because of the constraints of meter and rhyme. As it turns out, these
two opposite forces are approximately of equal strength, so that their effects are
canceled. This is likely not a coincidence, but an indication that language dictates
a certain level of unpredictability. Texts that are too predictable sound banal, and
texts that are too unpredictable border on nonsense (which is, in fact, a playground
of much avant-garde literature).
But this begs a question: why would the poet bother to increase predictability
with unusual word combinations while at the same time decreasing it back to
where it was by following formal restrictions? Is anything measurably gained
in the process? It turns out that yes, poetry has a significantly higher measure
of constrainedness, a quantity indicating how easy it is for a reader to detect a
substituted word. One can view each word in a text as being constrained by its
environment via syntax and semantics. In poetry, though, words are also constrained
by other features of the text: rhythm (not necessarily meter), sound patterning (not
necessarily rhyme), and all kinds of semantic and grammatical echos. This is what
makes a poem into a rigid structure where each word uniquely fits in its place and
is hard or impossible to replace.
The dynamics of entropy (predictability, redundancy) becomes clearer, if we
invoke the error-correcting function of redundancy. Consider the simplest code
which achieves higher reliability in a noisy environment by simply doubling each
transmitted character. If any symbol is omitted in a message encoded this way, it can
be reconstructed with certainty. Hence, the extra characters carry no information.
Why then are they needed? Because they carry meta-information, a meta-message:
“this message was not corrupted in transmission.” The feeling of “the right word
in the right place” in a literary text can have a similar function, except that it is an
evidence that the message has been deciphered (understood) correctly.
Lotman’s idea of a literary text simultaneously carrying a message and defining
the language in which it is encoded is apt here. If the reader feels that all the words
are where they belong, this feeling is an assurance that the language was correctly
decoded. For this, the text must have sufficient redundancy. But poetry, as opposed
to prose, can transmit the meta-message via meter, as well as rhyme and other
formal devices, which are not usable for encoding the message proper. By shifting
the redundancy/predictability into these non-semantic domains, poetry frees up the
semantic resources of the text for transmitting the meaning, which therefore can be
made much denser.
If that is true, it means that formal constraints paradoxically increase information
content or rather open the possibility for such an increase. With some exaggeration,
we could say that the formal organization of the text helps us accept linguistic
constructs that would be impossible otherwise, those that expand the set of all
admissible texts. There seems to be a clear parallel here with the remarkable
result of McGlone and Tofighbakhsh (1999) who discovered that rhymed aphorisms
are perceived as being more true than their non-rhymed semantic equivalents
(while being equally comprehensible). Indeed, a rhymed saying has a higher total
redundancy than the unrhymed equivalent, which is subconsciously perceived as a
certificate of correctness, but this redundancy doesn’t come at the expense of the
meaning-carrying capacity.
In fact, the results of Manin (2012) make it possible to estimate the relative
magnitude of entropy redistribution between semantic and formal aspects of a poem.
The probability to guess a word is the product of two probabilities: to guess the word
length only (the formal part) and to guess the word, if its length is known (mostly
semantic part). So, the total entropy, with its logarithmic dependence on probability,
can be approximated as the sum of formal and semantic entropies. It turns out that
in prose, they are approximately equal, while in metered poetry, the formal entropy
is very low, which means that semantic entropy is at least twice as high as in prose.
Perhaps, it is one of the functions of great poetry to expand the set of all
admissible texts. “In order to be realized, poetry needs to transcend the boundaries
of language, needs a kind of ex-stasis” (Geide, 2006). As a counterpoint, consider
the following raw account, not mediated by theoretical thought, of how a new,
and otherwise inexpressible, meaning is actually created for the reader (listener)
when the poet “transcend[s] the boundaries of language.” Director T. Haynes (2007)
discusses Bob Dylan’s song I’m Not Here after which he named his film about
Dylan: There’s words that no one can ever decipher, that he is sort of filling in as he is singing. And in a way because it escapes linguistic logic and mastery it almost communicates more than it ever could if it was fully legible, readable. It’s sort of beyond words. 

## Beyond Entropy
Though the Shannonian paradigm eventually proved quite productive in its applica-
tions to literature analysis, it is not the only possible information-theoretic approach.
Kolmogorov complexity, which is roughly the length of the shortest program that
generates a given text, provides another interesting perspective. Quoting Manin and
Manin (2017) (see also Manin, 2003): A natural language message is usually treated as carrying information. But it also can be treated as a program that runs in the brain of the receiver and whose purpose is to create a certain mind state in it. This interpretation is particularly interesting for literary texts, especially poetry, because their purpose is not conveying information, but rather imparting an emotional state to the reader. It is customary to state that successful poetry compresses its language and, consequently, if one wants to fully explicate the “meaning” of a good poem, an extensive prose text has to be written. So perhaps the right way to conceptualize a great poem is to say that it represents a maximally Kolmogorov-compressed representation of the target mind state.  Note that because Kolmogorov complexity is not computable, finding the maximally compressed description of something – whether a target mind state or an image, a scene, and a situation being described in the poem – is necessarily a creative act, something that can’t be done with an algorithm (faster than brute-force enumeration). Although this idea seems quite speculative, a recent work by Grietzer (2017a,b) explores a closely related territory in a spectacularly concrete fashion. Grietzer’s main instrument is autoencoders, a class of machine-learning algorithms based on the neural network architecture. An autoencoder is “trained” on a large corpus of objects from a multidimensional feature space and “learns” a transformation that maps this input space into a low-dimensional representation space. In other words, a trained autoencoder embodies a compression algorithm. This algorithm is
reversible, so that any point in the representation space can be mapped back into the
input space, but it is also, generally speaking, lossy, i.e., the reverse mapping will
not necessarily reconstruct the original object exactly.

However, there is an important low-dimensional submanifold in the input space,
namely, the set of its points the trained neural net learned to project into. We can
call it the invariant manifold, because the objects belonging to it are compressed
by the autoencoder losslessly and can be reconstructed from their representations
exactly. A crucial property of the invariant manifold is that the best way to recreate
the same mapping in another autoencoder is to train it on the first autoencoder’s
invariant manifold. (Of course, when dealing with computer software, it’s easier to
just copy the trained state to another instance, but that only works for instances with
identical architecture.)  This is where art and literature come in. Everyone perceives the world by constructing an internal lower-dimensional representation of it. Only the most
important features of the objects and events are represented there. Some important
features are more or less shared by all people; others are defined by one’s unique
perspective and personality. So every human essentially embodies an autoencoder.
Suppose one wants to share one’s unique perspective on the world (or, rather, a
fragment of it) with others. The best way to do it is to publish one’s invariant
manifold (or, rather, a consistent piece of it) and let others train themselves on it.
This describes creating artwork and reading/viewing/listening to it.  Interestingly, this description seems to circumvent the non-computability prob-lem of Kolmogorov complexity, because instead of trying to find the shortest description of a predefined fragment of the world, the author takes an existing short description and constructs a fragment of the world best described by it. But of course, the analogy is somewhat broken at this point, because a work of art is not (usually) a literal fragment of the world, but a symbolic representation of it. Nevertheless, this looks like a very powerful paradigm with a great promise.
## Conclusion

Thinking about poetry and literature in general in terms of information theory turns
out to be surprisingly productive. Many centuries-old notions, as well as relatively
recent developments in the humanities, can be naturally integrated into a cohesive
paradigm. Moreover, recent technological developments make it possible to move
from informed, but informal speculation to verifiable, reproducible results that give
a solid ground to conclusions. Poetry emerges perhaps most importantly as language use that pushes the boundaries of standard syntax and semantics, expanding the set of all admissible texts. A poem can utilize highly unusual word combinations but still maintain a
comfortable level of total redundancy with rich patterning on phonic, morphologic,
and syntactic levels. This effectively increases its meaning-carrying capacity. The 
rules of the underlying language are relaxed and partially replaced with regularities
particular to this specific piece. Thus, a poem can be described as a message that to
some extent defines its own language. This in turn leads to the reduction of textual
synonymy and the feeling of every word fitting harmonically in its place, which
likely is an important component of aesthetic satisfaction.  We are still at the beginning of this journey, and one should expect many new developments in the years to come.