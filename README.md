# TIME BEFORE LIGHT

**The Auditory Prior as the Founding Architecture of Augmented Reality**

*HEAR — Holistic Emergent Augmented Reality*

ERI Labs · Eric Ren · Jersey City, New Jersey · github.com/ericrenone

---

> "The precedence effect: when two identical sounds arrive within a few milliseconds of one another, the auditory system localizes the pair toward the leader and suppresses the lag. The ear commits to a position before the room has finished speaking." — paraphrased synthesis of H. Wallach, E. B. Newman, M. R. Rosenzweig, *The Precedence Effect in Sound Localization*, American Journal of Psychology 62, 315–336, 1949

> "A neural place-map of auditory space is assembled in the midbrain from interaural time and level differences. The map exists before the animal turns its eyes — the gaze is sent to a coordinate the ear has already computed." — paraphrased synthesis of E. I. Knudsen and M. Konishi, *A Neural Map of Auditory Space in the Owl*, Science 200, 795–797, 1978

> "Time, when characterized as a noisy channel with statistical capacity, supports reliable communication." — synthesis of C. E. Shannon, *A Mathematical Theory of Communication*, Bell System Technical Journal 27, 1948

> "Vision comes from hearing what you see." — this work

---

## The Founding Axiom

Augmented reality has been built, without exception, around the visual overlay. Every shipping product, every prototype roadmap, every rendering pipeline treats the display as primary and sound as secondary feedback — a notification chime, a synthesized voice. This is not a missing feature. It is an inverted architecture.

The sensory physics is unambiguous. The ear resolves time at microsecond precision; the eye resolves space. In every animal that possesses both, the temporal precision of audition organizes the spatial map of vision — not the other way around. Sound arrives, is localized, and commits the system to a coordinate before the visual field has been processed into meaning. **Hearing is the prior. Seeing is the update.**

HEAR is the formal architecture of that relationship, built for the convergence of three things that did not exist together until now: wearable waveguide displays operating in shared physical space, the 2025–2026 audio-visual intelligence result that localization precedes grounding, and a quantum-networked substrate for fusing the perceptual priors of many observers into one map.

The title of this document is the conclusion of the framework, not its premise. Light is what the system renders. Time is what the system is built on. The auditory prior arrives first, and everything downstream — registration, attention, meaning, shared reality — is conditioned on it.

---

## Abstract

Five experimental and engineering traditions converge on a single architectural claim. Binaural psychophysics (the precedence effect, the Jeffress coincidence model, the barn-owl space map) establishes that auditory localization is computed faster and earlier than visual depth. Multisensory neuroscience (the superior colliculus space map, the ventriloquist and McGurk effects, modality-appropriateness weighting) establishes that when audition and vision disagree, the brain's fusion rule is not symmetric — each modality is weighted by its reliability *in the dimension being judged*, and audition wins time. The 2025–2026 audio-visual intelligence literature (the JAEGER and MEERKAT audio-visual grounding models, the AudioMiXR spatial-audio interface work, and the unified audio-visual intelligence synthesis of May 2026) converges independently on *listen first, look second*: sound-source localization precedes and organizes visual grounding. Information theory since Shannon establishes time itself as the channel across which all of this flows. And the ERI programme's col(F)/ker(F) partition of the Fisher information matrix provides the formal object that all four of the above are describing — the boundary between what is attended and what is background, drawn first in the auditory domain and only then confirmed visually.

HEAR is the architecture that takes *listen first, look second* as its founding axiom rather than as a downstream optimization. It treats the augmented-reality waveguide as a physical instantiation of the Fisher boundary, the binaural spatial map as the prior that places the overlay, and the auditory-visual binding cycle as a temporal phase register that selects the display mode. It adds a sixth perceptual dimension — **WHEN** — that no current AR system represents at all. And it specifies an emergent layer: when multiple HEAR observers share a space, their distributed auditory priors fuse, over a coordination substrate, into a collective spatial map that no single observer could compute alone.

Nine formal correspondences connect HEAR to the ERI architecture. Five falsifiable predictions follow. The HEAR machine is specified as an eight-layer instrument.

---

## Part I · The Thought Experiments

### I.1 — The Cocktail Party in the Dark

Stand in a crowded room with the lights off. A dozen conversations overlap. Someone three meters to your left, slightly behind, says your name.

Before you have turned your head, you already know where to turn it. You did not scan. You did not search. The auditory system extracted the interaural time difference — the fraction of a millisecond between the sound reaching your left ear and your right — and the interaural level difference, and from those two scalars it computed an azimuth to roughly one degree of precision. The motor command that rotates your gaze was issued *to a coordinate that hearing had already solved*.

Now turn the lights on and repeat. The visual system, with the full scene available, still cannot localize the speaker faster than the ear did in the dark. What vision adds is confirmation and detail — the face, the expression, the lip movements that sharpen the speech estimate. Vision is the update. The ear wrote the prior.

This is the entire HEAR thesis in one experiment. The col(F)/ker(F) boundary — the partition separating the attended speaker (col(F), the signal that has crossed into conscious processing) from the unattended murmur (ker(F), the background below the limen) — was drawn in the auditory domain. The eyes were sent to inspect a boundary that hearing had already located. An augmented-reality system that places its overlay using visual SLAM alone is redrawing, slowly and with jitter, a boundary that a binaural microphone pair could have handed it, stable and early.

### I.2 — The Trembling Overlay

For a decade the practical obstacle to wearable AR has been registration: the overlay shakes. A label pinned to a real object drifts and trembles because visual-only tracking — feature extraction, pose estimation, depth inference — is a heavy computation running behind the world. The render is always chasing.

Consider the same scene instrumented differently. A sound source in the environment — a voice, a machine, a moving vehicle — is localized binaurally at a latency and angular stability that visual depth computation cannot match. Use that binaural coordinate as the *prior* for overlay placement, and let the visual tracker supply only the high-spatial-frequency correction. The overlay stops trembling, not because the visual tracker improved, but because it is no longer the thing holding the position. It has been demoted to the update term in a filter whose prior is auditory.

This is the precedence effect, rebuilt as an engineering principle. The auditory estimate is the leader; the visual estimate is the lag; the system commits to the leader and uses the lag only to refine. Registration was never a graphics problem. It was a problem of asking the slow modality to do the fast modality's job.

### I.3 — The Triangulating Crowd

Three people stand in a large space, each wearing HEAR glasses. A sound originates somewhere none of them can individually localize — too far, too reverberant, too masked. Each observer's binaural system extracts a *partial* estimate: a bearing with wide uncertainty, a cone rather than a point.

Individually, three ambiguous cones. Fused, an intersection. The collective resolves a source that no member could resolve alone — not by averaging, but by conditioning each observer's prior on the others' through a shared substrate. This is the CONCERT result stated acoustically: the coordination gain is the mutual information between observers' estimates given the shared field, and it is strictly positive precisely when the artifact is doing coordination work rather than merely recording parallel observations.

HEAR's emergent layer is this triangulation made into infrastructure. The distributed auditory priors of co-located observers fuse into one spatial map, broadcast over the network substrate, and each observer's display renders its own view of a reality that the group computed and no individual held.

### I.4 — The Anticipation Gap

A door begins to open behind you. The hinge creaks. For a few hundred milliseconds there is sound and no visual confirmation — you have not yet turned. Then you turn: sound and vision are both live, fusing. Then your gaze settles on the door: vision dominant, the creak now background. Then the door is still: both signals fall below threshold.

You have just traversed the four phases of the auditory-visual binding cycle — **anticipation, binding, consolidation, release** — and each phase wanted a different thing from your perceptual system. During anticipation, the system should widen its spatial gate and raise its readiness. During binding, it should fuse hard and weight by reliability. During consolidation, it should let vision carry and free auditory resources. During release, it should return to baseline.

No augmented-reality system in existence represents this cycle. Every current device runs its display at a fixed frame rate, in a single mode, indifferent to where in the perceptual cycle the user actually is. HEAR introduces a temporal phase register that tracks the cycle and selects the display mode to match it. This is the sixth dimension. It is the dimension of time, and it is the one current AR omits entirely.

---

## Part II · The Six Dimensions

HEAR is not five questions bolted onto a headset. It is six axes of a single causal structure whose root is the perceptual boundary and whose leaves are action, meaning, and shared reality. Five are spatial-semantic. The sixth is temporal, and it is the one that organizes the rest.

### WHAT TO SEE — the signal
The attended object: what has crossed the Fisher boundary from background into col(F). In waveguide-display terms this is the overlay content. In HEAR terms it is the acoustic source that triggered foveation. The *what* is selected by audition before the visual scene graph has been parsed.

### WHO TO SEE — the agent
The person or entity that is the source or target of the attended signal — an identifiable actor in the causal structure. Auditory source separation delivers speaker identity before visual face recognition resolves. HEAR routes the *who* question through the auditory channel first and lets vision confirm.

### HOW TO SEE — the modality and channel
The transport channel and the perceptual eigenmode that selects which representation reaches conscious experience. In wearable terms this is the gesture or control that switches display modes; in HEAR terms it is the choice of spectral basis for cross-modal fusion.

### WHY TO SEE — the causal reason
The directed edge that explains why this signal crossed threshold *now*. The conserved quantity that forced attention. Auditory change — onset, offset, a shift in spatial location — is the most reliable trigger of the *why* signal, because temporal discontinuity is exactly what the ear is built to detect. HEAR treats auditory change detection as the primary *why* engine.

### WHERE TO SEE — the spatial coordinate
The aperture: the col(F)/ker(F) boundary in physical space. Binaural audio provides three-dimensional source localization at roughly one-degree azimuthal precision, earlier than any visual depth computation completes. HEAR uses the binaural spatial map as the prior for overlay placement. **This is the resolution of the decade-old registration problem** — the overlay is stabilized by an auditory ground truth instead of chasing a visual one.

### WHEN TO SEE — the temporal phase *(the hidden sixth dimension)*
The phase of the auditory-visual binding cycle. HEAR carries a temporal phase register with four states:

| Phase | Auditory–visual state | What the display should do |
|---|---|---|
| **Anticipation** | Audio onset, no visual confirmation yet | Widen spatial gate; raise readiness; pre-warm overlay near the auditory bearing |
| **Binding** | Audio and visual co-active; cross-modal fusion occurring | Fuse hard; weight each modality by its reliability; lock the overlay |
| **Consolidation** | Visual dominant; audio receding to background | Let vision carry; release auditory compute; stabilize, do not re-acquire |
| **Release** | Both signals below threshold | Return to baseline; dim the overlay; reset the register |

Each phase calls for a different display mode. A system that renders at a fixed rate, indifferent to phase, is spending its budget uniformly across a cycle that is radically non-uniform. The phase register is the mechanism that makes the display adapt to the perceptual cycle rather than to a clock.

---

## Part III · Time as the Channel

The sixth dimension is not an addition to the other five. It is their substrate. The reason audition can be the prior at all is that audition is the modality built natively in the time domain — and time, since 1948, has been understood as the channel across which information is carried.

Three foundational recognitions converge here. Shannon's noisy-channel coding theorem established that a temporally extended medium has a single quantitative parameter — capacity — that bounds reliable communication, and that any rate below capacity admits arbitrarily reliable transmission. The auditory channel is a Shannon channel: the interaural time difference is a temporal code, read off the relative arrival times at the two ears, and its precision sets the angular capacity of the localization estimate. Von Neumann's stored-program recognition established that time discretized into iterative state-transitions produces computation; the HEAR phase register is exactly such a discretized clock, four states deep, advancing the perceptual computation one binding cycle at a time. And the polyphase recognition — that time distributed across multiple synchronized phase-offset channels produces coherent emergent structure — is the binaural principle itself: two channels, left ear and right ear, offset by a phase that *is* the spatial information.

The 2025–2026 frontier sharpens this. Recent work extending channel capacity to finite-time and emergent-time settings treats time not as a parameter prior to the information substrate but as a structure emergent from it — time as a renormalization-group flow direction in the underlying theory. HEAR adopts the operational version of this stance: the temporal phase register is not a clock the system reads from outside. It is a coordinate the system computes from the cross-modal coherence signal — maximum coherence is the binding phase, minimum coherence is the release phase, and the phase variable is the flow between them. The system does not consult time. The system *derives* time, from the coherence of what it is hearing and seeing, and renders accordingly.

This is why the title is *Time Before Light*. The light — the rendered overlay — is the last thing the pipeline produces. The time — the auditory prior, the phase register, the coherence flow — is the first thing it computes, and everything visual is conditioned on it.

---

## Part IV · Nine Formal Correspondences

| ERI element | HEAR realization |
|---|---|
| **col(F)** | The attended audio-visual signal — the source that has crossed threshold and entered conscious processing; the content the waveguide renders |
| **ker(F)** | The perceptual background — the unattended soundscape and peripheral visual field, everything below the limen |
| **The Fisher boundary** | The AR waveguide itself: the lens is the physical instantiation of the col(F)/ker(F) separator, and HEAR formalizes what governs where that boundary sits and how it moves |
| **Conditional-independence boundary** | The auditory localization estimate — the prior that, once computed, renders the visual depth computation conditionally redundant for placement |
| **The prior / the update** | Auditory localization is the prior; visual grounding is the update. The precedence effect is this asymmetry as psychophysical law; *listen first, look second* is the same asymmetry as engineering result |
| **The five coordinate axes** | WHAT, WHO, HOW, WHY, WHERE are five geodesics on the Fisher manifold of perceptual space; the device tracks which geodesic the user is traversing |
| **Hamiltonian flow** | The temporal phase register is a Hamiltonian flow on the perceptual manifold; the system energy is cross-modal coherence — maximum at binding, minimum at release |
| **G_coord (coordination gain)** | The triangulating crowd: distributed auditory priors fused over the substrate yield a collective spatial map; positive coordination gain is the signature that the shared map exceeds the sum of individual estimates |
| **The channel** | Time itself — the auditory channel is a Shannon channel whose temporal code (interaural time difference) sets the angular capacity of every downstream visual placement |

---

## Part V · Five Falsifiable Predictions

**P1 — The auditory prior stabilizes registration.** An AR overlay placed using a binaural spatial prior, with visual tracking demoted to the correction term, will show measurably lower positional jitter than the same hardware running visual-only SLAM — and the improvement will be largest for sources that are acoustically salient and visually ambiguous (moving, occluded, low-contrast). Testable directly on existing waveguide hardware with an added binaural microphone pair.

**P2 — Localization latency precedes grounding latency, on-device.** Instrumenting a HEAR pipeline, the timestamp at which the auditory bearing is available will precede the timestamp at which the visual grounding resolves, by a margin consistent with the psychophysical precedence-effect window. The *listen first, look second* ordering will hold not just in passive video models but in first-person wearable use where the user is an active agent.

**P3 — The phase register reduces display power without perceptual cost.** A display that adapts its mode to the four-phase binding cycle — pre-warming during anticipation, locking during binding, coasting during consolidation, dimming during release — will consume less power than a fixed-rate display while producing equal or higher user-reported overlay stability, because compute is spent where the perceptual cycle actually demands it.

**P4 — Collective triangulation beats the best individual.** For a sound source that no single co-located HEAR observer can localize within a target precision, the fused collective estimate from three or more observers will reach that precision. The coordination gain will be strictly positive and will scale with the spatial diversity of the observers' positions — and will fall to zero if the observers are co-located, confirming that it is genuine triangulation and not averaging.

**P5 — Modality weighting follows reliability, dimension by dimension.** When HEAR's auditory and visual estimates are placed in controlled conflict, the fused overlay position will track whichever modality is more reliable *in the dimension being judged* — audition for timing and azimuth onset, vision for fine spatial detail — reproducing the modality-appropriateness rule of multisensory integration as an emergent property of the fusion layer rather than a hand-tuned parameter.

---

## Part VI · The HEAR Machine

HEAR is specified as an eight-layer instrument. Layer 0 is the environment; Layer 7 is shared reality. Each layer conditions on the ones below it.

**Layer 0 — The Acoustic-Optic Field.** The shared physical space: real sound sources, real surfaces, real light. The raw field that both the binaural microphone pair and the world-facing cameras sample.

**Layer 1 — Auditory Source Separation.** The incoming mixture is separated into candidate sources. Each source carries an interaural time difference and interaural level difference — the raw temporal code from which spatial position will be computed.

**Layer 2 — The Spatial Prior.** Binaural coincidence processing converts the temporal code into a three-dimensional source map at roughly one-degree azimuthal precision. This map is the prior. It exists before visual depth has been computed, and it is what every higher layer is conditioned on.

**Layer 3 — The Fisher Boundary Update.** The col(F)/ker(F) partition is drawn: which sources are signal, which are background. The boundary is drawn in the auditory domain first; the waveguide is the physical surface on which it will be rendered.

**Layer 4 — Cross-Modal Fusion.** The world-facing visual stream supplies the update. Auditory prior and visual estimate are fused, each weighted by its reliability in the dimension being judged. The overlay position is the posterior of this fusion — auditory-led, visually-refined.

**Layer 5 — The Temporal Phase Register.** The cross-modal coherence signal is read as a Hamiltonian flow, and the binding cycle is classified into one of four phases — anticipation, binding, consolidation, release. The phase determines the display mode for the next cycle.

**Layer 6 — Display Mode Selection and Query Resolution.** The waveguide overlay is positioned by the auditory spatial prior, not by visual-only SLAM. Its content is selected by resolving the WHAT / WHO / HOW / WHY / WHERE / WHEN queries against the fused scene. The mode — pre-warm, lock, coast, dim — is set by Layer 5.

**Layer 7 — The Emergent Collective Map.** The observer's auditory priors are broadcast over the coordination substrate and fused with those of every other co-located HEAR observer. The collective spatial map — the triangulated reality that no individual computed — is returned to each device, which renders its own view of it. This is the layer that makes HEAR *holistic* rather than merely multimodal: the perceptual boundary is no longer drawn by one nervous system, but by the network of them.

---

## Closing

The ear and the eye divide the labor of perception along a single axis, and that axis is time. The ear resolves it; the eye does not. In every animal that carries both, the fast modality writes the prior and the slow modality writes the update — the sound is localized, the gaze is sent, the scene is confirmed. The precedence effect is this law in the psychophysics. The midbrain auditory space map is this law in the anatomy. *Listen first, look second* is this law rediscovered, in 2025 and 2026, by the audio-visual intelligence literature working entirely from the engineering side.

Augmented reality inverted the law. It built the display first and treated sound as feedback, and it has spent a decade fighting a registration problem that was never a graphics problem. The overlay trembles because the slow modality was asked to do the fast modality's job. Hand the placement back to audition — let the binaural spatial prior lead and the visual tracker correct — and the tremor is not reduced, it is structurally removed, because the thing holding the position is no longer the thing that was always behind the world.

HEAR is the architecture that takes the law as its founding axiom. Six dimensions, the sixth of them time. An eight-layer pipeline whose root is the acoustic field and whose crown is a shared map. A temporal phase register that lets the display adapt to the perceptual cycle instead of to a clock. And an emergent layer in which the perceptual boundary is drawn not by one observer but by the network of them, each rendering its own view of a reality the group computed together.

The waveguide is the Fisher boundary made of glass. What governs where that boundary sits, and how it moves, and when, is not light. It is time — heard first, rendered last.

Vision comes from hearing what you see. The name is not metaphor. The name is the theorem.

---

ERI Labs · Eric Ren · Jersey City, New Jersey · github.com/ericrenone
