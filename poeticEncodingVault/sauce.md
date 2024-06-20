**_1. Deep Learning, Literature, and Aesthetic Meaning_**

The central proposition of my dissertation is, informally, ‘it’s possible to learn a way of seeing by examining a group of objects that this way of seeing sees the best.’

I take my cue from how compression-based representation-learning neural nets (what AI researches would call ‘[autoencoders](https://medium.com/@peligrietzer/excerpt-from-a-literary-theorists-guide-to-autoencoding-582df5c3e025)’ in a broad sense, from RBMs to VAEs and two-way GANs) not only learn a low dimensional representation space, but also a projection from each point in input-space to some point in a low dimensional submanifold _within the input space._*****

[*****This geometrical description draws on the accepted practice of idealizing autoencoders with continuous input spaces and deterministic ‘pixel-independent’ decoders as non-linear dimensionality reduction algorithms. While the core ideas of this talk do carry over to autoencoders with autoregressive decoders, and in part even to pure autoregressive models like GPT architectures, the account becomes more complex.]

Speaking in rough terms, a trained autoencoder’s translation of an input object to its low dimensional representation space — the process of extracting an abstract, quasi-conceptual representation of the object — corresponds to taking the orthogonal projection of the input to a low dimensional submanifold in input-space, then taking the coordinates of the projection in a chart for this submanifold. I argue that there is a useful sense in which a sample from a trained autoencoder’s manifold expresses the autoencoder, and that studying this computational phenomenon gives us a fruitful formal model for thinking about a work of art as the expression of a way of seeing or a worldview.

To get the analogy going, let’s consider four properties that hold for the set of points composing the manifold of a (non-degenerate) trained autoencoder:

1. It’s the set of all the inputs that the trained net can compressedly encode with zero loss.*
2. All input reconstructions by the trained net will replace the original input with an element of this set.
3. The objects in this set collectively exemplify a specific high-fidelity simplification of the objects generated by the distribution underlying the training data.
4. A neural net trained on this set as its input distribution will very quickly approximate the neural net that generated the set.******

[*The idea that aesthetic artifacts may be unusually compressible goes back to Andrey Kolmogorov and more recently Jürgen Schmidhuber.]

[******Property 4 constitutes an ‘original,’ though elementary, mathematical observation formulated in collaboration with mathematician Tomer Schlank. More precisely, we show that the sample efficiency of the output set is significantly higher than the sample efficiency of the training set.]

Speaking informally, the above properties almost explicitly describe art as we know it: an individual apprehends the world in a particular lossy way that is partly adapted to her formative environment, she produces a mimesis (i.e. interpretive reproduction) of the world that’s simpler than the world in a specific way that bears the mark of her particular lossy apprehension of the world, and other individuals can learn her apprehension of the world by trying to very exactingly apprehend the artefactual world she produced.***** I argue that this similarity is not an accident or even an analogy, and properties 1–4 plausibly give something close to a functional definition of an ‘aesthetic symbol:’ a concrete, sensate representation of an abstract worldview. Additionally, properties 1–2 taken together give a near-equivalence between producing a mimesis of the world and curating a selection of minimum-loss objects from the world, as two ways to construct an approximate sample from the image of a net’s projection function. This near-equivalence suggest a way to understand curation, installation, collage, and other Modernist practices that are not immediately mimetic as, nevertheless, concrete sensate representations of a worldview.

[*****Notice that the analogues here are a _single_ literary artwork and a _set_ of input-space points. I discuss my grounds for conceiving of a single literary artwork as a _set_ of points at length below.]

Why call the image of a net’s projection function a ‘concrete, sensate representation’ of the net’s representation space? Let _f(D_n)_ mean the output of an unsupervised learning algorithm _f_ trained on n samples from dataset _D_. It’s provable from fairly weak assumptions about _D_ and _f_ that for any reasonably large _m_, there is an _n<m_ such that _f(f(D_m)_n)_ ≈ _f(D_m)_.* By way of an intuitive example, we might think about a toddler who learns how to geometrically compress worldly things by learning to compress their geometrically idealized illustrations in a children’s picture-book. Let _m_ be the number of sunflowers, full moons, oranges and apples that a toddler would need to contemplate in order to develop the cognitive schema of a circle, and _n_ the number of geometrically idealized picture-book illustrations of sunflowers, full moons, oranges and apples that a toddler would need to contemplate in order to develop this same cognitive schema. The set of pictures in the picture-book is, on this model, an approximation of a sample from the image of the projection function of the cognitive scheme of a circle, functioning as an information-theoretically optimal sensate representation of the cognitive scheme of a circle.

[*****Experimenting in a minimalist setup where _f_ is a 30-dimensional one-layer symmetrical autoencoder, _D_ is the MNIST database of handwritten digits, and _D_m_ is the full 50,000 pictures training set, we found that _f(f(D_m)_n)_ ≈ _f(D_m)_ when n ≥ 2,000. In other words, for _f_ a 30-dimensional one-layer symmetrical autoencoder, _f(f(MNIST_50,000)_2000)_ ≈ _f(MNIST_50,00). By contrast, f(MNIST_2000)_ has almost double the test loss of _f(f(MNIST_50,000)_2000)_ or _f(MNIST_50,00)._ We also experimented with deep variational autoencoders, where optimization issues make it difficult for _f(f(D_m)_n)_ to perfectly match _f(D_m),_ but _f(f(D_50,000)_n)_ is nevertheless strongly superior to _f(D_n)_ when _n_ is small. For convolutional, variational architectures trained on Fashion MNIST, for example, we reliably found that when _n_ ≤ _5000_ replacing _n_ raw samples with _n_ reconstructed samples is equivalent to raising _n_ by 50%_._]

When dealing with cognitive systems that one can’t “crack open” — like the read/write-inaccessible cognitive systems of the human world, and unlike the digital systems built by machine-learning engineers — the image of a cognitive system’s projection function becomes the most direct accessible manifestation of its representation space, and the concrete (or, in the case of literature, imaginative) realization of this image by mimesis of the world becomes a key method for communicating this representation space to new cognitive systems. In fact, considerations from _n<m_ suggest a method for transferring high-fidelity compression schemas between agents, and a reason to believe that this method has a computational advantage over training each agent individually: assume a trained neural network _w_ that has a high-fidelity compression schema for a distribution _D_, and an untrained* neural network _v_ that we want to train to have a high-fidelity compression schema for _D_. Assume, now, for the sake of an analogy with humans, that the internal structure of the neural nets is read/write inaccessible. If _w_ and _v_ have broadly compatible architectures (i.e _w(D)_ ≈ _v(D)_), the efficient and reliable solution is to train _v_ on samples from _w_’s reconstructions of inputs from D, instead of training _v_ directly on samples from _D_. In learning to compress the image of the trained net _w_’s projection function, _v_ learns a projection function that closely approximates (on _D_) that of the trained net _w_.

[*Importantly, the actual cognitive-theoretic model I’m proposing deals with works of art as methods for communicating a compression schema to a learner that already has a moderately advanced compression schema to start with — i.e. a pre-trained nets whose representation space is low-dimensional relative to the input space but high-dimensional relative to _D_ — rather than as methods of communicating a compression schema to a blank slate learner, so it contains some further technical complexities, but the general principles remain the same.]

Building upon these observations, I construct a mathematically informed interpretation of a classic literary-theoretic thesis: ==t====hat a work of literature can effectively communicate an ineffably complex holistic understanding of the real world, which we might call the work’s ‘aesthetic meaning.’== While my discussion focuses on literature, these same considerations may also apply to works of art in other media, to the extent that one can (partially) interpret a given work of art as constructing or curating a specialized dataset.

I begin by arguing that we should treat the content of a literary work as, in part, a set of data-points in a cognitive input-space. Why should this be the case? The kind of pattern-recognition practices typical of literary or aesthetic reading, I propose, consistently call on the reader to discretize the work’s content into intercomparable data-points in order to appreciate the play of difference, repetition, and variation that makes up a literary work’s narrative and rhetorical progression: to appreciate a literary work aesthetically is, in part, to compare and contrast the various situations, objects, actions, places, characters, tropes, concepts, and images that vary over the work’s narrative and rhetorical course. The concrete imaginative content of a literary work is therefore, in part, a pattern-rich sequence of data-points in the reader’s representation space. On the analysis that I propose, the reader’s representation space acts as the input-space in an unsupervised representation-learning process that the reader carries out by studying the work’s concrete imaginative content. For the purposes of the current thesis, we put sequencing aside* and focus on the _set_ of intercomparable data-points associated with a given literary work.

[*We can reintegrate matters of sequencing into our theory of a work’s ‘aesthetic meaning’ by adding considerations of ‘curriculum learning’ to our analysis, or by identifying the work’s data-points with stages of a growing sequence as in a recurrent network. ]

One primary structure of meaning in a literary work, I argue, is the aesthetic unity of all the objects or phenomena spanned by the fictional or notional world that the work imaginatively constructs. The meaning of a literary work like Dante’s ‘Inferno,’ Beckett’s ‘Waiting for Godot,’ or Kafka’s ‘The Trial,’ we would like to say, lies at least partly in an aesthetic ‘vibe’ or ‘style’ that we can sense when we consider all the myriad objects that make up the imaginative landscape of the work as a kind of curated set. On the account that I’m proposing, a literary work like ‘Godot’ or ‘The Trial’ has an ‘aesthetic meaning’ to the extent that the compression schema (i.e. trained autoencoder) that solves locally linear unsupervised learning on the set of data-points that make up the work is also a compression schema for some real-life distribution _D_. More formally, we might state this as follows. Let _f(‘The Trial’)_ mean the output of an unsupervised learning algorithm _f_ trained on the data-points that make up the concrete imaginative content of ‘The Trial.’ To the extent that _f(‘The Trial’)_ ≈ _f(D_m)_ for some non-trivial real world distribution _D_ such that _m>|’The Trial’|_, I argue, the compression schema optimal for the data-points of ‘The Trial’ is a robust form of ‘ineffably complex holistic understanding of the real world,’ and apt to play the role of ‘aesthetic meaning.’

A little more precisely, I identify the ‘aesthetic meaning’ of a literary work with the _input-space manifold_ equivalent to a compression schema (i.e. trained autoencoder) of the form discussed above. The several computational uses of this manifold, I argue in part **_2_**_._, each mirror an important literary-theoretic view of the cognitive use of ‘aesthetic meaning,’ and give a wealth of nuance to the relevant notion of an ‘ineffably complex holistic understanding of the real world.’

**2. _…With Applications to Modernist Studies_**

The proposition that a work of art can model the manifold structure of a real-world distribution is particularly useful as key to Modernist aesthetic theory and practice, in as much as Modernism is associated with a focus on abstract, diffused, ineffable structures of meaning bound to a work’s overall aesthetic form rather than on the more direct fruits of a work’s narrative, rhetorical, and lyrical communication. Specifically, the concept of a trained autoencoder’s manifold provides a strong conceptual interface between three major critical approaches to Modernist works’ ‘abstract, diffused, ineffable’ structures of meanings. The three approaches that concern us are as follows:

**A)** A cultural-Phenomenological approach to Modernist works as portraits of moods or ‘Stimmungen’ (subjects’ representation-spaces), nowadays very actively at play in literary studies. _(cf. Sianne Ngai, Jonathan Flatley)_

[Simplified: a Modernist work aims to demonstrate a way of looking at the world.]

**B)** A formalist-materialist approach to Modernist works as algorithms for the aggregation of textual or cultural materials that together form some weak field of coherence, central to the theory and practice of (speaking real loosely here) ‘conceptual writing.’ _(cf. Tan Lin, Hugh Kenner)_

[Simplified: a Modernist work aims to demonstrate a weak affinity between the many heterogeneous worldly or textual materials it patches together.]

**C)** The Symbolist approach to Modernist (Symbolist) texts as invocations of the ‘correspondences’ or ‘esoteric affinities’ that structure the perceptible surfaces of the world in accordance with ‘primordial Ideals’ that govern the ordinary world of visible phenomena. Associated with the early Modernist writers themselves more than literary studies. _(cf. Charles Baudelaire, Gertrude Stein)_

[Simplified: a Modernist work aims to demonstrate an underlying structure in phenomena that seem unstructured.]

On my account, each of these paradigms identically identifies the ‘meaning’ of a Modernist work with a trained autoencoder’s manifold, _describing one and the same formal structure via different functional definitions_. (Elsewhere, in work geared to the literary theorist, I relate this multifunctionality to Raymond Williams’ appropriately tricky concept of ‘structures of feeling.’)

The integrated story of our three ‘Modernist paradigms,’ under the manifold interpretation, can be told roughly as follows. To begin, let us recall that in unsupervised representation learning, we take a large set of data and learn a set of features that allows us to compressedly represent each piece of data in the set with minimal loss. We can regard this set of features as a ‘mental language,’ in a certain strictly heuristic sense: a trained net’s low-dimensional representation is functionally comparable to sequences of qualified predicates — e.g. ‘somewhat _p_, not _f_, not _q_, barely _t_, very _g_…’ — such that the predicates stay constant from input to input but the qualifiers vary. To the extent that a deep dimensionality reduction is appropriate for some given dataset, the ‘vocabulary’ of the language must approximately track the factors of variation entangled in the data. The features, in other words, must more or less correspond to something like ==Plato’s objects== ==whose ineffably interacting shadows on the cave’s wall are the data==. At the same time, to the extent that a deep dimensionality reduction is appropriate for some dataset, the ‘semantics’ of the resulting ‘vocabulary’ is also likely to be highly non-modular, analytically intractable, and “situated.” With these considerations in mind, calling the features learned in deep dimensionality reduction ‘_esoteric affinities of perceptible surfaces to primordial Ideals_,’ as in **C**, requires little if any poetic license.

Let us also recall, now, that the feature list extracted by unsupervised deep learning is equivalent to a coordinate system on a lower-dimensional manifold in the input space, such that given the feature list we can efficiently ask of new data whether it lies close to this manifold, and with certain further allowances even generate random new data that lies on this manifold. While points on this manifold are not necessarily _similar_ to one another, they collectively have an _affinity_ to one another: as objects generated from the same highly constrained generative ‘language,‘ they share at least of some minimal form of what we might tentatively call a ‘style’ or ‘vibe’ or ‘genre.’ Equivalently, any sufficiently large — relative to the learning algorithm’s complexity — set of datapoints covered by the manifold has an unusually low absolute Kolmogorov complexity (i.e. has high compressibility), a condition which most sciences regard as necessary, but only ambiguously sufficient, for possessing a “meaningful structure.” These structures of affinity are the kind of promising but in and of themselves _‘weak’_ fields of coherence that we know from ‘**B**.’

Finally, recall that once the training of an unsupervised deep learning algorithm is finished, when the algorithm encounters new input data it projects the data into the lower-dimensional manifold (within the input space) corresponding to the feature list. The algorithm ‘keeps’ only the aspects of the data that are captured by the feature list, then treats these feature values as coordinates on the manifold, and then picks the corresponding item on the manifold as the reconstruction of the input data. I propose that quite apart from any implication that a trained unsupervised deep learning algorithm is a good overall analogue for the mind of a human subject, we have good (if provisional) grounds to hold that the problem of locally linear dimensionality reduction is a staple of the “ecological niche” humans and learning algorithms for ‘AI domains’ share. If this is so, then we sometimes have reason to regard a person whose cognition is sensitive to some patterns in the world around her and insensitive to others— a person who excels at seeing certain similarities and differences but erases others — as projecting the worldly things she encounters into a lower-dimensional manifold spanned by her already-trained mental ‘language.’ On this account, we might treat the lower-dimensional manifold we’re learning when our minds are doing a dimensionality reduction on the data in e.g. a Modernist novel as a “reverse engineering” of the lower-dimensional manifold covered by the author’s or narrator’s ‘mental language’ (i.e. feature space). Or better yet, we might treat this manifold as the ‘mental language’ of a new way of seeing for which the novel’s aesthetic meaning is a blueprint. We have arrived, in any case, at one form or another of a _Stimmung_ as in ‘**A**.’

Let’s sum up. I propose that Modernist works are often in the business of teaching you the coordinates of a lower-dimensional manifold in the space of possible data. When we look at the three paradigms for thinking about the cognitive product of Modernist works, ‘**C**’ (’Ideals’) treats learning the manifold as learning the generative model of the data, ‘**A**’ (’Stimmung’) treats learning the manifold as learning the dimensionality reduction method that produced the data as ‘reconstructions’ of other data, and ‘**B**’ (’weak coherence’) treats learning the manifold as learning that a certain set is compressible. In other words, the same thin twisty slice in the input space can be interpreted as the expression of someone’s dimensionality reduction method (re: Stimmung), or as a set of objects that compress together well en masse (re: weak fields of coherence), or as a set of objects such that the difference between any object y and any object x is a principled difference (re: primordial Ideals).