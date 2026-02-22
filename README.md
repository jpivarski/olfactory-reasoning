# Olfactory Reasoning

Most of what we consider rational thinking is strongly dependent on visual and oral metaphors. That is, when we analyze some aspect of the world in a value-free way, we usually conceptualize it with patterns of thought that work well for visible objects or human speech, but not as well for the other senses, such as touch and smell. However, some of the things we want to think about—emotions, values, and ethics—don't fit well into these visual and oral metaphors. These topics have a reputation for being not rational or hard to frame rationally, but what if we're mistaking clarity of thinking with a preference for our long-distance senses?

## Sights

The primary mental model for most of the physical sciences and data analysis is a vector space. Most data can be described as some sort of table, in which each row of the table is an entity and each column is an attribute of that entity. These can be imagined as _N_ points in an _M_-dimensional space, in which _N_ is the number of rows and _M_ is the number of columns of the table. One row is called a vector, and a collection of vectors can be visualized by picking 2 or 3 columns and drawing them as a 2D or 3D scatter-plot. A model of a real-world mechanism, purported to give rise to the data, is a function that maps every _M_-dimensional point to a probability, which we can draw by coloring the page behind the data with an intensity of color that is proportional to the probability. If most of the data points lie in hotspots of the model's probability, then the model is a good "fit" to the data.

The visual metaphor should be immediately apparent: the data—whatever they represent—have become geometry. Every attribute has become a length, which is to say, a real-valued number. If we want to compare the same attribute of any two data points, or any two attributes expressed in the same units, we can align a ruler with each attribute's axis and read off the distance with as much precision as we need.

A vector space has many things in common with physical space, though physical space has only three dimensions. (Including time as a fourth dimension complicates things for reasons that aren't relevant for this argument.) The _M_ dimensions of an _M_-column table can't be visualized if _M_ > 3, but they function in the same way as the first, second, and third dimension of physical space.

Just like lengths in a physical dimension, a component of a vector scales continuously. An object in physical space can also be rotated: rotating it 90° means replacing its original length and width with width and length, and rotating it 45° means that the original length and width each become mixtures of the new length and width. Similarly, columns of a table can be swapped, or columns A and B of a table can be replaced with A + B and A – B. Just as it's meaningful to compute the size of an object in space, however it is oriented, the length of a vector can be computed from its components (the square root of the sum of the squares of the components, just as you'd compute the hypotenuse of a right triangle). All of these are meaningful operations in physical space because spatial dimensions are interchangeable: we could have labeled any directions "x," "y," and "z," as long as they're perpendicular to each other. Vectors in _M_ dimensions have these properties as well (though more care should be taken if the attributes are expressed in different units of measure, such as pounds-per-square-inch and inflation-adjusted dollars).

As the sciences developed over the past few centuries, data came to be cast more and more as tables of numbers and drawn as charts. An early example of this was William Playfair's 1786 _Commercial and Political Atlas_, which introduced line graphs, bar graphs, and area charts by analogy to cartographic maps—an explicit metaphor of space. Quantifying objects of study as numbers in tables and visualizing them as charts has by now become so strongly associated with rational thinking that the connection is usually implicit. Furthermore, the idea that data can be expressed in a vector space is the starting point for nearly all machine learning techniques.

## Sounds

Some aspects of rational thought are not easily expressed as tables of real numbers, but many of them instead fit a different metaphor, derived from language. Human hearing is sensitive to an almost continuous range of pitches, but we nevertheless force them into categorically distinct pitches when we make or listen to music: notes conform to a scale. Different cultures have different scales, and one culture's notes might be "micro-tones" when measured on another culture's scales, but all traditional music locks into some set of distinguishable pitches. Similarly, human speech can make use of wide variety of sounds, and yet we cluster sounds into distinguishable phonemes with standardized vowel formants, intonation, voicing, lengths of aspiration, and places of articulation. Different languages can have completely different sets of phonemes, but within a language, phonemes are consistent with sharp boundaries between them: "b" and "bet" need to be distinguishable from "p" and "pet." Oral reasoning tends to be categorical.

Visual data is sometimes categorical, especially when it consists of a small number of sharply contrasting colors, such as different kinds of fruits that stand out from the background leaves. But language analogies are more often our source of metaphors when we want to analyze categorical data.

For instance, when reasoning about integers (whole numbers), we conceptualize the numbers as words, rather than lengths in space. The sequence of words known as counting—"one, two, three, four, five..."—is a kind of prose poem that corresponds with everything that can be counted through a one-to-one relationship. The most evident one-to-one relationship between the sequence
* 🦆
* 🦆🦆
* 🦆🦆🦆
* 🦆🦆🦆🦆
* 🦆🦆🦆🦆🦆

and the sequence
* 🗿
* 🗿🗿
* 🗿🗿🗿
* 🗿🗿🗿🗿
* 🗿🗿🗿🗿🗿

also has a one-to-one relationship with the word sequence
* one,
* two,
* three,
* four,
* five.

Although no one has ever uttered it, this prose poem has rules that describe how it continues to very high numbers: "million, billion, trillion, quadrillion, quintillion, sextillion, septillion, octillion, nonillion, decillion, undecillion, duodecillion," etc. provides a vocabulary for ever-increasing scales (derived from Latin prefixes), and there are rules for constructing and interpreting a number like "five quadrillion, two million and seventeen." The decimal form of a number, such as "5,000,000,002,000,017", is also linguistic: it has a vocabulary of ten single-letter digit-words, a very simple grammar, and a rule for associating any such sequence with a numerical concept.

Just as European mathematics had an emphasis on geometry, influenced by Euclid's _Elements_ and Zeno's distance paradox, Indian mathematics had an emphasis on number theory and combinatorics, influenced by Pingala and other mathematicians who were more interested in enumeration and poetry than shapes and distance. Pingala's _Chandaḥśāstra_ ("on prosody", 3rd‒2nd century BCE) counts the number of possible poetic forms using combinatorial algorithms, introducing binary numbers to represent patterns of short and long syllables, as well as recursion and what we call Pascal's Triangle and Fibonacci Numbers. Ancient Indian mathematics emphasized combinatorics, number theory, algebra, and algorithms (both "al"s from from India through Arabic), making up what we today call discrete mathematics. It was also much more oral than visual: whereas Niccolò Tartaglia (1545 CE in Italy) felt compelled to draw interlocking 3D shapes to describe his solution to the cubic equation, Indian mathematicians were more comfortable with word sequences and symbols. For instance, Madhava of Sangamagrama (1340‒1425 CE in Kerala) computed sine and cosine tables that were then memorized using a mnemonic system of associating digits with spoken syllables (Katapayadi).

Language is a model for logic as well, which may be self-evident because logic is a formalization and strengthening of verbal arguments. But logic is not just applied to verbal speech, it also has the same form as language, especially grammar. Humans develop grammar naturally, sometimes without even being aware of it, and yet they can be extremely formal systems. We may think of grammar as rules that can be broken, but that reflects a lack of diligence on the part of the descriptive grammarian. In 6th‒5th century BCE India, Pāṇini expressed the grammar of Sanskrit with iron-clad rules—no exceptions—it just took 3,996 rules to express all the variations.

Both grammar and logic consist of templates that specify when a sequence of words is valid. An important difference is that violating grammar results in sentences that can't be comprehended, whereas violating logic results in faulty conclusions. They're different domains, but with the same shape.

The classic example of a logical template is a syllogism like "All A are B; C is an A; therefore C is B," which could be filled in as "All men are mortal; Socrates is a man; therefore Socrates is mortal." Modern logic (starting from George Boole, Gottlob Frege, and Bertrand Russell) takes logic to be a completely algebraic system of symbol manipulation: you write a sequence of symbols, transform the sequence following a specified set of inference rules, and attempt to arrive at another sequence of symbols. This form of logic was absolutely essential in the formulation of computer science and the working of today's computers.

Although mathematical logic and computer programming languages are rarely read out loud, they're clearly derived from language and still have the form of oral speech, just as vector spaces—however abstract—have the form of visible objects.

## Smells

Smells are different. Whereas we might draw a chart to get a better understanding of some data or read a proof out loud to get a better understanding of its logical structure, we almost never turn to smells to aid our rational thinking. Moreover, sights and sounds are often (not always) value-neutral, whereas smells are almost immediately good smells or bad smells. Conceptualizing a smell in a value-neutral way often takes effort.

But smells are also different in that they are hard to fit into vector spaces or categorical templates. We might attempt to describe a smell as a row in a table by enumerating all the possible smells as columns of the table: ginger, lilac, nail polish, manure, and so on. If the air smells overwhelmingly of ginger, we mark "1, 0, 0, 0, ..." and if the air of another room is predominantly lilac and nail polish, we fill in the next row as "0, 1, 1, 0, ..." However, smell perception is not adept at perceiving differences the way vision is for lengths. How do we know the lilac and nail polish should both be 1? Maybe the lilac smell is twice as strong as the nail polish, and it should be "0, 2, 1, 0, ..." Worse still, the problem is not just a matter of precision, but definition: what does "twice as strong" even mean when comparing the smell of lilac and the smell of nail polish? It is as though every type of smell is expressed in different units of measure—as different as pounds-per-square-inch and inflation-adjusted dollars.

If we can't express different components of the smell vector in the same units, then we can't add components to "rotate" the vector, either. Furthermore, this vector has no concept of length. We can't express the total smell, summed over all the individual smells.

Just as smells don't fit into a vector space well, they don't have the categorical strictness or temporal sequencing to be language-like, either. Smells fail to be categorical in two ways. First, there's a difference in intensity between a weak smell and a strong smell, without the sharp distinctions that separate phonemes. We might rate them as weak, medium, and strong, or five levels, without clear dividing lines between them. Second, different types of smells (columns in the table) blur together as well. One person might consider two smells to be different types—the "manure" on a farm might be a different type from the "manure" in a sewer—but another person might not be able to distinguish them. There's no shared language with standardized clusters. Even color names on a rainbow tend to be clusterized within a culture: Japanese doesn't distinguish between green and blue as sharply as English does, and English does not distinguish between light blue (голубой) and dark blue (синий) as Russian does. Smell languages vary from individual to individual.

Of course it's possible to identify which odorant molecules activate distinct physiological pathways in the human nose, measure the density of these molecules in the air, fill a table, and draw a chart. In this form, the fundamental set of types of odorants are enumerable (the "basis set" in vector terminology), and the number/intensity of each type of molecule can be measured relative to each other type. But such a procedure would replace the sense of smell with machines that we read out visually with dials or aurally by counting clicks—the experiment could be performed by a scientist with no sense of smell at all. Such an analysis would fit the visual metaphor of a vector space, but it bypass the subjective sense of smell itself.

## Emotions and Values

asdf

## Ethics

asdf
