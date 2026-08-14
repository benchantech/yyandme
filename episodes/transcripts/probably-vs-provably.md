I have spent much of my life in systems where the difference between probably and provably matters.

Software is an obvious example. If I write a function and give it the same inputs under the same conditions, I can often prove what it will do. I can inspect the code. I can write a test. I can reproduce the result. If the test fails, something is wrong. The system does not get credit because its answer was plausible.

Music is different. If a violinist plays a passage better on the second attempt, I can observe some things directly. The rhythm may have become steadier. A shift may have landed more accurately. A note may have spoken more clearly. But the explanation for the improvement is already less certain. Perhaps the player changed the bow speed. Perhaps the left hand released tension. Perhaps the first attempt simply prepared the second.

The observation may be provable.

The explanation is probably true.

Those are not the same thing.

Artificial intelligence has made this distinction much harder to ignore because large language models are extraordinarily good at producing the second kind of answer in the clothing of the first. They generate language confidently enough that a probable interpretation can feel like a demonstrated fact.

That does not make probabilistic reasoning defective. Much of human intelligence works this way too. We recognize patterns, infer causes, predict reactions, and act without complete information. A parent hears something unusual in a child’s violin playing and suspects what happened. A teacher watches a student’s hand and forms a hypothesis. A leader hears three versions of a problem and decides which explanation is most likely. Waiting for proof in every case would make ordinary life impossible.

The mistake is not acting on probability.

The mistake is forgetting that probability is what we are acting on.

I have been running into this repeatedly while building AI applications. Some parts of an application should be boringly provable. A player’s stated instrument should remain their instrument tomorrow. A choice recorded today should still exist next week. A safety rule should not disappear because another interpretation sounds more contextually elegant. If the application says an activity was completed, there should be evidence that it was completed.

These are bad places for probability.

But suppose the player writes, “That felt weird today and I don’t know why.”

Now probability becomes useful. A sufficiently rigid system can only reject the input or force it into predefined categories. An AI can interpret the description, connect it with earlier observations, generate a few plausible explanations, and suggest a useful next experiment.

That is exactly where I want it.

The architecture I increasingly prefer is therefore simple:

Deterministic systems govern. Probabilistic systems interpret and assist.

The boundary matters more than the slogan.

I have watched AI systems violate it in surprisingly subtle ways. A system may remember free-form text more reliably than a supposedly structured choice. An application simulator may confidently behave in a way its blueprint never intended. A coach may infer that a musician has improved because several signals point in that direction. None of these outputs is necessarily bad. Some may be excellent. But fluent behavior is not proof that the underlying system is behaving correctly.

This creates a peculiar engineering trap. When deterministic software fails, it usually looks broken. When probabilistic software fails, it may look insightful.

That is much more dangerous.

The same problem appears when AI analyzes music. A model may detect something concrete in a recording: a note began late, the tempo changed, the pitch moved, a second attempt differed measurably from the first. Those observations can become evidence. But when the model says why they happened, it has crossed an epistemic boundary.

Perhaps the player tightened the hand.

Perhaps the bow distribution caused the problem.

Perhaps attention moved elsewhere.

The correct response is not to prohibit the inference. It is to label it properly and make it cheap to challenge.

This is one reason I keep returning to bounded experiments. Instead of converting a plausible explanation into doctrine, change one thing and try again. Compare the attempts. Keep what survives contact with evidence. Discard what does not.

That is also why correction matters so much in an AI system. If the musician says, “No, that isn’t what happened,” the system should not defend the statistical elegance of its interpretation. The player’s correction becomes new evidence. The model revises.

Observation → interpretation → experiment → comparison → judgment.

The order matters.

The principle extends well beyond AI.

We routinely mistake proxies for proof. A streak proves that something was recorded on consecutive days; it does not prove commitment. Finishing a lesson proves completion; it does not prove understanding. Engagement proves interaction; it does not prove value. A polished plan proves that a plan exists; it does not prove that the plan is good. A confident explanation proves only that someone—or something—can produce a confident explanation.

Once noticed, the distinction becomes uncomfortable because very little of the interesting part of life is provable.

That is not an argument for paralysis. It is an argument for proportional confidence.

Some things I know.

Some things the evidence strongly suggests.

Some things are my best current explanation.

Some things are guesses worth testing.

Those categories should not collapse merely because language allows all four to be expressed with the same confidence.

This may be one of the most important disciplines for working with increasingly capable AI. The objective is not to make everything deterministic. That would throw away much of what makes these systems valuable. Nor is the objective to trust the probabilistic system because it is usually right. “Usually right” is precisely the condition that requires judgment.

Instead, I want to push each kind of problem toward the system best suited to it.

If something must remain true, encode it.

If something can be tested, test it.

If something can be observed, preserve the observation.

If something must be inferred, infer it—but preserve the uncertainty.

If something requires judgment, do not quietly convert the inference into the decision.

This is where the distinction intersects with the principle underneath much of my work with the YY Method: outsource execution; never outsource judgment.

AI can produce the probable answer astonishingly quickly. That is leverage. It can generate hypotheses I would not have considered, notice patterns across information I could not hold simultaneously, and make messy situations tractable.

But probability should create options for judgment, not impersonate judgment itself.

And proof has its own limitation. What can be proved is constrained by what we decided to measure, encode, and test. A deterministic system can perfectly enforce the wrong rule. A metric can precisely measure the wrong thing. A regression suite can prove that software behaves exactly as specified while the specification itself remains foolish.

Provably correct is therefore not the same as wisely chosen.

That final step still belongs somewhere else.

Perhaps that is the deeper resonant pattern.

We need probably because the world is larger than what we can prove.

We need provably because our stories about the world are easier to believe than they deserve to be.

And we need human judgment because neither probability nor proof can decide, by itself, what deserves to govern.
