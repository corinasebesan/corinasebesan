## Corina Nicoleta Sebesan

Senior software engineer in Timisoara, Romania. Seven years of commercial experience, all of it on long-lived products: five years of C# and .NET on a desktop and web analytics platform, and seven of TypeScript across Angular and Preact.

I am most useful in the layer beneath the feature. Shared component libraries,
design systems, and the contracts that keep a large codebase coherent while six
applications are built on top of it.

Most of what is here is older work. In 2026 I went back through it, which turned
out to be more interesting than writing something new: the repositories below
are worth opening partly for what they do and partly for what I found in them.

### Worth opening

**[MedicalOnTime](https://github.com/corinasebesan/MedicalOnTime)** ·
Spring Boot, MySQL, React

A clinic appointment system from 2020 that had no working authentication at all.
The login screen asked for a password and never checked it, every endpoint was
open to anyone who could reach the port, and the database password was committed
to the repository. It now runs on Spring Security with BCrypt and JWT, with
authorisation in two layers: role rules on the URLs, and per record checks for
the things a URL pattern cannot express, like one patient reading another
patient.

**[PocketTravelGuide](https://github.com/corinasebesan/PocketTravelGuide)** ·
Java, Android, Google Maps

Which of 31 sights in Sibiu can you fit into one day, in what order, respecting
each one's opening hours? That is the orienteering problem with time windows,
and it is NP-hard. My bachelor's thesis solves it on the phone with a pulse
branch and bound: arc filtering before the search, a precomputed bounding oracle
that lets a branch die the moment it cannot win, and two-opt dominance checks.
The solver was finished in 2019 but never connected; the app shipped a hardcoded
route. It is connected now.

**[Tomatology](https://github.com/corinasebesan/Tomatology)** ·
Kotlin, TensorFlow Lite, Firebase

Ten tomato leaf diseases from a photograph. My master's thesis: a custom CNN
trained on 45,860 images, where a preprocessing pipeline in OpenCV took accuracy
from 82% to roughly 98% and beat all 28 off-the-shelf architectures I
benchmarked against it. The part I would point at first is not the model but the
delivery: quantised from 139 MB to 11 MB and shipped over the air through
Firebase ML, so a new model reaches users without an app release and can be A/B
tested in production against real photographs.

### Also here

[randommeal](https://github.com/corinasebesan/randommeal), a small AngularJS and
TypeScript app written to learn the tooling properly ·
[MusicHub](https://github.com/corinasebesan/MusicHub), the Android client from
an accelerator semifinal ·
[Hobby](https://github.com/corinasebesan/Hobby), my first Android project, from
2017

### Elsewhere

[LinkedIn](https://www.linkedin.com/in/corina-nicoleta-sebesan-b2679213a/) ·
sebesan.corina@gmail.com

Currently looking for a senior frontend or full stack role, remote or in
Timisoara.

<!--
**corinasebesan/corinasebesan** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
