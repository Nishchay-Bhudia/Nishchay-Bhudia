# Nishchay Bhudia

Sixth-form developer in London. I build machine learning systems and the software
that has to sit around them to make them useful.

Most of what I work on starts because something specific annoyed me or somebody
needed it. A meditation teacher wanted to see what was happening in a student's
head during a sitting. A teacher's office chair kept going missing. A treasure
hunt needed every team to walk a genuinely different route rather than follow
each other. The interesting part is almost never the model. It is everything
between the sensor and the screen.

I am going into my final year at Woodhouse College taking Computer Science,
Maths and Economics, predicted A\*AA, finishing in 2027. I am looking for a
degree apprenticeship in software or machine learning.

## What I am working on

**Meditation Analyser.** A biofeedback platform for a meditation teacher and
their students. A consumer EEG headband streams four channels over Bluetooth,
and every four seconds the browser turns a window of that into a reading of the
practitioner's state of mind, or refuses to make a claim if the signal will not
support one. A .NET API does the signal processing, a Vue app drives the
headband over Web Bluetooth, and a Python implementation sits alongside both as
the reference the other two are tested against. It runs on Kubernetes, and it is
in real use, in English and Gujarati.
[See what it does](https://meditation-analyser.test.narnarayan.org/information)

**Adaptive Traffic Manager.** My A-Level coursework: a junction simulator that
pits an ordinary fixed-timer traffic light against a Deep Q-Network trained to do
the same job. Over thirty seeded runs each, the fixed timer won, 4.48 seconds of
mean wait per vehicle against the agent's 5.10. Writing up why my own AI lost
taught me considerably more than a win would have.

Alongside those: a what3words treasure hunt platform that gives every team a
provably different route, a fourteen-day TypeScript course that compiles and
grades submissions with the real compiler in a web worker, and a Zigbee motion
alarm for my house that exists because my router turned out not to expose the
WiFi data the original plan depended on.

## Things you can actually look at

| Repo | What it is |
|---|---|
| [Emotions Classifier CNN](https://github.com/Nishchay-Bhudia/Emotions-Classifier-CNN) | A convolutional network in PyTorch reading facial expression from a live webcam |
| [World Cup Match Predictor](https://github.com/Nishchay-Bhudia/WORLD-CUP-MATCH-OUTCOME-) | Predicts scorelines from 4,196 fixtures using Negative Binomial goal distributions and a learned Dixon-Coles term |
| [Intelligent Office Surveillance](https://github.com/Nishchay-Bhudia/Intelligent-Office-Surveillance-System) | Computer vision watching a room, built with a classmate after a chair went missing once too often |
| [Multilingual RAG](https://github.com/Nishchay-Bhudia/WEB-RAG) | Retrieval over scriptural texts in English, Gujarati and Sanskrit. It also answers questions on my portfolio |
| [Unbeatable Tic Tac Toe](https://github.com/Nishchay-Bhudia/Minimax-Tic-Tac-Toe) | Minimax searching the full game tree. The best you can force is a draw |
| [Linear](https://github.com/Nishchay-Bhudia/Linear-Regression) and [Logistic Regression](https://github.com/Nishchay-Bhudia/Logical-Regression) | Gradient descent by hand in NumPy, with no library doing the work |
| [Sorting and Searching Visualiser](https://github.com/Nishchay-Bhudia/Sorting-and-Search-algorithms) | Animated, so the gap between O(n squared) and O(n log n) is something you watch |
| [Impossible Platformer](https://github.com/Nishchay-Bhudia/Impossible-Platformer-Game) | A deliberately punishing Pygame platformer with pixel-mask collision |

A few of the bigger projects are private because they hold other people's data.
Happy to walk through any of them.

## What I have actually learned from this

That the bug is usually below the layer you are looking at. I spent months
tuning a classifier that was reading its input wrong: the decoder pulled nine
signed 16-bit samples out of a packet that holds twelve unsigned 12-bit ones.
That single mistake suppressed the alpha band by a factor of four and inflated
gamma by a factor of sixty. No amount of model work was ever going to fix it.

That a system should say "I do not know" out loud. The same project refuses to
classify roughly on demand rather than guessing, and the threshold for refusing
is computed from the maths instead of tuned until the demo looked good.

That two implementations of the same specification will silently disagree. Mine
agreed on 52.3 percent of stored results before I wrote fixtures that held them
to each other, and nothing in the build had noticed.

## Elsewhere

Mentored by the co-founders of Valyu AI and Navatech, working on production
TypeScript and LLM features. Two weeks of work experience at a London IT firm
sitting between clients and developers. Away from a keyboard I am an AV
technician and drone operator for events of a couple of thousand people at
Stanmore Temple, which I have been volunteering at for most of a decade, and I
run middle distance.

- Portfolio: [portfolio-gilt-two-10.vercel.app](https://portfolio-gilt-two-10.vercel.app)
- LinkedIn: [nishchaybhudia](https://linkedin.com/in/nishchaybhudia)
- Email: nishchaybhudia@gmail.com
