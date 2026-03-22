# INFO5995 Assignment 1 - Activity Log

## Group Members
- Member A: Tareq Alsubaie
- Member B: Bharathwaj Murali
- Member C: Peisen Zheng
- Member D: Nishanth Shanmugasundaram
- Member E: Shyam Karthick Venkatraman Balakrishnan

## Contribution Matrix

### Row 1 - Written by Tareq Alsubaie
- Tareq on Tareq: I decompiled the APK, identified the key classes for registration, login, and profile, confirmed that the main in-scope issue was the weak randomness used for session token generation, improved the wording and structure of the report, and helped produce the PoC demo video.
- Tareq on Bharathwaj: Bharathwaj reviewed the decompiled source, mapped the main components and local storage, built the system model and data-flow summary, and helped connect the attacker capabilities to the protected assets in the report.
- Tareq on Peisen: Peisen searched the code for random, token, and session-related values, verified that `java.util.Random` was used in `Login.generateSessionToken()`, created the slides, and edited the PoC README.
- Tareq on Nishanth: Nishanth drafted and refined the threat model, attacker capabilities, attack scenario, vulnerability explanation, and mitigation wording for the written report.
- Tareq on Shyam: Shyam helped organise the presentation flow, reviewed the content for consistency, supported rehearsal and timing, and contributed to coordination and final submission organisation.

### Row 2 - Written by Bharathwaj Murali
- Bharathwaj on Tareq: Tareq led the initial APK inspection, helped the group understand the login flow, local credential handling, and session creation logic, and also improved the final report and PoC demonstration material.
- Bharathwaj on Bharathwaj: I focused on the system model, identified the protected assets and important data flows, linked them to the local authentication design of the app, and helped frame the attacker capabilities used in the threat model.
- Bharathwaj on Peisen: Peisen carried out targeted code searches for randomness-related APIs, recorded the exact code location of the insecure session token generator, and prepared the slide deck and PoC README.
- Bharathwaj on Nishanth: Nishanth helped write and edit the vulnerability explanation, especially why `java.util.Random` is unsuitable for a security-sensitive session token, how the attack scenario should be described, and why `SecureRandom` is the correct fix.
- Bharathwaj on Shyam: Shyam assisted with presentation logistics, timing, rehearsal planning, and review of the final submission package, and helped keep the team output consistent.

### Row 3 - Written by Peisen Zheng
- Peisen on Tareq: Tareq helped validate the main vulnerability with direct code evidence, made sure our selected issue matched the assignment scope on randomness and cryptography, polished the document, and supported the PoC demo video.
- Peisen on Bharathwaj: Bharathwaj created the system and threat model summary, identified key assets and data flows, made the attacker capabilities realistic and consistent with the app design, and helped keep the model aligned with the vulnerability we selected.
- Peisen on Peisen: I searched for all values treated as random, token, or session-related, compared their security roles, confirmed that the session token in `Login` was the main security-relevant weak usage, created the slides, and edited the PoC README.
- Peisen on Nishanth: Nishanth drafted the attack scenario and mitigation section, including the recommendation to replace `java.util.Random` with `SecureRandom`, edited the report wording, and helped align the report with the rubric.
- Peisen on Shyam: Shyam helped review the presentation flow, supported coordination work, contributed to rehearsal and timing checks, and assisted with final checking and packaging before submission.

### Row 4 - Written by Nishanth Shanmugasundaram
- Nishanth on Tareq: Tareq contributed strongly to reverse engineering and validation of the code paths related to registration, login, and local authentication state, and also improved the final document and PoC demo preparation.
- Nishanth on Bharathwaj: Bharathwaj documented the app structure clearly and helped connect components, assets, data flows, and attacker assumptions in a consistent system model.
- Nishanth on Peisen: Peisen produced the clearest technical evidence for the randomness issue by locating the generator API, token format, and local storage references, and he also prepared the slide deck and updated the PoC README.
- Nishanth on Nishanth: I wrote major parts of the threat model, vulnerability explanation, attack scenario, and fix section, and helped align the write-up with the rubric requirements and presentation focus.
- Nishanth on Shyam: Shyam supported presentation preparation, contributed to final content review, helped rehearse timing and speaking order, and helped organise the submission materials and group coordination.

### Row 5 - Written by Shyam Karthick Venkatraman Balakrishnan
- Shyam on Tareq: Tareq was central to the technical analysis of the APK, helped validate that the group claims matched the decompiled source, improved the report wording, and contributed to the PoC demo video.
- Shyam on Bharathwaj: Bharathwaj made the system model more precise by identifying the main components, assets, data flows, and attacker assumptions used in the report and slides.
- Shyam on Peisen: Peisen was mainly responsible for code searching and evidence collection on randomness-related values, helped justify why the chosen vulnerability was security-relevant, and also made the slides and edited the PoC README.
- Shyam on Nishanth: Nishanth helped turn the technical findings into a clear written explanation, especially the attacker model, exploitation path, mitigation rationale, and final report refinement.
- Shyam on Shyam: I supported presentation preparation, reviewed the final materials for consistency, helped with coordination, rehearsal, and timing, and contributed to organising the final submission package.

