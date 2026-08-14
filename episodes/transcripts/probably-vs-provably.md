# YY & Me, Episode 10: Probably Versus Provably

When I was a teenager, my brother and I made an RPG in Visual Basic.

And when I say we made an RPG, I mean we had to make almost everything.

We made a little pixel character editor.

You moved around with the arrow keys and filled in squares one at a time.

We drew characters facing up, down, left, and right.

We made trees and rooms and treasure chests with open and closed states.

Then we had to teach the computer what all those things meant.

Can you walk on this square?

Can you walk underneath this object?

If you opened this treasure chest, does it stay open when you come back?

If you picked up the thing inside it, does it appear in your inventory?

What happens when you use it?

Then we needed battles, stats, magic, and dice rolls behind the scenes.

We played Dungeons & Dragons, and we played an enormous number of video games.

Mario.

Zelda.

Final Fantasy.

EarthBound.

Secret of Mana.

Chrono Trigger.

We would get maybe a game for Christmas or a birthday and then play the heck out of it.

So we were constantly reverse-engineering them.

How did Final Fantasy make this battle system work?

How did they make a cutscene?

How did the game remember that I already did something?

And the basic assumption underneath all of this was simple:

If I tell the computer exactly what to do, it will do exactly that.

If opening a treasure chest changes a variable from zero to one, that chest is open every time.

That’s the world I learned to program in.

And now I’m building software with AI, and that assumption is disappearing.

I can tell an AI system, “When the player chooses this, remember it and use it later.”

And it might.

Probably.

Maybe nine times out of ten.

And that difference between probably and provably is enormous.

Because a normal program can have a rule that says, “Health goes down by ten.”

An AI system can understand what health is.

It can understand why health should go down.

It can write a beautiful description of the character getting hurt.

And then, every once in a while, it might forget to actually subtract ten.

That’s a very strange kind of machine to build with.

It gets stranger when you’re making a game.

In the games I grew up making, I had to anticipate what you could do.

Talk.

Fight.

Open.

Use.

Run away.

Whatever choices I programmed were the choices you had.

Now I can give somebody a text box.

Suddenly they can say anything.

That’s incredibly powerful.

It also means I can no longer anticipate the entire program.

So I’ve found myself programming in a different way.

Instead of only saying what I want, I spend a surprising amount of time saying what I don’t want.

Do this, but don’t do this.

And if this happens, definitely don’t do that.

And if you’re uncertain, preserve this other thing.

It’s actually very close to the Why and Why-Not part of the YY Method.

I’m giving the AI a direction, but I’m also trying to define the boundaries around that direction.

And even then, I don’t actually know if it worked.

I have to run it.

Then run it again.

And again.

Because if something works nine times out of ten, testing it once tells me almost nothing.

And here’s where things get really weird.

I can use another AI to test the first AI.

I can give it a pretend player.

I can say, “You’re this age. You like these things. You chose these answers. Now go through the experience repeatedly and record what happens.”

But then I have another problem.

How do I know the AI testing my AI is right?

I can use another AI to inspect the results.

But how do I know that AI is right?

You can see where this is going.

Eventually, someone has to exercise judgment.

And I think that’s the part of AI that interests me much more than whether AI can code.

Because, yes, AI can code.

It can now do in seconds things that took my brother and me hours or days to figure out from books.

I don’t have to think very often anymore about sprite masks or bitmap caching or the mechanics of a loop.

That’s wonderful.

But I’ve traded one kind of difficulty for another.

The old difficulty was:

How do I make the computer do this?

The new difficulty is:

How do I create a system that usually does what I mean, recognize when it doesn’t, and recover when it fails?

That last part is becoming increasingly important for me.

I’m starting to think that trying to make probabilistic software behave perfectly may be the wrong goal.

I still want to make it as reliable as I can.

But I’m also beginning to design for repair.

If the AI forgets something, can the person correct it?

If a game takes the story in the wrong direction, can the player tell it so?

If the system misunderstands your intention, have I taught you enough about how it works that you can recover instead of assuming the machine must be right?

That’s a very different relationship with software.

And it leaves me with a much bigger question.

Because I have kids.

What should they learn?

Should they learn the things I learned?

Variables.

Data structures.

Syntax.

All the machinery underneath the software?

Or should they spend that time learning how to describe what they want, judge what comes back, find the failure modes, and direct machines that already know how to do the underlying work?

I genuinely don’t know.

And I’m not sure anybody knows.

I think about it in music.

I’ve spent decades learning how to make sounds physically on a violin.

If I want a particular effect, I know what détaché is.

I know what ricochet is.

I know what pizzicato is.

I know what happens when I move the bow toward the fingerboard.

But imagine that instead of playing the instrument, my job becomes directing an instrument that can play itself.

I might simply say, “Make this sound spooky.”

The machine can figure out the low register, the articulation, the harmony, the texture.

So do I still need to know how those sounds are made?

Maybe.

Maybe not.

But I know that my ability to judge what the machine produces is deeply connected to having spent decades making those sounds myself.

And that’s the unresolved part for me.

I’m building AI systems right now partly because I think this may be where software is going.

I could also be early.

I could be wrong.

The things I’m making could work beautifully and find an audience.

Or I could discover that nobody wants them.

That’s okay.

The useful part isn’t dependent on that outcome.

Because I’m learning how to operate in a world where more and more things are probably right instead of provably right.

And I suspect that’s bigger than programming.

Maybe the important skill isn’t knowing how to make the machine obey.

Maybe it’s knowing what to do when it doesn’t.
