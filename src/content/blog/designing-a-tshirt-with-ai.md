---
title: 'Designing a T-Shirt with AI: What I Learned About Being the Human in the Loop'
description: "Newcastle's tech conference (/NEW) announced a t-shirt design competition. I'm a software developer, not a designer. But I had Claude Code, a clear brief, and opinions."
pubDate: '2026-03-25'
heroImage: '../../assets/designing-a-tshirt-with-ai.jpeg'
---

Newcastle's tech conference (/NEW) announced a t-shirt design competition. I am a software developer, not a designer. But I wanted to try something out of my comfort zone with Claude Code. I wear t-shirts, I have seen bad and good conference tshirts. So I decided to give it a go.

The theme was "Humans In The Loop." Which turned out to be so meta, because the entire process became exactly that.

Here's what actually happened across hundreds of iterations:

Claude got the brief, past designs, and brand specs. About 30 tshirt designs that I liked. A few of my ideas. It generated multiple concepts. I picked one based on gut feeling — not because Claude decided it was a good idea (it actually came up with some very lame ideas - robotic hand reaches out to touch human's hand, like in the "Creation of Adam"! I wouldn't wear a tshirt with that!).

Then I started looking into actually designing. Various tools, almost gave up — it meant installing, registering, buying, learning something new. I put that idea to rest and went for a walk. Browsed for more ideas later, and after a bit of back and forth with Claude, I realised that all of my ideas were based on text. All I need is an SVG. And it is code. Claude is good at generating code. Right?

We kicked off with some designs. They were absolutely terrible. The long refinement started. Dozens of SVG iterations. I'd give messy feedback — "too busy," "less chrome," "I still like the clean version better" — and Claude would translate that into new updated SVGs. Then it got boring and repetitive and I still felt like I have no idea what I was doing. So I gave Claude a "design critic" persona — a senior designer with screen-printing experience. It knew what works in production: minimum stroke widths, how colours hold on fabric, whether something will read from across a room. Every iteration got reviewed against those constraints before I even saw it. My critic was ruthless and really cared about 1 pixel differences.

At some point I noticed I was just agreeing with the critic's every suggestion. It sounded like it knew more than me about printing designs on shirts, and with every iteration it was getting better and better. So I built an autonomous review loop and took myself out of that layer. Made myself some tea and watched it iterate.

Eventually the design got to a 9/10. Pixel-perfect. Production-ready. Done. Pretty amazed that it created something printable pretty much on its own. Showed it to my kids. They were not impressed. I had to do a lot of explaining — what AI does, what the human does, the loop... They shrugged their shoulders and walked away.

Clearly not the right design. Threw it away and started over. My gut (and my kids) said the concept was too narrow for the audience (the conference audience is not just developers), and no amount of polish was going to fix that. So I went back to the brief, explored a completely different direction, and refined that into something I was actually happy with (using the same critic-SVG loop). This time I ran 10 of them at the same time exploring different ideas. Showed it to the family and they got it. Looked at the design from a distance on my screen, did some more refinements and finally submitted.

No idea if it'll get picked, but honestly that was not the point. The process was the valuable part.

It's been almost a week since I submitted my designs. Looking back, there are a few things I'd tighten up if I did this again.

My "design critic" was a persona prompt in the same conversation that generated the work. That's like asking a developer to QA their own code — too attached to the output. A separate evaluation step, with no memory of generating the work, would have been harsher and more honest earlier.

The critic scored out of 10, but 10 against what? Design quality, print readiness, and audience fit are different axes. Collapsing them into one number is why a 9/10 design still felt wrong.

In the ideal world, I would have run many more iterations, but I was quickly running out of tokens.

There are a lot of other things I would have refined if I ever did this again — research what makes a better critic, actually understand design, typography, perception, colours, etc. But honestly, the fact that a software developer with zero design experience could produce a printable t-shirt design is kind of the point. The tshirt design is ok, nothing to brag about. But design is such a subjective thing and so hard to automate! If I could improve one thing - that would be my taste in conference tshirts. AI was just a tool to get my ideas onto something tangible.

AI is already lowering the barrier for non-experts to do things outside their field. Designers write code, plumbers write trading bots, school librarians create e-commerce sites for book fairs. We're not there yet though — the tooling still has some friction, and producing quality output without domain expertise is harder than it should be. But it will not take too long for AI and tools to get better.
