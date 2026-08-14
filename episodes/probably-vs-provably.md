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

AI makes probable answers feel provable, which makes the boundary between inference and evidence matter more.

This episode traces the difference between observations we can preserve, explanations we can only infer, and decisions that require human judgment. It moves through software, music practice, AI applications, bounded experiments, and the YY Method principle to outsource execution without outsourcing judgment.

**Keywords**: AI judgment, probabilistic systems, deterministic software, evidence and inference, bounded experiments, YY Method
{: .ep-keywords}

🎧 **Start with [The First Echo](https://yyandme.benchantech.com/the-first-echo)** — then leave a trace. Your feedback shapes this podcast.

{% include episode-navigation.html %}

<div class="section-rule transcript-rule">
  <span class="label">FULL TRANSCRIPT</span>
  <span class="line"></span>
</div>
<div class="transcript-paper">
<p>I have spent much of my life in systems where the difference between probably and provably matters.</p>
<p>Software is an obvious example. If I write a function and give it the same inputs under the same conditions, I can often prove what it will do. I can inspect the code. I can write a test. I can reproduce the result. If the test fails, something is wrong. The system does not get credit because its answer was plausible.</p>
<p>Music is different. If a violinist plays a passage better on the second attempt, I can observe some things directly. The rhythm may have become steadier. A shift may have landed more accurately. A note may have spoken more clearly. But the explanation for the improvement is already less certain. Perhaps the player changed the bow speed. Perhaps the left hand released tension. Perhaps the first attempt simply prepared the second.</p>
<p>The observation may be provable.</p>
<p>The explanation is probably true.</p>
<p>Those are not the same thing.</p>
<p>Artificial intelligence has made this distinction much harder to ignore because large language models are extraordinarily good at producing the second kind of answer in the clothing of the first. They generate language confidently enough that a probable interpretation can feel like a demonstrated fact.</p>
<p>That does not make probabilistic reasoning defective. Much of human intelligence works this way too. We recognize patterns, infer causes, predict reactions, and act without complete information. A parent hears something unusual in a child’s violin playing and suspects what happened. A teacher watches a student’s hand and forms a hypothesis. A leader hears three versions of a problem and decides which explanation is most likely. Waiting for proof in every case would make ordinary life impossible.</p>
<p>The mistake is not acting on probability.</p>
<p>The mistake is forgetting that probability is what we are acting on.</p>
<p>I have been running into this repeatedly while building AI applications. Some parts of an application should be boringly provable. A player’s stated instrument should remain their instrument tomorrow. A choice recorded today should still exist next week. A safety rule should not disappear because another interpretation sounds more contextually elegant. If the application says an activity was completed, there should be evidence that it was completed.</p>
<p>These are bad places for probability.</p>
<p>But suppose the player writes, “That felt weird today and I don’t know why.”</p>
<p>Now probability becomes useful. A sufficiently rigid system can only reject the input or force it into predefined categories. An AI can interpret the description, connect it with earlier observations, generate a few plausible explanations, and suggest a useful next experiment.</p>
<p>That is exactly where I want it.</p>
<p>The architecture I increasingly prefer is therefore simple:</p>
<p>Deterministic systems govern. Probabilistic systems interpret and assist.</p>
<p>The boundary matters more than the slogan.</p>
<p>I have watched AI systems violate it in surprisingly subtle ways. A system may remember free-form text more reliably than a supposedly structured choice. An application simulator may confidently behave in a way its blueprint never intended. A coach may infer that a musician has improved because several signals point in that direction. None of these outputs is necessarily bad. Some may be excellent. But fluent behavior is not proof that the underlying system is behaving correctly.</p>
<p>This creates a peculiar engineering trap. When deterministic software fails, it usually looks broken. When probabilistic software fails, it may look insightful.</p>
<p>That is much more dangerous.</p>
<p>The same problem appears when AI analyzes music. A model may detect something concrete in a recording: a note began late, the tempo changed, the pitch moved, a second attempt differed measurably from the first. Those observations can become evidence. But when the model says why they happened, it has crossed an epistemic boundary.</p>
<p>Perhaps the player tightened the hand.</p>
<p>Perhaps the bow distribution caused the problem.</p>
<p>Perhaps attention moved elsewhere.</p>
<p>The correct response is not to prohibit the inference. It is to label it properly and make it cheap to challenge.</p>
<p>This is one reason I keep returning to bounded experiments. Instead of converting a plausible explanation into doctrine, change one thing and try again. Compare the attempts. Keep what survives contact with evidence. Discard what does not.</p>
<p>That is also why correction matters so much in an AI system. If the musician says, “No, that isn’t what happened,” the system should not defend the statistical elegance of its interpretation. The player’s correction becomes new evidence. The model revises.</p>
<p>Observation → interpretation → experiment → comparison → judgment.</p>
<p>The order matters.</p>
<p>The principle extends well beyond AI.</p>
<p>We routinely mistake proxies for proof. A streak proves that something was recorded on consecutive days; it does not prove commitment. Finishing a lesson proves completion; it does not prove understanding. Engagement proves interaction; it does not prove value. A polished plan proves that a plan exists; it does not prove that the plan is good. A confident explanation proves only that someone—or something—can produce a confident explanation.</p>
<p>Once noticed, the distinction becomes uncomfortable because very little of the interesting part of life is provable.</p>
<p>That is not an argument for paralysis. It is an argument for proportional confidence.</p>
<p>Some things I know.</p>
<p>Some things the evidence strongly suggests.</p>
<p>Some things are my best current explanation.</p>
<p>Some things are guesses worth testing.</p>
<p>Those categories should not collapse merely because language allows all four to be expressed with the same confidence.</p>
<p>This may be one of the most important disciplines for working with increasingly capable AI. The objective is not to make everything deterministic. That would throw away much of what makes these systems valuable. Nor is the objective to trust the probabilistic system because it is usually right. “Usually right” is precisely the condition that requires judgment.</p>
<p>Instead, I want to push each kind of problem toward the system best suited to it.</p>
<p>If something must remain true, encode it.</p>
<p>If something can be tested, test it.</p>
<p>If something can be observed, preserve the observation.</p>
<p>If something must be inferred, infer it—but preserve the uncertainty.</p>
<p>If something requires judgment, do not quietly convert the inference into the decision.</p>
<p>This is where the distinction intersects with the principle underneath much of my work with the YY Method: outsource execution; never outsource judgment.</p>
<p>AI can produce the probable answer astonishingly quickly. That is leverage. It can generate hypotheses I would not have considered, notice patterns across information I could not hold simultaneously, and make messy situations tractable.</p>
<p>But probability should create options for judgment, not impersonate judgment itself.</p>
<p>And proof has its own limitation. What can be proved is constrained by what we decided to measure, encode, and test. A deterministic system can perfectly enforce the wrong rule. A metric can precisely measure the wrong thing. A regression suite can prove that software behaves exactly as specified while the specification itself remains foolish.</p>
<p>Provably correct is therefore not the same as wisely chosen.</p>
<p>That final step still belongs somewhere else.</p>
<p>Perhaps that is the deeper resonant pattern.</p>
<p>We need probably because the world is larger than what we can prove.</p>
<p>We need provably because our stories about the world are easier to believe than they deserve to be.</p>
<p>And we need human judgment because neither probability nor proof can decide, by itself, what deserves to govern.</p>
</div>
