_Fill in each this file with your responses, placing each response after its
corresponding question._

---

**Question**

Pick three quotes from the readings about language design. Good candidates
are:

- Something you agreed with / resonates with your own experience
- Something you disagree with
- Something that is interesting, a new idea or perspective you'd like to remember
- Something you didn't understand

For each quote, describe what it was about the quote that led you pick it.

**Response**


1. “I think that our discipline mostly uses anecdotes to argue about programming languages. As such, it is no wonder that the arguments get heated.” [Palvus, 2012]
    I really liked this quote from Andreas Stefik, as it reflected on my experience with programming languages. Typically people base their views/arguments of PL’s on incomplete views or stereotypes. In “C is Manly, Python is for ‘n00bs’”, Linus Torvalds is cited as saying “C++ is a horrible language… made more horribly by the fact that a lot of substandard programmers use it, to the point where it’s much much easier to generate total and utter crap with it”[Yang and Rabkin, 2015] Which is exactly what Stefik is saying in this instance word for word, which has the impact of invalidating the work of all C++ developers, because of Linus Torvalds’ anecdote.

2. “API design is not a solitary activity. Show your design to as many people as you can, and take their feedback seriously. Possibilities that elude your imagination may be clear to others.”[Bloch, 2006]
    I also really liked this quote, as it reminded me of user testing in CS124: Interaction Design and reading through Don’t Make Me Think by Steve Krug. He mentions that “After you’ve worked on a site for even a few weeks, you can’t see it freshly anymore. You know too much. The only way to find out if it really works is to test it.”[Krug, 2006]. This also connects to the idea that “ Possibilities that elude your imagination may be clear to others.”
    It also reminds me of an instance of user testing in CS124. I had created mockups in Figma for this application, and I was happy with the layout and everything to do with it, and the feedback received was “it looks like how a clown looks and I can’t read anything”, which upon looking at the mockup, it did look like how a clown looks and I could barely read anything. This was then fixed by altering the color scheme to have more contrast/more readable and legible text. The important part to me was that I was completely blind that something that I was so happy to go ahead with was almost unusable. 

3. “You can always add things later, but you can't take them away.”[Bloch, 2006]
    This quote I think is really important. I can’t remember which feature was removed because it was so long ago, but I remember the language Elm removed huge features that people had been using in the new release of Elm and people being upset over this and jumping ship to other functional languages. I remembered that it made sense to remove bloat (and to have a smaller language with fewer warts!) but that it also made very little sense to remove features already being used by people. Hence the quote “you can’t take them away” as people already depend on those things.


---

**Question**

How would you know a well-designed language? What are the symptoms? How would
you know a poorly designed language? What are the symptoms?

**Response**

    I think a well-designed language is a language where it falls into a niche and has it's use cases. Steele mentions that "In a race, a small language with warts will beat a well designed language because users will not wait for the right thing; they will use the language that is quick and cheap, and put up with the warts. Once a small language fills a niche, it is hard to take its place."[Steele, 1998]. Hence, I think the symptoms of a well-designed language is one where it's started out as a smaller language, but has been designed with support from users and groups to grow into a bigger language, whether that's through changing over time or through package libraries and extensions, which allows it to fall under a niche that loves the language.
    I think a poorly designed language is one which might fall into niches along with other programming languages, or one that has started out with a high barrier of entry through bloat (or warts in the case of Steele). A symptom of this could be removing features later on, as the language has become too bloated and needs to remove functionality.

---

**Question**

How might the themes of _Growing a Language_ relate to ideas from the Fowler reading?

**Response**

    I think they're both concerned with the design of programming languages and to make a set of guiding principles when designing them. For instance, Steele is concerned with readability as "programming languages need to be more like the languages we speak—but it might be good, too, if we were to use the languages we speak more in the way that we now use programming languages."[Steele, 1998], and Fowler mentions that "The overall goal for a DSL, as with any writing, is clarity for the reader."[Fowler, 2010]. The interesting part though is that Fowler also mentions that designers shouldn't "try to make the DSL read like natural language"[Fowler, 2010]. I think this could infer that Steele is concerned with making programming languages sound more like natural language conventions, whereas Fowler is concerned with making languages (or more specifically DSL's) more precise and readable.

---

**Question**

In what way is an API a language?

**Response**

    An API is a language similar to how DSL's are languages. In the book Domain-Specific Languages Fowler states that DSLs are "a front-end to a library providing a different style of manipulation to the commend-query API. In this context, the library is the semantic model of the DSL."[Fowler, 2010]. 
    Bloch references this as well, stating that API's should "Strive for intelligibility, consistency, and symmetry. Every API is a little language, and people must learn to read and write it. If you get an API right, code will read like prose."[Bloch, 2006]. 
    Therefore I think that an API is a language in the same way that DSL's are languages, so like normal languages but in limited domains/not general purpose use cases. 

---

**Question**

What does the post on grayscale tell us about the process of API design?

**Response**

    I think the post tells us how there can be multiple meanings for a concept/problem. For instance, some users will prefer the first option, others the second or third, even though they follow the same process but with different naming conventions. The only different implementation is the 4th option, which makes clear that "you will need to change the function name to get a semi-transparent version of the color. Also, if in the future one needs to change the color to not be a shade of gray, a function name change is not needed."[Verou, 2014].
    I think this also connects to How to Design a Good API and Why It Matters as function names being changed ties back into being able to add in features but not being able to remove features.
    What I'm trying to say is that the the  notation for grayscale colors can seem like a very insignificant design decision, but in the realm of API design this problem can have real impacts on the work people do, and it's the reasons outlined in Bloch's paper that this should be carefully navigated.


---

**Question**

The Pavlus article mentions the researchers' comments that people preferred
"natural-language replacements for some of the more abstruse syntax". In other
words, people found it easier to work with code that looks more like a human language (e.g.,
English). Consider the following quote by William R. Cook, one of the creators
of AppleScript:

> The experiment in designing a language that resembled natural languages (English
> and Japanese) was not successful. It was assumed that scripts should be
> presented in “natural language” so that average people could read and write
> them. … In the end the syntactic variations and flexibility did more to confuse
> programmers than to help them out. It is not clear whether it is easier for
> novice users to work with a scripting language that resembles natural language,
> with all its special cases and idiosyncrasies. The main problem is that
> AppleScript only appears to be a natural language: in fact, it is an artificial
> language, like any other programming language. … even small changes to the
> script may introduce subtle syntactic errors that baffle users. It is easy to
> read AppleScript, but quite hard to write it.
> [[Cook 2007, page 1-20]](https://dl.acm.org/citation.cfm?doid=1238844.1238845)

Are these two experiences of natural languages at odds with one another? Would
you choose to include natural language in the design of a DSL? If so, how might
you do so? If not, why not?

**Response**

    I think they're at odds with one another. The syntax of Quorum/how one would read and write it seems very very similar to AppleScript. 
    I do think that natural language should be included in the design of DSLs however. I personally enjoy the use of natural language in languages like SQL, where it's not exactly a natural language, but by utilizing natural language replacements it can be readable and understood by beginners and novices.  

---
