---
title: "Idea List"
date: 2021-06-17T00:33:42-04:00
tags:
  - evergreen
---

## Technical

- block based text editor
	- allow you to rip paragraph apart and rearrange sentences spatially
		- paragraph should be able to have hierarchy like bullet points
		- the 'bullet points' should be purely visual (easy toggle to turn it into paragraph/prose mode)
	- column based drafts throughout history (save as draft button but also rewindable history)
- fuzzy rip grep
- hoogle for rdf shapes
- optimizing network topology for crdts
- [[thoughts/CodeMirror|codemirror]] but CRDT + TreeSitter
  - smart [[thoughts/git|git]] merges
  - https://www.wilfred.me.uk/blog/2022/09/06/difftastic-the-fantastic-diff/
- markup any site with a webcrawler + yjs + tldraw
  - maybe use webrecorder
  - markupthis.site is not taken!!
  - backed by content-addressed cdn store?
- daily link share
  - inventory packing simulator but its with tabs... what would affect tab size? length of article == perceived weight in bag?
  - what if you could bring your little backpack of tabs with you to a square or market and trade your tabs with other people
  - list building primitive
- [[thoughts/WebAssembly|WASM]]-based val.town with [[thoughts/CID|CIDs]] distributed using a [[thoughts/Sloppy Hashing DHT]]
  - [[thoughts/IPFS]] as a versioned package manager for all software
  - good example: https://github.com/dylibso/wasmstore
- rotmg but actually good lol
  - dodge mechanic
  - no instakill, should be iframes and way less health (similar to EtG)
  - keep soulbound mechanic
  - no screen rotation
  - multi-floor dungeons, take more inspo from roguelites
  - crowdsources levels + bossfights - community rating system like how Geometry Dash does it
  - should have one free key a day
  - actual good graveyard mechanics to look at past runs/chars
- latency based quorum sensing, similar to how bacteria release a particular molecule and behave differently if sensors of the molecule are particularly active
  - see also: [[thoughts/Sloppy Hashing DHT]]
- [webgpt](https://openai.com/blog/webgpt/) but its for tools for thought
  - "A [reader-generated essay](https://escapingflatland.substack.com/p/reader-generated-essays) is what you get when you can go into someone else’s knowledge graph and make a linear journey through the network, while GPT-5 generates a just-in-time essay that is human-readable."
  - turning a graph traversal into a beautiful essay
- what does entropy + erosion of data look like?
  - is they ways to make [[thoughts/cryptography|cryptography]] that are valid in time windows?
- big touchscreen desk
  - what if i just got a huge old flatscreen tv
  - mounted 4 pressure sensors on each corner and then got a big sheet of thin glass
  - 4 points is enough to pinpoint single-point touch accurately for dragging
  - what if you could use it like a scratch space? like an always available figjam/muse board that also supports linking and trails a la [[thoughts/tools for thought#Memex|memex]]
    - a vision of [communal computing](https://interconnected.org/home/2021/12/21/sage) perhaps
    - a shared screen which anyone can 'connect' to as an external display
    - anyone can drag windows/files to and from it
- wave function collapse for poetry
  - bringing shape-shifting text to its most literal form
  - [https://oskarstalberg.com/Townscaper/](https://oskarstalberg.com/Townscaper/ "https://oskarstalberg.com/Townscaper/") for words
  - base representation is word vectors
    - you can jiggle word vectors around
    - apply transformations to vectors (e.g. the past tense vector)
    - some sort of 1d marching cubes which modifies a vector depending on context?
      - potentially transformer related
  - image <-> text interop using CLIP/unCLIP/DALL-E?
- procedural city + building generation in minecraft + rtx using a codified version of [[thoughts/A Pattern Language]]
  - https://en.wikipedia.org/wiki/Constraint_satisfaction_problem
- procedural visualization of digital garden as an actual garden to help you tend to it better
- better search
  - searching through vectors
    - (no clue if this would work) integral images but applied to vector similarity search in text documents
    - viola-jones for text [[thoughts/latent-factor model|embeddings]]
    - https://github.com/facebookresearch/faiss
	    - https://arxiv.org/pdf/1702.08734.pdf
	    - https://crates.io/crates/kd-tree
	    - https://dl.acm.org/doi/10.1145/3154273.3154307
  - how do we encode sentences/paragraphs/documents as vectors?
    - https://beta.openai.com/docs/guides/embeddings/text-search-using-embeddings
    - https://github.com/ryankiros/skip-thoughts
    - https://github.com/pytorch/fairseq/tree/main/examples/data2vec
  - wasm-based in-browser
    - open question: how do we get the query -> vector??
    - compute vectors for documents ahead of time and compile it into a single static binary file
    - frontend will just load this
    - in the browser, use webgl for fast dot-products
	    - write a fragment shader to compute similarity between search vector and indexed vectors ($1 \times n$ image where $n$ is number of documents and output is value in $[0,1]$ for similarity)
- data provenance
  - https://www.cs.cmu.edu/~NatProg/whyline.html
- LayoutLM + screenshots → auto-categorization of knowledge
  - https://screenotate.com/ but with atlas recall
  - maybe turn this into an app which auto-extracts semantic info from screenshots/images on webpages and does something w it idk
  - how do we prevent https://twitter.com/rsnous/status/1130910375795277824
- Marginalia for the web? browser as a graph database, chronological browsing?
  - what if you could 3 finger swipe up on a browser to see what pages this page is connected to in a graph
  - and you could write on the margins of pages and share those with friends
    - a little annotated web
- Conversational GPS: why do we even look at a screen when we can just ask for directions as if it was a normal person lol
- google photos + olo radio (see [attention economy](thoughts/attention%20economy.md))
* DreamCoder boolsat
  - Creating a LISP-like higher-order language to exploit reusable sub-proofs in specific domains (e.g. graph colouring)
  - kinda iffy on the sat problem solver using dreamcoder, not a lot of exploitable structure in the proofs (otherwise we'd have a more reliable human method)
  - Background:
    - https://en.wikipedia.org/wiki/Boolean_satisfiability_problem
    - https://searchworks.stanford.edu/view/13250178
  * NeuroSAT Paper:
    - https://arxiv.org/pdf/1802.03685.pdf
  * DreamCoder Paper:
    - https://arxiv.org/pdf/2006.08381.pdf
    - https://www.youtube.com/watch?v=qtu0aSTDE2I
- tabfs but for emails
  - [https://bazil.org/fuse/](https://bazil.org/fuse/)
  * [https://blog.gopheracademy.com/advent-2014/fuse-zipfs/](https://blog.gopheracademy.com/advent-2014/fuse-zipfs/)
  * listen on any email server
- deep foveal VR rendering

## Writing

- Short stories/speculative fiction
  - [[thoughts/CID|CID]] as the library of babel
  - Interplanetary communication / state machine
  - Packet switched electricity
  - saving sun for later (make something we take for granted extremely scarce)
- Essays
  - Analog software: software by analogy and by atomic building blocks that interface with each other
    - We should be able to directly manipulate them, like files, rather than only indirectly work with them, like layer activations in a neural network.
    - Software representations for similar ideas should be obviously similar in some way – they should click together, or look similar, or feel similar to the touch.
    - Ideas should remember where they came from – what blog I copied it from, which author I quoted it from, and so on.
  - Essay on epistemic play + [[thoughts/Jestermaxxing]] + mill’s take on why censorship is unethical
  - limits to [[thoughts/Byzantine Faults|BFT]]
    - some malicious activity is indistinguishable from legitimate activity (e.g. deleting a document)
      - _semantic_ byzantine fault tolerance vs protocol byzantine fault tolerance
    - Making distributed systems reliable is inherently impossible; we cling to Byzantine fault tolerance like Charlton Heston clings to his guns, hoping that a series of complex software protocols will somehow protect us from the oncoming storm of furious apes who have somehow learned how to wear pants and maliciously tamper with our network packets. (_[The Saddest Moment](https://scholar.harvard.edu/files/mickens/files/thesaddestmoment.pdf)_ by James Mickens)
    - "I have never had a real-life experience that resembled a Byzantine fault tolerant protocol."
  - two axes of collaborative vs local-first software
	  - ultimately about state reconciliation 
	  - one is temporally (offline-first) the other is spatially (collaboration across multiple computers)
	  - two axes, not mutually exclusive
	  - maybe worth plotting where everything sits lol
	  - data is either
		  - collaborative: co-editing
		  - persistent: saved somewhere (as opposed to ephemeral)
		  - versioned: can time travel
  - [[thoughts/independent research|independent research]] is applied [[thoughts/taste]]
	  - Aesthetics as a heuristic for non obvious optimality
  - Good [[thoughts/search|search]] (aggregators) turns random networks into scale-free networks (see: [[thoughts/Network Theory|network theory]])
  - The sequel to SQL (Against table databases)
    - Data interoperability is really hard with SQL
      - I think interoperability in the context of the web means being able to transparently understand and share data, agnostic of platform.
      - Closed platforms disallow this as they curate the information they present to end-users/devs through the frontend but close off access to the actual data itself.
      - This forces one 'correct' way of looking at data (which is often not the case!)
    - What about evolution of applications?
    - Taking evolution to its natural extension, a different application all together?
    - How do we create sources of truth that are *legible outside of the application*, possibly in ways that the application developer never anticipated?
    - Well, we've done this already once! The applications on our computers ‘share’ data between them is through the file system
      - An application then is a specific view on types of data rather than a standalone thing. Data can be dragged through different applications. Each data is annotated with a type.
    - How might we do this for more general data?
    - Recent years has seen a revival of academic and research interest in the tuple store which will allow us to pull out structure when we need it. It embraces a pluriversal view of data -- a world where multiple alternatives co-exist
      - We can think of a [triple store](https://jzhao.xyz/thoughts/RDF) as a distributed and fragmented SQL database, where instead of tables with rows and value, we have entities with attributes and values. Any application can declare new attributes or alias an attribute to a more common one. The most important part is that applications that share attributes can automatically interoperate their data by using the same attributes
      - This type of ‘decentralized’ database means there is no canonical schema. You can’t mistake the map for the territory because everyone has their own map and can’t force others to view the ’truth’ of the world through your map
      - See more: https://jzhao.xyz/thoughts/Rhizome-Research-Log#october-19th
      - (Inkandswitch explored this with Cambria)
    - One common critique of this is that we lose efficiency and that by knowing the structure of the data ahead of time, we can better optimize queries, etc.
    - Using tuples doesn't prevent us from creating indices and using incremental view maintenance! A lot of really good recent research on differential data flow
    - Importantly, this gives us moldable data which enables people to have the raw material to sculpt and play with
      - (AtProto making the data and schema public means that we've seen an explosion of clients and projects that use BlueSky data)