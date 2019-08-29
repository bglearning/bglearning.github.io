---
layout: post
title: "Tongue-in-cheek NLP Paper Summaries"
author: "Bijay Gurung"
categories: technology
tags: [ml, papers, tech]
image: assets/img/nlp.png
---

### [2001: Neural language model](http://www.jmlr.org/papers/volume3/bengio03a/bengio03a.pdf)
We should really be using a distributed representation of words and also Neural Networks for Language Modeling! 
No more mucking around with these counts and all. See, it works! (Albeit takes a bit of computation…)
  
### [2013: Word2Vec](https://arxiv.org/pdf/1301.3781.pdf) 
>“You shall know a word by the company it keeps”.  

We should be fully exploiting this. I mean, if we want embeddings, why language model? 
Let’s predict the word from its context and while we are at it, try predicting the context from the word as well! 
Oh, and let’s make this a very simple linear model so that we can go through a ton of data.

### [2014: Sequence-to-sequence](https://arxiv.org/pdf/1409.3215.pdf)
So ya, for translation, if we want an end-to-end network, think it makes sense to have an encoder that… 
(no points for guessing) encodes the source sequence and then have a decoder that decodes it to the target sequence. 
Hmm… this works. It’s almost state-of-the-art. (Oh, and it works better if we reverse the source sentence; don’t ask why).

### [2015: Jointly learning to align and translate (Attention)](https://arxiv.org/pdf/1409.0473.pdf)
Why are we expecting the encoder to encode a whole sentence (with all its complexity and nuances) into one vector? 
The poor encoder! Let’s do this instead: allow the decoder to pay “attention” to whatever it wants/needs in the source sentence. 
Wow, it works! Thank me later dear encoder...

### [2017: Attention is all you need](https://arxiv.org/pdf/1706.03762.pdf)
Well, hold on a second. If we are allowing the decoder to attend to any part of the input sequence, 
then do we really need the recurrence bit? It seems redundant. Let's do away with it. 
What if we used attention all the way down… Ha, it works! Knew it! Attention is all you need! Behold, the mighty *Transformer*.

### [2018: ULMFiT](https://arxiv.org/pdf/1801.06146.pdf)
Transfer Learning for NLP hasn’t been working as good as it does for Computer Vision until now… *eyes sparkle*. 
If we make it a three phase process: General LM, Domain specific LM fine-tuning and then classifier fine-tuning, 
and also use a bunch of smart techniques (discriminative fine-tuning, slanted triangular learning rates, 
gradual unfreezing), it starts working!

### [2018: ELMo](https://arxiv.org/pdf/1802.05365.pdf)
The meaning of words are context-dependent and so their embeddings should be context-dependent too. 
Of course, that’s not news. Many have tried. 
But hear out our method: we train a multi-layer Bidirectional LSTM Language Model and then have the embeddings be 
linear weighted combinations of their representations in the different layers! And as we believe in individual 
freedom and agency, we let the network decide how much to weigh each layer for the particular downstream task. 
And... it works!

### [2018: GPT](https://s3-us-west-2.amazonaws.com/openai-assets/research-covers/language-unsupervised/language_understanding_paper.pdf)
Ya, pre-training of a Language Model is a great idea. 
But a lot of the time, when fine-tuning it for some other task, we end up having to change the architecture into 
something task-specific. Boo! What if instead we go the other way around i.e massage the input into something 
we can feed into the model. Ya, why should the model bend the knee! Also, let’s use *Transformer* (Decoders) instead of LSTMs. 
That’s more fashionable now.

### [2018: BERT](https://arxiv.org/pdf/1810.04805.pdf)
When pre-training language models, we should really be looking at both the previous and next tokens. 
And do that at the same time. *Takes out masks*  Masked LM, let’s go! 
Oh and we should have a sentence-level pre-training task as well. How about Next Sentence prediction? 
And let’s use Transformers! Woah! This works so well.

### [2019: TransformerXL](https://arxiv.org/pdf/1901.02860.pdf)
We should bring back recurrence. Ya, make recurrence great again! Not at the token level though. 
How about at the segment level? Oh, and the positional encodings need to be relative now.

### [2019: GPT2](https://d4mucfpksywv.cloudfront.net/better-language-models/language-models.pdf)
Hmm… So, looks like the uni-directional nature of our Language Modeling is our Achilles heel. 
Oh well, let’s just scale the whole thing up. \*more data, compute and some changes later\* Unicorns! :o What have we done!

### [2019: XLNet](https://arxiv.org/pdf/1906.08237.pdf)
BERT, dude. You are doing good but your masks are all over the place! It’s messing things up. 
We should really be doing *Permutation Language Modeling*. 
Oh, and while we are at it, let’s use TransformerXL because  
a) Recurrence ftw! b) It'll be easier to name the network...

### [2019: RoBERTa](https://arxiv.org/pdf/1907.11692.pdf)
Meh. Let's train BERT longer and on more data.

--- 

**Disclaimer**: *This is a just-in-jest, tongue-in-cheek post and so comes nowhere close to doing justice to all the work, details
and nuances of these (and tons of other) papers. Still, even as such, if any of it is just plain wrong in some way, please let me
know. Feedback always welcome.*

