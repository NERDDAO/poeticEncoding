2.2
A Defense of Poetry
When dealing with cognitive systems that one can’t ‘crack open’—like the read/write-
inaccessible cognitive systems of the human world, and unlike the digital systems built
by machine-learning engineers—the image of a cognitive system’s projection function is the
most direct accessible manifestation of its representation-space, and the concrete (or, in the
case of literature, imaginative) realization of this image by mimesis of the world becomes a
key method for inputing this representation-space to new cognitive systems. In fact, consid-
erations from n < m suggest a method for transferring (lossy) compression schemas between
agents, and a reason to believe that this method has a computational advantage over training
each agent individually: assume a trained neural network w that has a (lossy) compression
schema for a distribution D, and an untrained36 neural network v that we want to train to
have a (lossy) compression schema for D. Assume, now, for the sake of an analogy with
humans, that the internal structure of the neural nets is read/write inaccessible. If w and v
have broadly compatible architectures (i.e w(D) ≃ v(D)), the efficient and reliable solution
is to train on samples from w’s reconstructions of inputs from D, instead of training v di-
36
Importantly, the actual cognitive-theoretic model I’m proposing deals with works of art as methods for
communicating a compression schema to a learner that already has a moderately advanced compression
schema to start with—i.e. a pre-trained net whose representation-space is low-dimensional relative its ‘raw’
input-space but high-dimensional relative to the size of D—rather than as methods for communicating a
compression schema to a new autoencoder. While the general principles remain applicable, one crucial
difference has to do with the general learning-theoretic rule of thumb that an effective training set must be
large and diverse. On a ‘new autoencoder’ model, this rule would predict ‘rich’ Modernist works like ‘Ulysses’
or ‘Zorns Lemma’ or ‘Tender Buttons’ or ‘Ketjak,’ but disqualify ‘thin’ Modernist works like ‘The Making of
Americans’ or ‘The Trial’ or ‘7CV’ or ‘Blood and Guts in High-school.’ Things look very different, however,
when we consider what a training set designed to update only the connections between higher layers of a
network that already received a lot of broadly relevant training would be like: the training can now take
advantage of the network’s existing sophisticated similarity space to generalize from a prototypical instance
of an everyday concept to the rest of this concept’s (reasonably typical) instances, such that e.g. however
‘The Metamorphosis’ is training a reader to encode states of the Samsa family, after training the reader will
fairly similarly encode states of the Zamsa family, who are like the Samsa family but Dutch and have red
hair.
69rectly on samples from D. In learning to compress the image of the trained net v’s projection
function, w learns a projection function that closely approximates (on D) that of the trained
net v.
Building upon the above principle, we can construct a mathematically informed inter-
pretation of a kind of minimal romantic, Symbolist, Modernist working assumption: that a
work of literature can effectively communicate an ineffably complex holistic understanding
of the real world, which we might intuitively call the work’s ‘aesthetic meaning.’ On our
mathematically informed interpretation, one sufficient condition for romantic, Symbolist,
Modernist ‘aesthetic meaning’ is the sensible representation of an autoencoding manifold
in an intersubjective input-space, which we will call ‘ambient meaning.’ Not to feign inno-
cence, let us observe ahead of time that we will argue that at least some actually-existing
works of literature in fact construct ‘ambient meaning,’ and the minimal romantic, Sym-
bolist, Modernist working assumption is well-integrated with our best social-theoretic and
technoscientific understanding of the realms where it must operate. Our construction of this
‘mathematically informed interpretation’ will, in this sense, take more after the dialectical
form of a ‘defense’ (as in ‘Defence of Poetry) or an apologetics37 than after the dialecti-
cal form of disinterested scholarship. Where scholarship is predicated on commitment to a
specific engine of reasoning and a promise of disinterest in the end-result of reasoning—the
scholar goes where the unbiased application of her method leads—the stance of an apol-
ogy admits a prior commitment to a certain end-result, and seeks to demonstrate that this
commitment is compatible with certain prima facie challenging methodological commitment.
Moreover, the inevitably theological connotations of ’apology’ are especially apt here, since
reification of ‘romantic, Symbolist, Modernist’ forms of insight, sense, or meaning that are
37
We might consider Rita Felski’s ‘Uses of Literature’ or Caroline Levine’s ‘Forms’ as two contemporary
examples.
70not accessible to common sense or ordinary analytic thought is oftentimes associated with
what Rita Felski recently and accurately nicknamed ‘theological’ (3) accounts of literature.
In its capacity as an apology, this dissertation makes the case for literature’s ‘otherworldly
aspects’ (ibid) to the twice-materialist magisteria of social theory and technoscience: on our
account, the ‘otherworldly’ is an aspect of the natural and social world that is ‘foreclosed to
‘analytical’ and concept-driven styles of political or philosophical thought,’ (ibid) but whose
interactions with conceptual cognition and with everyday practical knowledge are abundant
and empirically tractable, and whose foreclosure is itself analytically and technoscientficially
explicable. While neither the form nor the substance of ‘ambient meaning,’ as we have it,
finds a place within the order of things as revealed by commonsense materialisms, the forms
and substance of ambient meaning are plausibly all but endemic to the language of a math-
ematically sophisticated technoscientific materialism, and to the language of an affectively
sophisticated cultural materialism.
The proposition that a work of art can model the manifold structure of a real-world dis-
tribution is, perhaps, particularly pressing in its relevance to Modernist aesthetic theory and
practice, in as much as Modernism is stereotypically associated with a focus on abstract,
diffused, ineffable structures of meaning bound to a work’s overall aesthetic form rather
than on more direct or local cognitive-affective fruits of a work’s narrative, rhetorical, and
lyrical communication. We will regard as ‘stereotypically Modernist,’38 for instance, the full
corpuses of Jarry, Woolf, Kafka, Maeterlinck, Roussel, Pound, TS Eliot, Stein, Musil, Bely,
Shklovsky, Benjamin, Khlebnikov, Kharms, Mishima, Beckett, Pinter, Ashbery, Saurraute,
Haroldo de Campos, or Robbe-Grillet, and of staple ‘proto-Modernist’ anchors like Büchner,
Melville, Lautreamont or Dickinson, as well as parts of later Goethe, Charlotte Bront, later
38
We of course use ‘stereotypically’ here in a value-neutral sense.
71Chekhov, and later Flaubert. While it is plausible, in my view, that ‘ambient meaning’—in
effect, the sensible representation of a systemic gestalt—is already an endemic aspect of ‘sen-
sible discourse’ as Baumgarten understood it in 1735, and that many or most literary works
in many or most literary canons function in part as holistic aesthetic symbols in the relevant
sense, our model nevertheless has a certain rich ‘elective affinity’ with Modernist, as well as
21st century ‘experimental,’ literary practices and literary thought. First, and most crudely,
an account of a given literary work’s ambient meaning plausibly explains more in the case
of a stereotypically Modernist work than in the case of, for example, a Regency novel. It’s
useful, here, to draw on Roman Jakobson’s conception of a literary work’s ‘dominant’: a
work’s subsuming semiotic structure, whereby a work’s non-dominant semiotic structures
operate as lower-order organizing principles downstream from the dominant’s logic. Even
rejecting, as we should, the rigidity of Jakobson’s idea of a perfectly teleological, means-end
relationship between a work’s various semiotic structures, it’s fair enough to say that from
among reliably salient organizing principles like rhetoric, narrative, lyricism, verisimilitude,
and holistic aesthetic symbolization, the logic of holistic aesthetic symbolization tends to the
condition of Jakobsonian dominance in the semiotic economy of a stereotypically Modernist
literary work. Whatever we believe about just how exhaustively e.g. ‘Bouvard et Pécuchet’
(or even ‘Le Dictionnaire des idées reçues’) or ‘The Making of Americans’ are optimized for
the sensible representation of a trained autoencoder’s manifold, there can be little doubt that
‘Pride and Prejudice’ comprises a wealth of aesthetically and ideologically salient semiotic
operations besides ‘ambient representation.’ Stereotypically Modernist works, on the other
hand, are often marked not only by structural subsumption, but also by zero-sum tradeoffs
whereby typically salient or pressing semiotic structures like plot, agency, logos or are broken
or matted to allow additional ‘degrees of freedom’ for the work’s holistic aesthetic symbol-
72ization structure. At the limit of stereotypically Modernist practice—‘Finnegans Wake,’
‘The Making of Americans,’ “‘A,”’ ‘Galáxias’—we are left with perhaps nothing other than
holistic aesthetic symbolization to hang our hat on.
The final point above is, perhaps, particularly relevant to this dissertation’s project from
a practical or dialectical perspective. While—for example—Tolstoy famously asserted that
the sense of ‘War and Peace’ is inextricable from the totality of ‘War and Peace,’ and while
I would propose that ‘ambient meaning’ as per our autoencoder model is a major aspect
of this total meaning in the case of ‘War and Peace’ perhaps no less than in the case of
‘Tender Buttons,’ an interlocutor may peacefully reject holistic aesthetic symbolization as
nonsense upon stilts and still believe that ‘War and Peace’ not only delights but instructs,
delivering many individually fine lessons about human nature through its piths and para-
bles. The bare assertion that ‘War and Peace’ plausibly yields substantive cognitive-affective
content doesn’t, on its face, present us with an explanundum that calls for a mathematically
augmented theory of ‘ideas in things.’ When dealing with a stereotypically Modernist work
of literature, on the other hand, ascription of substantive cognitive-affective structure nec-
essarily courts theoretical controversy. In fact, the question of the cognitive robustness of
stereotypically Modernist meaning-making even breaks away from the glorious isolation of
‘pure’ or transhistorical aesthetic discourse, and powerfully interpolates our theory of ‘am-
bient meaning’ into a dialectical relationship with what we might call the default Marxian
story of representation under late modernity, as we discuss below.
Marxian literary history, if there is a Marxian literary history, contends that under late
modernity the causal structure of social-material conditions of subjective life has become
too complicated to abide a narrative or lyrical representation, and modern literature has
therefore been increasingly unable to provide ‘cognitive mapping’ of the social-material con-
73ditions of subjective life. An ‘ambient meaning’ viewpoint on Modernist literary practices
accepts the Marxian literary historian’s premise while rejecting her conclusion, arguing that
the conditions of modernity do not necessarily diminish literature’s overall capacity to struc-
turally model social-material conditions, but perhaps modulate the capacity of narrative or
lyric tactics of cognitive mapping while amplifying the capacity of ‘ambient’ mapping strate-
gies. I have hinted above that the ‘default Marxian narrative’ about representation under
late modernity enjoys a certain pro tanto authority that is sufficient for putting ascriptions
of substantive cognitive-affective modeling capacities to stereotypically Modernist literary
work in the position of apologetics. The factors that determine our dialectical positioning
here are, perhaps, a contingency of the particulars of Anglophone literary-theoretic discourse
on forms,39 but they have nevertheless found reification through one more successful illocu-
tion in 20th century literary academia. Speaking at the now-legendary 1983 ‘Marxism and the
Interpretation of Culture’ conference, Frederic Jameson gave a keynote lecture called ‘Cog-
nitive Mapping,’ that will later become the foundation for the most heavily cited monograph
in literary theory:
’I am addressing a subject about which I know nothing, whatsoever, save for
the fact that it does not exist. [...] Since I am not even sure how to imagine
the kind of art I want to propose here, let alone affirm its possibility, it may
well be wondered what kind an operation this will be, to produce the concept of
something we cannot imagine.’ (347)
In his lecture, Jameson hypothesized a Marxian aesthetic of the future, called ‘the aes-
thetic of cognitive mapping,’ that is waiting to be born and as of yet unknowable. Declaring
39
As Caroline Levine observes, the systematic study of aesthetic forms in late 20th century literary theory
has been, for the most part, the domain of a single Marxian lineage.
74from the start that he has nothing to say about this yet-unborn aesthetic, Jameson left the
baptism itself to be the only anchor of the future aesthetic’s identity. And like a Catholic
Walter Shandy, Jameson set the fortunes of his unborn Marxian aesthetic for the next four
decades with the act of giving it a name. Naming the concept after a beloved senior rela-
tive from Marxian urban planning theory—the concept of ‘cognitive mapping’ in the work
of urban theorist Kevin Lynch, where ‘cognitive mapping’ denotes a city resident’s ability
to comprehend the spatial, social, and functional layout of her city as an integrated living
system—Jameson’s Marxian baptism proved at least the equal of its Roman-Catholic an-
tecedent in illocutionary force. All future talk of an aesthetic practice that is epistemically
constructive (not unlike a city resident’s cognitive mapping of her city), systems-minded
(not unlike a city resident’s cognitive mapping of her city), and holistic (not unlike a city
resident’s cognitive mapping of her city) was to become, at least partly by power of this
Jameson’s 1983 illocution, a claim on Jameson’s hypothesized ‘aesthetics of cognitive map-
ping.’ It should be obvious, then, that ascriptions of ‘ambient meaning’ to a literary work
are in some sense a claim on Jameson’s ‘aesthetics of cognitive mapping.’ While Jameson’s
lecture does steer clear, as promised, from describing what his ‘unimaginable’ aesthetics of
cognitive mapping might be like, Jameson does forcefully argue that there are no examples of
an actually-existing aesthetics of cognitive mapping—and therefore, on my terms, that there
are no actually-existing literary practices of ambient meaning-making. Moreover, Jameson’s
‘Cognitive Mapping’ lecture offers a rather thorough study of its namesake aesthetic via neg-
ativa, by recounting the Lukácsian story about literature’s loss of powers of representation
under the conditions of modernity.
On Jameson’s ‘Cognitive Mapping’ account, orthodox to what we might call the Lukács-
Jameson-Moretti school of Marxian literary theory, Modernist forms are primarily dramatic
75performances of epistemological desire, not good so much for the modeling of worldly systemic
structures and relations as for dramatizing (symptomatically or critically) modernity’s pro-
gressive crises of representation and of social knowledge. This dissertation both accepts—in
as much as every literary-theoretic enterprise operates from some implicit or explicit norma-
tive stance, and this is ours—the Lukács-Jameson-Moretti teleology wherein a literary art’s
success or failure as an epochal enterprise lies in its capacity to model systemic structures
and relations (not, let’s say, a literary art’s capacity for stirring passions, or for immersive
storytelling, or for free-play of the faculties), and rejects the Lukácsian tradition’s actual
diagnosis of late 19th - 21st century literature’s capacity to model systemic structures and
relation. By contrast with the Lukácsian tradition, the present work treats Modernist and
avant-garde forms not as epistemic dramas but as epistemic methods. This commitment
goes beyond objecting to the often caustic treatment of Modernist projects in the work of
Lukács, Jameson, or Moretti proper, and challenges a rather flexible and porous paradigm
associated with the rich diffusion of Jamesonian (Lukácsian) ideas in Modernist studies at
large. Where the work of Lukács, Jameson, or Moretti proper tends to cast Modernist forms
as tellingly miscalibrated readjustments of literature’s epistemic project to the objectively
contracting possibilities for social knowledge and representation, critics and theorists who are
broadly Jamesonian (Lukácsian) but sympathetic to experimental literary practices typically
defend Modernist forms as tactics of resilience, wherein literature lowers its representational
ambitions in the face of the objectively contracting possibilities for social knowledge and
representation in order to make the most of what can still be represented.40 By contrast
with even these (so to speak) Jameson-compatible defenses of Modernist representation, this
40
Sianne Ngai’s chapter on ‘stuplimity’ in ‘Ugly Feelings,’ a book which is otherwise an inspiration for
the present work in many respects, is a prototypical example of an account of Modernist forms as tactics of
resilience.
76dissertation’s point of view suggests that Modernist forms are not entirely a reconciliation
of literature’s epistemic ambitions to an epoch’s already-configured epistemic possibilities,
but also an invention or discovery of novel41 epistemic possibilities that epochal conditions
have made newly practicable, thinkable, or urgent.
From the viewpoint of Modernist studies, the theory of ambient meaning can propose
new possibilities for a concrete constructive account of the capacities of Modernist and
avant-garde textual forms for modeling social, psychical, and cultural-material structuring
structures: concrete, at first, in the high specificity of its recourses to social-theoretical
and cognitive-theoretical discourse when defining the semantics and epistemology of the
Modernism-friendly (to say the least) form of sensible representation that I call ‘ambient
meaning,’ and resultantly concrete in the high specificity of the relationship that it imputes
between the historical and formal vicissitudes of Modernist textual practice and the historical
and cognitive vicissitudes of making, sharing, using, representing, and scrutinizing mental
models of the social. Modernist forms, from this viewpoint, are concrete adaptations or de-
velopments in the technology of cognitive mapping—they are pragmatically sociohistorically
contingent42 methods for creating mental models of the structures and dynamics of phenom-
ena. While such a research program as described above is well beyond the purview of this
present effort, in the course of our study of ambient meaning we hope to give solid ground to
the hypothesis (redundant to some, hopeless to others, and therefore maybe relevant to all)
that Modernist and avant-garde forms are a viable, and sometimes vital, cognitive technology
41
Much like in the history of science, philosophy, or technology, we should read ‘invention,’ ‘discovery,’ or
‘novel’ so strongly as to suggest historical discontinuity or lack of antecedent.
42
We bracket the question of whether or to what extent the relevant form of sociohistorical contingency
is ideological in additional to practical. That is, it may or may not be the case that the rise of Modernism
was simply a function of ‘motive and opportunity’ for certain kinds of cognitive-aesthetic literary operations,
and it may or may not be the case that the rise of Modernism was a result of some ideological shift in the
criteria of truth, knowledge, representation and so on.
77for representing sensible systemic structures in a social-material.
Speaking in more literary-critical terms, we might say that the ‘ambient meaning’ view-
point treats Modernist form as a method of map-making, rather than as a map:43 I treat
abstraction, parataxis, fragmentation, indeterminacy, polysemy and polyvalence not as rep-
resentations of a psychological or cultural predicament but as methods of a process of cog-
nition. We will read radical fragmentation in a Modernist text, for example—all else being
equal—as part of the functional structure of a learning/teaching process that proceeds by
way of a curated field of heterogeneous objects to impute whatever representation of the
mind or the world, rather than as a representation of a fragmented mind or a fragmented
world. We thus partially detach the questions of Modernist form from questions about the
form of modernity, of the world-system, of our Worldedness or of Lukács totality—not in
order to deny the possibility of a deep epochal relationship between the cognitive and social
conditions of modernity and Modernist form, but to propose that this relationship is at least
in part mediated by the extent to which the conditions of modernity are especially enabling
of, or make a special necessity of, the cognitive work of producing ambient meaning. One
stance which this work does take on matters of form and epoch, however, is that every
degree of abstraction, parataxis, fragmentation, indeterminacy and polysemy is consistent
with every orientation towards social totality, social brokenness, capitalism, fragmentation
of society, affect, or what you will. In fact, I would suggest that it is something of a catas-
trophe of the academic Modernist canon that when we think of Modernist collage we think
43
In ‘Plurality in Question,’ Jackson instructively makes a complementary, ‘opposite’ point in a very
different context. Jackson observes that critics often read the typical rhetorical and narratological linearity
and rigidity of the contemporary Zimbabwean novel as imputing a linear, rigid world or worldview, and
takes issue with the reduction of the representational function of literary form to a direct analogy between
the discursive structure of a novel and the structure of a social-material totality. On Jackson’s account, the
narratological linearity and rigidity typical of the contemporary Zimbabwean novel is instead an aspect of
its functional form as a dialectical or argumentative novel, a novel whose structure constructs a particular
thesis rather than simulates a totality.
78only of Eliot’s ‘heap of broken images’ and not of Zukofsky’s ‘integral, lower limit speech,
upper limit music,’ or that when we think of parataxis we think of Tristan Tzara’s histrionic
nihilism but not of William Carlos Williams’s earnest repleteness.
There is a visible relation, one might notice, between our gloss on ‘stereotypically Mod-
ernist’ literature and what Marjorie Perloff’s ‘The Poetics of Indeterminacy’ famously called
‘the ‘other’ tradition’—a subtradition within Modernism that Perloff identifies (in poetry)
with Rimbaud, Pound, Williams, Stein, Ashbery, Beckett, and Cage, and against Baudelaire,
Mallarmé, Eliot, Stevens, Crane, and Lowell. Perloff’s ‘other’ tradition is a useful marker
for the Modernism I seek to associate with the production of ambient meaning, but more
useful yet is Perloff’s reflection, some thirty years later, that the Modernist ‘other’ tradi-
tion is perhaps not an exact historical class of literary corpuses, but a literary-theoretic and
literary-historical point of view :
‘I contrasted this “other” tradition to the TS Eliot “Symbolist” one. In
retrospect, of course this dichotomy is specious. Eliot, surely a major influence
on Ashbery, could just as well have been placed in the opposite camp, and of
course Mallarmé could have replaced Rimbaud. I think what I really had in mind
was less the poetry itself than the way it was being read. Eliot’s New Critical
heirs were read for their “symbolic” meanings and you couldn’t do that with
Ashbery. So from that point of view, the distinction was, and I hope still is,
useful.’
In fact, the difference was perhaps as much in who was reading Eliot and Crane and who
was reading Pound and Ashbery—and, circa 2006, started developing a taste for Eliot.
Perloff’s ‘Poetics of Indeterminacy’ was the work of a liaison between late New Critical,
early post-structuralist academic poetry criticism and its own ‘other tradition,’ the commu-
79nity of para-academic literary scholars and practitioners that grew out of the Black Moun-
tain school, Cage’s circle, and the New York School in the 60’s, began to consolidate its
counter-institutions and counter-canon in 1971 with ‘THIS’ press and its companion mag-
azine ‘THIS,’ and by 1981 already founded the iconic ‘L=A=N=G=U=A=G=E’ journal.
Still, it is more than reasonable to ask what kind of practice takes the Poundian collage of
heterogeneous, barely-networked, but richly concrete nodes—concrete as texts, or concrete
as images, or concrete as concepts, and often concrete in all three regards—together with the
small, molecularly unstable Ashbery lyric, but not the Baudelairean symbol that ponders
‘secret and intimate connections between things, correspondences and analogies.’ In what
sense, or through what kind of reading, could an Ashbery lyric, let alone a Rimbaud lyric,
be more Poundian than Baudelerian?
With apologies to my reader, I reserve my own treatment of an Ashbery lyric (‘At North
Farm’), which well serves as a first experiment in ‘ambient reading,’ for the final section
of this dissertation. Perloff, writing in 1981 under the auspices of ‘indeterminacy,’ finds a
welcoming junction between Poundian concreteness and Rimbaudian instability in the then-
popular trope of difference/deferral, understood as a locus of both the materiality of language
and the instability of meaning. From the perspective that I favor, this theoretical instinct for
analogizing Ashbery’s or Rimbaud’s practice and a Poundian field-composition at the level
of the signifier is misguided in a particularly instructive way. It’s natural enough, in this
respect, to map the unstable relationship between semiotic parts in a Rimbaudian poetic
practice to the paratactic freedom of semiotic parts in a Poundian field composition, but
the aesthetic of entangled semiotic parts in a disequilibrium is not, or at least not for every
kind of reader, in great aesthetic sympathy with the vistas of Pound, Olson, or Zukofsky
field composition. An aporia of semiotic entanglements and subsumptions as in Ashbery or
80Rimbaud is, to the contrary, a proliferation of relations drowning the relata—the things—out.
In fact, I would propose that if there is a genuine shibboleth for the ‘other’ literary-critical
and literary-practical community as it continues to this day, it’s a certain silent rejection of
the prima facie Modernist or radical appeal of aporia, by contrast with e.g. Paul de Man’s
celebratory deconstructionist readings of English romantic verse, or the literary-practical
mainstay of post-Modernist fiction. (We may recall, for instance, that Louis Zukofsky,
the immediate Modernist model for Language Writing, describes poetry as ‘the detail, not
mirage, of seeing, of thinking with the things as they exist, and of directing them along a line
of melody,’ or that Ron Silliman described ‘Ketjak’ as one 106 page long syllogism.) In fact,
from Perloff’s later ‘Radical Artifice,’ to Barrett Watten’s ‘The Constructivist Moment,’ to
Sianne Ngai’s use of ‘constructivist’ to describe the unifying genre of the literary lineage
that runs through ‘Ugly Feelings,’ the idea that—far from being deconstructionist in even
the philosophically subtle sense—‘constructivism’ is the tradition’s best name repeatedly,
more or less independently asserts itself. As such, the term ‘constructivist’ operates in
this context not so much as a shared literary-theoretic concept, but as an occasion for
improvisation. Watten, for example, explicitly constructs his concept of ‘constructivist’ as
a massively overdetermined polyseme, referring to historical Russian Constructivism, to the
foregrounding of a work of art’s formal construction, to the society-making work of utopian
vision, to Freud’s ‘Construction in Analysis,’ and to the social construction of subjectivity.44
Ngai, describing the typical formal profile of the works that appear in ‘Ugly Feelings’—a
study not officially about Modernism at all, but one whose literary-historical outlook, and
implicit literary canon, is drastically shaped by Ngai’s decade in post-Language literary
practice—negotiates her choice by calling the selected works ‘constructivist,’ (10) in quotes.
44
See Watten xix.
81The Modernist literature we take to have an ‘ambient meaning’ dominant, then, is a
‘constructivist’ literature.45 What ‘constructivist’ will mean, on this occasion, is that it is
a cognitive-aesthetically constructive literature—that is, a literature that deals in learning
more than in unlearning—and that it is a literature that presents more as a kind of construct,
a kind of structure or a system or machine, than as a speech act. For a ‘constructivist’ liter-
ature, uninterpretability is a basic condition for the artwork, not a paradox or a reversal or
deferral of resolution. To the degree that this requirement of non-interpretation is motivated
by concerns about the capacity of interpretive closure to suppress richer or wilder shades of
meaning, its game is not to defer the reduction of hermeneutic engagement to interpretive
resolution, but to obviate the reduction of cognitive-aesthetic engagement to hermeneutic
engagement. What does this mean? Imagine, for example, that somebody asked you what
‘The Trial’ proves about the world. Not what ‘The Trial’ says about the world—we have
interpretation for that—but what ‘The Trial’ actually proves. A strange question, surely,
even if a little similar to ones we’ve heard every few hundred years since Aristotle. We might
answer that the question seems askew, that the relationship of literature to knowledge goes
through testimony, trust, communication. (Or perhaps we answer in our critical-theoretical
voice, talking instead of author-functions, power, and performances of knowledge.) We clar-
ify, in either case, that to say that a literary text produces knowledge is to take it on its word,
to trust that what the text communicates to us expresses knowledge. Still, our interlocutor
insists that what she wants to know is what is it that ‘The Trial’ would teach you equally
whether she told you it’s a book by Kafka or the product of a thousand monkeys on a thou-
sand typewriters—what is it that you’d learn if you were visiting the Library of Babel and
45
In calling a work of literature ‘constructivist,’ or—as we do later—‘radically aesthetic,’ I mean primarily
to imply that that a strongly constructivist viewpoint is congenial to the work. I do not mean to imply
that a constructivist viewpoint is the only viewpoint congenial to the given work. Let a thousand partially
overlapping literary-historical classes and literary-critical paradigms bloom.
82picked up ‘The Trial’ from one of the endless rows of shelves. Curiouser and curiouser, then:
the royal road from literary text to knowledge goes through testimony, and testimony in turn
goes through interpretation—through an author-function that says what the work believes
and lends it epistemic weight. To ask what ‘The Trial’ proves—what knowledge it produces
outside of the worth of testimony—is to ask what’s left of literature as an epistemic practice
if we take away interpretation. What can a work of literature prove, before interpretation
turns it into testimony? Nothing in particular, we’d have to say. This dissertation’s point
of view aligns with that part of Modernist literary practice we might understand as working
to make everything out of this nothing—as working to construct the epistemic engine of a
work of art on the underside of interpretation.
This dissertation’s project, then, is partly aiming to begin a story about the epistemic
productivity of Modernist texts that is radically aesthetic in a Kantian sense (in that it re-
gards what depends on testimony and interpretation as external to the work of the Modernist
text), passably materialist in the technoscientific sense, and at least passably materialistic
in the Marxian sense. With these broader pursuits in mind, I propose the framework of
ambient meaning in part to propose a treatment of Modernist and avant-garde texts as both
uninterpretable and cognitively constructive. The driving force behind this dyad comes in
part from the ethos of contemporary ‘ambient writing’ practice—what is sometimes and to
no one’s benefit called ‘post-conceptual poetry’—in the United States: anti-referential, anti-
metaphorical, anti-Idealist, and anti-expressionist, but nevertheless conceiving of itself as
strongly ideas-driven and world-directed. Developing in large part out of Tan Lin’s ‘Ambi-
ent Stylistics,’ ‘Heath,’ and ‘7CV,’ the uninterpretable practice of young experimental writers
like Sophia Le Fraga, Gordon Faylor, Trisha Low, or Gabriel Ojeda-Sague positions itself
not as a body-without-organs or a trans-sense, but as a cognitively constructive practice
83(arguably closely related to the genre Northrop Fry calls an ‘anatomy’) whose productivity
does not operate via interpretability—a Steinian sort of Symbolist practice, we might say.46
My approach to canonical Modernist and avant-garde texts as works of ‘ambient meaning’
is, in this sense, partly by way of proposing a particular 21st century story about what the
Modernist enterprise in literature meant. I believe that this ‘autoencoding’ story is, perhaps,
our latest best hope (if one is inclined to hope this way) for a culturally47 relevant aesthetic
story about radical Modernist form. Where the heroic age of 20th century literary theory cel-
ebrated radical aesthetics in the name of the erotic48 others of interpretation—semiosis, the
body-without-organs, jouissance, the being of language, ‘the third meaning’—the backlash of
a more Bourdieusian age leaves little room for the radically aesthetic, or for anti-interpretive
critical practice, if in the contrast between interpretation and aesthetics the aesthetic is con-
figured as autonomous, immanent, anti-epistemic. Nor does the radically aesthetic fair much
better, from this angle, when configured as endlessly differencing and deferring, self-negating,
and again anti-epistemic.
To think about Modernism through the prism of its epistemic engine, I would argue, is
to reconsider the radically aesthetic by taking ‘aesthetics’ back to its older Baumgratenian
sense as ‘sensible knowledge,’ and taking ‘radical’ back to its older sense of ‘root.’ From
this ‘radically cognitive-aesthetic’ point of view, interpretation fails to access the heart of
Modernist and avant-garde practices not because interpretation treats the text too much like
an epistemic enterprise, but because interpretation doesn’t treat the text like enough of an
epistemic enterprise. Interpretation asks ‘what does the text believe’ but not ‘what does the
text prove, demonstrate, establish.’ As philosopher of science Kenny Easwaran has argued in
46
See for example Trisha Low in Bomb Magazine.
‘Cultural relevance’ of the—admittedly rather vague—kind at question above may, or may not, be
political or social relevance ‘in the last instance.’
48
See Sontag.
47
84discussing the epistemology of mathematical proofs,49 in a sufficiently epistemically rigorous
(in the relevant sense) cognitive engagement with a text, the very concepts of intention and
interpretation lose their grip on the reader’s engagement:
‘If someone presents a sequence of propositions for my consideration, and each
proposition is such that mere consideration of it in light of my current beliefs leads
me to believe it, then I can learn quite a bit from this person, even if I do not trust
him. For instance, if he presents a deductive proof of some conclusion, I do not
have to believe anything he says, as long as I independently have a high credence
in the premises, and see independently that each step follows from previous ones.
(...) This is related to some counterexamples to Grice’s thesis about speaker
meaning. Grice claimed that for a speaker to mean something, she must intend
that her intentions play a role in generating a belief in the listener. However,
with a deductive proof from shared premises, the intentions are irrelevant. This
seems to be the case with many sorts of arguments beyond strict deductive proofs
from shared premises.’
Interpretation, as opposed to ‘mere’ attention, association, and reflection, matters epis-
temically exactly to the extent that we stake the epistemic productivity of our engagement
with a work on the work’s value as testimony.50 Or, in a more critical-theory parlance, inter-
pretation determines what world-directed propositions the author or author-function puts
49
Easwaran, private correspondence (2017): ‘I like to summarize my transferability thesis as ‘show, don’t
tell,’ so it makes sense that the original use of that phrase exemplifies it in a sense though here it’s about
a way of seeing or a conceptual category or something like that, rather than merely the world itself.’ We
might observe, incidentally, that ‘show, don’t tell’ found its way into MFA culture by way of Paul Engle’s
interest in Pound.
50
In speaking of ‘testimony’ above, we mean to refer not to the direct assertoric content of e.g. an author’s
narration, but to the ideological (in the broadest sense) content of the author’s total semiotic act—what
junior-high English class would call an author’s ‘message.’
85her epistemic weight behind. The Foucauldian ‘author function’ is, in this sense, equally
foundational to the epistemology of traditional literary reading or (most versions of) New-
Critical close reading and to the epistemology of ‘subversive’ reading wherein the authorial
testimonial speech-act is put to a cross-examination or a ‘hermeneutics of suspicion,’ but
external to the epistemology of radically cognitive-aesthetic reading. ‘In mathematics,’ Fou-
cault writes, ‘reference to the author is barely anything any longer,’ and in fact we are free
to push our analogy to mathematical proof even further. From the viewpoint of practical51
mathematical formalism (e.g. David Hilbert), a mathematical proof does not assert a math-
ematical truth by means of its propositional content, but instead materially demonstrates
a logical-mathematical truth about its own semiotic system52 by its own structure, which we
then extend through structural analogy to other worldly systems or to Plato’s heaven as we
wish. From the viewpoint of radically cognitive-aesthetic reading, a literary work materially
demonstrates an information-theoretic truth about its own semiotic self by its own structure,
which we then extend through metonymy of content to other, worldly systems or to Plato’s
heaven if we wish. In the next chapter, we set forth to characterize this potential relationship
of a literary work’s semiotic structure to other, worldly systems and to Plato’s heaven both.