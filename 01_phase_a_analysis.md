# Phase A: Ethical Analysis of Synthetic Representation

*Reasoning outward from the artifact I built in Task 6*

**Sources.** My Task 6 repository: [INSERT TASK 6 REPOSITORY URL]. I refer to `script.md`, `process_log.md`, `detection_results.md`, the README, and the two artifacts (`attempt1_[Elevenlabs]_tts_SYNTHETIC.mp3` and the D-ID lip-sync video). Everything I say about what I built comes from those logs. Every scenario in Section 3 is invented by me; as the assignment instructs, I did not research documented incidents. Where my reasoning is unstable, I say so.

---

## 1. What I built (for a reader who has not seen Task 6)

| Element | What I did |
|---|---|
| Script | An analytical explainer, "Should We Pilot a Four-Day Work Week?", whose claims I verified in Task 5. It includes its own caveat: the evidence comes from self-selected employers, and much of the productivity data was self-reported. |
| Voice | ElevenLabs free tier. Stock voice "Steven: Natural, Kind and Steady." Stability 50, similarity 50, style 41, speed 1.07. Free-tier limits: 10,000 characters per month, a limited set of stock voices, 128 kbps MP3. **One attempt, about 40 minutes, no refusals, errors or truncations.** |
| Video | D-ID free-tier photo-to-video. The presenter is a tool-supplied synthetic presenter, not my face and not my voice, standing in the tool's stock "creative office" set (chalkboard covered in words like COMMUNICATION and TEAMWORK, pendant bulbs). The audio was the ElevenLabs file. The frame carries a tiled semi-transparent D-ID watermark. |
| Detection | Hive Moderation, one upload of the video: **0.8% likelihood AI-generated, 0% deepfake, classification "No deepfake / no manipulation detected," no explanation given.** |
| Disclosure | A `_SYNTHETIC` suffix in the filenames and a disclosure banner in the repo README. The only label inside the pixels was the vendor's watermark. |
| My own evaluation | The video held up to a casual glance. Closer inspection showed stiff blinking and a flat emotional register that did not match the script's content. The audio was fluent, but the pacing in paragraphs two and three felt rushed. |

---

## 2. Returning to what I built

### 2.1 Ethical questions the artifact raises even though it was honest

**The honesty is not in the file.** My script was true because of work I did in Task 5, and that work leaves no trace in the output. A viewer sees a calm voice and a presenter in an office. A fabricated script would produce a file with the identical surface. Whatever made my artifact acceptable was a property of my process, not of the media, and the media cannot carry it.

**A speaker who cannot be questioned.** The script contains a deliberate hedge: "Here's the honest caveat: these are self-selected employers." A human saying that line pauses, shifts, signals how much weight to put on it. The synthetic presenter delivered the caveat at the same pace and tone as the headline statistics. My Task 6 evaluation recorded the flat emotional register as a craft flaw. Reading it again, I think it is also an ethical loss: audiences calibrate trust from a speaker's hesitations, and the synthetic presenter removes that signal. It is also a flaw the tools will likely fix, so I should not rely on it as protection.

**Borrowed trust cues, chosen from a menu.** The voice was labeled "Natural, Kind and Steady." The set had a chalkboard reading COMMUNICATION and TEAMWORK. I did not design either of these trust signals; I picked them from a vendor menu at no cost. Part of what makes synthetic representation persuasive is that credibility signals are now product features.

**My labels sat outside the media.** The filename suffix and README banner describe the file; they are not part of what a viewer sees. The only in-frame signal was the vendor's watermark, which (as I understand it, and I have not verified this) is a feature of the free tier rather than a safety mechanism. So my disclosure was honest but fragile by construction. Section 3 (context axis) follows this through.

### 2.2 What the log records but understates

The process log records the voice attempt in three lines: one try, no refusals, forty minutes. That is the finding. A fluent synthetic voice in a trustworthy register took a single pass, and the only complaint I logged was pacing. The distance between "honest, careful, labeled" and "convincing enough" turned out to be very small, and it was crossed by choosing from menus.

### 2.3 Where the tools refused or degraded

They did not refuse anything. That is worth stating plainly rather than inventing a limit I did not hit. I used a stock voice, a tool-supplied presenter and an honest script, and I did not, and will not, test the boundaries with anyone's real likeness. So I cannot infer the vendors' safety systems from my experience; the absence of refusal tells me only that a benign use is unimpeded.

The friction I did meet was commercial: a 10,000-character monthly cap, a limited voice set, a bitrate cap, a watermark. These are pricing tiers, not principles. What the vendors visibly protect is their upgrade path; what they protect against, I could not observe.

One more gap I should name: I did not verify how the stock voice or the presenter were originally sourced. My "no consent issue" statement in the Task 6 ethics note rested entirely on the vendor's menu. Consent can be laundered upstream, where I cannot see it.

### 2.4 What I would not build again

Nothing in Task 6 is something I would refuse to rebuild. What I would change is the labeling: I would burn the label into the frame from the start rather than relying on filenames and a README that do not travel with the video. And there are versions of this artifact I would refuse to build at all, discussed in Section 5.

---

## 3. Reasoning across the axes

### 3.1 Truth axis: "The reassurance memo"

*Scenario.* An employee at a mid-sized firm opens the same two free-tier tools I used. She writes a 300-word script in the register of my Task 6 script (statistics, a mild-sounding caveat, a decision rule), but the facts are invented: the executive team has approved a permanent four-day week at full pay starting next month, and staff should tell clients Fridays are no longer available. She picks a calm stock voice and a presenter in an office. It takes her an afternoon. It goes out in a team chat on a Friday. By Monday, three people have told clients, one has cancelled a Friday appointment, and the CEO has to issue a correction. The correction is text; the fabrication was a person-shaped presenter speaking calmly. Some employees keep believing the video.

*What changes ethically.* Nothing changes in the pipeline, and that is the point. What made my artifact acceptable, that it was true, is not a property of the file. Nobody can tell my verified script from her fabricated one, because both are flat, fluent and calm. Even my hedging ("here's the honest caveat") is a style a forger can imitate; hedging is cheap and may even raise credibility. So truth cannot be recovered from the format. It has to be recovered from provenance of the claim: who stands behind it and can be asked.

*Where I'm unsure.* I do not know whether audiences can learn to treat any unsourced video as rumor, or whether norms shift more slowly than tools do.

### 3.2 Consent axis: two scenarios

*Scenario A (malicious).* A finance clerk gets a voicemail in the regional director's voice asking her to release a vendor payment before a deadline. The voice was cloned from a twenty-second segment of a recorded town hall on the intranet. The director never said it and knows nothing about it, yet his voice is the instrument of the fraud.

*Scenario B (benign).* A training team has twelve onboarding videos narrated by Marta, who left the firm in the spring. A new regulation means the modules need updating. The team clones Marta's voice from the old videos to narrate the new versions; nobody asks her, because the firm owns the videos. There is no malice and no lie about the content. But Marta's voice now says things she never approved, under a credit that may still carry her name.

*What changes ethically.* In my artifact the speaker was nobody, so nobody could be wronged by what was said. Once the voice belongs to someone, three things attach. First, they become answerable for utterances they did not make. Second, they lose control over future speech: a photograph shows one moment, but a voice model speaks on demand, indefinitely. Third, consent has a scope and a time limit that a file does not carry. Scenario B is the more instructive one because good intentions do the harm. A policy that only forbids "malicious" use misses it entirely; the boundary is authorization, not intent.

*Where I'm unsure.* Whether any consent can be fully free inside an employment relationship is a question I cannot settle. I return to it in the policy limitations.

### 3.3 Context axis: "The six-second clip"

*Scenario.* My video's disclosure lived in three places: the `_SYNTHETIC` filename, the README banner, and the tiled watermark. Follow the file out of my repo. Someone downloads it and forwards it through a chat app; the filename changes and the README is not attached. Only the watermark remains, and it exists only because of the pricing tier. Now suppose an employee trims six seconds from the final paragraph, the part saying the risk of a short, reversible pilot is low relative to the documented upside, and posts it in a group chat captioned "our analysts say the four-day week is low risk." The caveat about self-selected employers, which came before that sentence, is gone. Every word in the six seconds is true. The presenter is unlabeled in any way that survived the excerpt.

*What changes ethically.* A label attached to a file is not a label attached to a viewing. The second-hand viewer is a different person from the audience I imagined and has none of the surrounding context. Also, true content can be turned misleading by selection alone, without fabrication. A synthetic presenter makes this worse: there is no human who can say "that is not what I meant." Screen recordings and platform re-encoding would erase any metadata, so the only labels that can survive are ones inside the frame, and even those depend on viewers not having learned to ignore overlay text.

*Where I'm unsure.* Whether a burned-in label truly helps once audiences become habituated to it.

### 3.4 Scale axis: "Every department gets its own version"

*Scenario.* The free tier's 10,000 characters per month, against a script of roughly 2,000 characters, allowed me on the order of five such passes a month. That friction is commercial, and disappears with a paid plan or more accounts. Suppose someone with a paid plan and a spreadsheet of 250 employees generates 250 versions of a benefits announcement, each in the voice of that employee's own manager, each saying something slightly different about what changes for that team. No two copies match. When employees compare notes they cannot tell which are real. The following week the CEO's real all-hands video is dismissed by some as "probably another fake."

*What changes ethically.* Two harms appear that do not exist at n=1: personalized deception (each viewer is targeted with the version most likely to move them), and the liar's dividend (real evidence becomes deniable because fakes are known to exist). Scale also breaks the defenses. My own detection test was a single upload of a single file. Verification costs are per item, production costs are close to zero, and that asymmetry favors the producer.

*Where I'm unsure.* I do not know at what volume the effect on trust becomes systemic rather than incident-by-incident. I am reasoning about the direction, not the threshold.

### 3.5 An axis of my own, register and authority: "The redundancy notice"

*Scenario.* A firm loses a major client and decides to announce redundancies by video, using the same calm voice and presenter as its other explainers, "to keep the tone consistent and save the CEO's time." Nobody is deceived about a single fact.

*What changes ethically.* The recipients are addressed by no one. There is nobody to look in the eye, nobody whose discomfort shows, nobody to ask a question. What is wrong is not falsehood but the removal of accountability that normally attaches to delivering consequential news: the voice and face borrow the authority of a person who is not there. My Task 6 README noted that the video's emotional register was flat and mismatched to the content; this scenario turns that observation from a craft flaw into a moral one. Even if the tools learn to fake appropriate gravity, the accountability gap remains. This axis produced the clearest rule in my policy.

*Where I'm unsure.* Where the line falls between consequential news and routine information. Changed parking rules? A new benefits vendor? The policy draws a line, but I am not confident it sits in exactly the right place.

---

## 4. The mitigation landscape

For each mitigation: what it promises, where it breaks, and what my Task 6 experience adds. None of these is a solution.

**Disclosure (labels, watermarks, spoken acknowledgments).**
*Promise:* the viewer knows what they are looking at. *Works when:* the label is prominent, persistent, in-frame, in the viewer's language, and the viewer is the intended audience. *Breaks:* it is stripped, cropped, excerpted or ignored; muted viewers miss spoken labels; second-hand viewers never see it; and there is a selection effect, since honest actors label and bad-faith actors do not. *Task 6:* my labels were a filename and a README, both external to the pixels. The only in-frame label was a vendor watermark I did not design.

**Provenance and content credentials (C2PA and similar).**
*Promise:* a signed record of how a file was made and edited, verifiable later. *Breaks:* metadata is commonly stripped by re-encoding, screenshots and screen recording; the absence of credentials proves nothing because most authentic media has none; adoption depends on generation tools and platforms opting in; and a signature shows who signed, not that the content is true. *Task 6:* I have to be honest here. In Task 6 I tested detection, not provenance. I did not verify whether my files carried credentials or whether they would survive re-encoding, so I have no finding to report. What I can say from my artifact is that its provenance was text: self-attested, unsigned, lost by a rename. In Phase B I therefore assume credentials will often be stripped and back them with an organization-held register that does not depend on metadata surviving.

**Detection (automated detectors and forensics).**
*Promise:* flag synthetic media without needing the creator's cooperation. *Breaks:* detectors are trained on yesterday's generators; scores can be confidently wrong; results often come with no explanation; and a low score invites false reassurance. *Task 6:* Hive scored my known-synthetic video at 0.8% AI-generated and 0% deepfake, with no reasoning. That is n=1: one tool, one file, one consumer pipeline. But the miss is what matters, and it points somewhere uncomfortable. A bad-faith actor can run their output through public detectors before release and iterate until it passes. My test was, in effect, the first step of that loop. The generalization that detectors structurally trail generators is my reasoning from one data point, not something I measured.

**Legal and regulatory regimes (the shape of the terrain).**
*Promise:* deterrence and remedy. The kinds of measures I am aware of include disclosure requirements for synthetic content (especially in political advertising), statutes on non-consensual intimate imagery, right-of-publicity and likeness laws, existing fraud and impersonation law, privacy rules on biometric identifiers, and platform takedown duties. *Breaks:* a patchwork across jurisdictions; slow relative to the harm; dependent on identifying the actor; constrained by free-speech and parody carve-outs; and largely silent on cases like Marta's, where no one intended harm. I have not verified the current text of any of these, and they change quickly, so my policy treats law as a floor rather than a design basis.

**Platform policy.**
*Promise:* labeling or removal of deceptive synthetic media at scale. *Breaks:* self-declaration relies on honest uploaders; automated enforcement inherits the limits of detection; enforcement is uneven; and re-sharing across platforms defeats any one platform's rules. In the setting I chose for Phase B, there is no outside platform: the organization's own intranet and chat tools are the platform, so the organization has to be its own enforcer.

**Professional and organizational norms.**
*Promise:* shared expectations enforced by reputation. Journalism generally expects disclosure of AI use and that no events be depicted that did not happen; advertising has truth-in-advertising duties; education has acceptable-use policies; political consulting has scattered pledges. *Breaks:* voluntary, uneven, and slow to keep pace. And some settings have no norm at all. Internal communications and HR, the setting I chose, have none I know of, which is part of why I chose it.

**Synthesis.** The mitigations that worked on my artifact were the ones I supplied myself (disclosure, my own honest process). The one that operated independently of me, detection, failed. That suggests these tools mostly catch honest actors, because they depend on cooperation, and the tool that does not depend on cooperation is the one that missed. Why keep them at all? Because they raise cost, establish norms, give good-faith actors a way to comply, and give investigators something to work with afterward. They do not prevent a determined adversary, and any policy that pretends otherwise is complacency.

---

## 5. Engaging the research questions

**What becomes dangerous?** Not the technology alone, and not scale alone. The danger is the combination: a borrowed authority register (calm human voice, office setting) that costs nothing to obtain, separated from an accountable speaker, at near-zero marginal cost. Remove any one and the danger shrinks; my Task 6 artifact had the first two and, at n=1, not the third.

**Do the mitigations that would have caught mine catch a bad-faith actor's?** Mostly no. See the synthesis above. What remains is institutional: registers, callback verification, and clear rules about who is allowed to speak for whom.

**Is there a use I would refuse regardless of policy?** Yes: any synthetic presenter speaking as a specific real person whose words they have not approved, and any use of a synthetic presenter to deliver consequential news to the people affected. I can state both as rules (a synthetic speaker must never carry someone else's accountability). Whether they began as rules or as instincts I cannot honestly reconstruct.

**Who bears the burden: producer, platform, audience or regulator?** If I had the authority, I would place primary accountability on the producer and the organization that publishes, because they alone know what is true and who consented. Platforms and regulators come second, since they act after the fact and at scale. The audience should carry the least burden, and the current situation shifts the most onto them: asking every viewer to authenticate every clip is unworkable.

**Would a different context change my policy?** Yes, materially. The consent rules (employees under a power asymmetry) and the "no bad news" rule are specific to an internal employer setting; a newsroom would center on never depicting events that did not occur, and a campaign on impersonation of candidates. What seems portable is the accountable-human requirement, the register, and the refusal to let labeling substitute for judgment.

**Where my reasoning is unstable.** (1) Whether employee consent can ever be truly free. (2) Where "consequential news" ends. (3) Whether burned-in labels help once viewers habituate to them. (4) Whether my single detection result generalizes.

---

## 6. What Phase A hands to Phase B

| Finding | Where it lands in the policy |
|---|---|
| Truth is not carried by the file, so someone must be accountable for the claim | Named Responsible Human on every piece (Sections 2, 6, 8) |
| A synthetic speaker removes accountability for consequential news | Prohibition on bad-news delivery (P3) and refusal conditions (Section 10) |
| Consent is about authorization and scope, not intent; consent can be laundered upstream | Consent workflow (Section 5); vendor sourcing check (5.9); the Marta case (P7) |
| Labels outside the pixels do not travel; excerpts mislead | In-frame burned-in labels, excerpt rules, caveat-proximity rule (Section 6) |
| Metadata and detectors fail; verification has to live outside the file | Organization-held register and employee callback rule (Section 7) |
| Scale collapses per-item verification | No synthetic media for individualized or mass messages beyond approved categories; audit reconciliation (Section 11) |
