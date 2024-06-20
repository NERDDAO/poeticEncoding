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