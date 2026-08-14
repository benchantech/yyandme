---
layout: episode
title: "Probably vs Provably (Arc 2 | Episode 10)"
permalink: /episodes/probably-vs-provably/
---

<iframe
  data-testid="embed-iframe"
  class="responsive-iframe"
  src="https://open.spotify.com/embed/episode/0lWUMAS7sdkhI3dkrOh2WL?utm_source=generator"
  frameborder="0"
  allowfullscreen
  allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"
  loading="lazy">
</iframe>

A childhood RPG in Visual Basic becomes a way to think about building software when the machine is probably right instead of provably obedient.

This episode moves from pixel editors, treasure chests, and game state into the stranger work of building AI systems: defining boundaries, testing probabilistic behavior, designing for repair, and deciding what children should learn when machines can already do so much of the underlying work.

**Keywords**: AI software, probabilistic systems, game design, software repair, human judgment, YY Method
{: .ep-keywords}

🎧 **Start with [The First Echo](https://yyandme.benchantech.com/the-first-echo)** — then leave a trace. Your feedback shapes this podcast.

{% include episode-navigation.html %}

<div class="section-rule transcript-rule">
  <span class="label">FULL TRANSCRIPT</span>
  <span class="line"></span>
</div>
<div class="transcript-paper">
<p>When I was a teenager, my brother and I made an RPG in Visual Basic.</p>
<p>And when I say we made an RPG, I mean we had to make almost everything.</p>
<p>We made a little pixel character editor.</p>
<p>You moved around with the arrow keys and filled in squares one at a time.</p>
<p>We drew characters facing up, down, left, and right.</p>
<p>We made trees and rooms and treasure chests with open and closed states.</p>
<p>Then we had to teach the computer what all those things meant.</p>
<p>Can you walk on this square?</p>
<p>Can you walk underneath this object?</p>
<p>If you opened this treasure chest, does it stay open when you come back?</p>
<p>If you picked up the thing inside it, does it appear in your inventory?</p>
<p>What happens when you use it?</p>
<p>Then we needed battles, stats, magic, and dice rolls behind the scenes.</p>
<p>We played Dungeons &amp; Dragons, and we played an enormous number of video games.</p>
<p>Mario.</p>
<p>Zelda.</p>
<p>Final Fantasy.</p>
<p>EarthBound.</p>
<p>Secret of Mana.</p>
<p>Chrono Trigger.</p>
<p>We would get maybe a game for Christmas or a birthday and then play the heck out of it.</p>
<p>So we were constantly reverse-engineering them.</p>
<p>How did Final Fantasy make this battle system work?</p>
<p>How did they make a cutscene?</p>
<p>How did the game remember that I already did something?</p>
<p>And the basic assumption underneath all of this was simple:</p>
<p>If I tell the computer exactly what to do, it will do exactly that.</p>
<p>If opening a treasure chest changes a variable from zero to one, that chest is open every time.</p>
<p>That’s the world I learned to program in.</p>
<p>And now I’m building software with AI, and that assumption is disappearing.</p>
<p>I can tell an AI system, “When the player chooses this, remember it and use it later.”</p>
<p>And it might.</p>
<p>Probably.</p>
<p>Maybe nine times out of ten.</p>
<p>And that difference between probably and provably is enormous.</p>
<p>Because a normal program can have a rule that says, “Health goes down by ten.”</p>
<p>An AI system can understand what health is.</p>
<p>It can understand why health should go down.</p>
<p>It can write a beautiful description of the character getting hurt.</p>
<p>And then, every once in a while, it might forget to actually subtract ten.</p>
<p>That’s a very strange kind of machine to build with.</p>
<p>It gets stranger when you’re making a game.</p>
<p>In the games I grew up making, I had to anticipate what you could do.</p>
<p>Talk.</p>
<p>Fight.</p>
<p>Open.</p>
<p>Use.</p>
<p>Run away.</p>
<p>Whatever choices I programmed were the choices you had.</p>
<p>Now I can give somebody a text box.</p>
<p>Suddenly they can say anything.</p>
<p>That’s incredibly powerful.</p>
<p>It also means I can no longer anticipate the entire program.</p>
<p>So I’ve found myself programming in a different way.</p>
<p>Instead of only saying what I want, I spend a surprising amount of time saying what I don’t want.</p>
<p>Do this, but don’t do this.</p>
<p>And if this happens, definitely don’t do that.</p>
<p>And if you’re uncertain, preserve this other thing.</p>
<p>It’s actually very close to the Why and Why-Not part of the YY Method.</p>
<p>I’m giving the AI a direction, but I’m also trying to define the boundaries around that direction.</p>
<p>And even then, I don’t actually know if it worked.</p>
<p>I have to run it.</p>
<p>Then run it again.</p>
<p>And again.</p>
<p>Because if something works nine times out of ten, testing it once tells me almost nothing.</p>
<p>And here’s where things get really weird.</p>
<p>I can use another AI to test the first AI.</p>
<p>I can give it a pretend player.</p>
<p>I can say, “You’re this age. You like these things. You chose these answers. Now go through the experience repeatedly and record what happens.”</p>
<p>But then I have another problem.</p>
<p>How do I know the AI testing my AI is right?</p>
<p>I can use another AI to inspect the results.</p>
<p>But how do I know that AI is right?</p>
<p>You can see where this is going.</p>
<p>Eventually, someone has to exercise judgment.</p>
<p>And I think that’s the part of AI that interests me much more than whether AI can code.</p>
<p>Because, yes, AI can code.</p>
<p>It can now do in seconds things that took my brother and me hours or days to figure out from books.</p>
<p>I don’t have to think very often anymore about sprite masks or bitmap caching or the mechanics of a loop.</p>
<p>That’s wonderful.</p>
<p>But I’ve traded one kind of difficulty for another.</p>
<p>The old difficulty was:</p>
<p>How do I make the computer do this?</p>
<p>The new difficulty is:</p>
<p>How do I create a system that usually does what I mean, recognize when it doesn’t, and recover when it fails?</p>
<p>That last part is becoming increasingly important for me.</p>
<p>I’m starting to think that trying to make probabilistic software behave perfectly may be the wrong goal.</p>
<p>I still want to make it as reliable as I can.</p>
<p>But I’m also beginning to design for repair.</p>
<p>If the AI forgets something, can the person correct it?</p>
<p>If a game takes the story in the wrong direction, can the player tell it so?</p>
<p>If the system misunderstands your intention, have I taught you enough about how it works that you can recover instead of assuming the machine must be right?</p>
<p>That’s a very different relationship with software.</p>
<p>And it leaves me with a much bigger question.</p>
<p>Because I have kids.</p>
<p>What should they learn?</p>
<p>Should they learn the things I learned?</p>
<p>Variables.</p>
<p>Data structures.</p>
<p>Syntax.</p>
<p>All the machinery underneath the software?</p>
<p>Or should they spend that time learning how to describe what they want, judge what comes back, find the failure modes, and direct machines that already know how to do the underlying work?</p>
<p>I genuinely don’t know.</p>
<p>And I’m not sure anybody knows.</p>
<p>I think about it in music.</p>
<p>I’ve spent decades learning how to make sounds physically on a violin.</p>
<p>If I want a particular effect, I know what détaché is.</p>
<p>I know what ricochet is.</p>
<p>I know what pizzicato is.</p>
<p>I know what happens when I move the bow toward the fingerboard.</p>
<p>But imagine that instead of playing the instrument, my job becomes directing an instrument that can play itself.</p>
<p>I might simply say, “Make this sound spooky.”</p>
<p>The machine can figure out the low register, the articulation, the harmony, the texture.</p>
<p>So do I still need to know how those sounds are made?</p>
<p>Maybe.</p>
<p>Maybe not.</p>
<p>But I know that my ability to judge what the machine produces is deeply connected to having spent decades making those sounds myself.</p>
<p>And that’s the unresolved part for me.</p>
<p>I’m building AI systems right now partly because I think this may be where software is going.</p>
<p>I could also be early.</p>
<p>I could be wrong.</p>
<p>The things I’m making could work beautifully and find an audience.</p>
<p>Or I could discover that nobody wants them.</p>
<p>That’s okay.</p>
<p>The useful part isn’t dependent on that outcome.</p>
<p>Because I’m learning how to operate in a world where more and more things are probably right instead of provably right.</p>
<p>And I suspect that’s bigger than programming.</p>
<p>Maybe the important skill isn’t knowing how to make the machine obey.</p>
<p>Maybe it’s knowing what to do when it doesn’t.</p>
</div>
