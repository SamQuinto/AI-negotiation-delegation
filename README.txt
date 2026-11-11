Negotiation Arena editable configuration
Application v33. Updated 11 November 2026.

Public app: https://play.the-negotiation-arena.workers.dev/
Fresh participant preview: https://play.the-negotiation-arena.workers.dev/try
Protected developer preview: https://play.the-negotiation-arena.workers.dev/preview
Administration: https://play.the-negotiation-arena.workers.dev/admin

Editable files
cases.json: original stories, private role values, explicit issues/options, role names and BATNA backstories.
parameters.json: legacy fee equations, score calibration, legal range, timing and no-deal values.
ai-prompts.json: named specialists, scope gate, concise voice and evidence-based dashboard review.
study-protocol.json: an editable protocol example. Actual saved runtime protocol may differ.
neggy-guide.json: warm-up and transition guide content.
update-log.json: timestamped changes and five-category quality review. Separate deployment receipts confirm publication.
AI_and_study_guide.txt: mechanics, analysis and operating notes.

Use Admin > Case files to validate/apply parameters, cases or prompts, including their raw GitHub links. Recruitment and timing controls edit the actual protocol. Changes affect new sequences; historical outcomes and active policy snapshots remain as saved.

Opening case order
Mixed is now the default. Its five standardized cases are community-sound, analyst-job-terms, recording-royalty, colleague-work-favour, land-development.
All-distributive: community-sound, recording-royalty, mobile-coffee-cart, shared-studio-hours, launch-photos.
All-integrative: analyst-job-terms, community-venue-terms, colleague-work-favour, household-renewal, land-development.
The app saves openingCaseIds and arena-standard-five-v1 on each new sequence. Keep those IDs available when editing a bank; the order itself is defined in lib/cases.ts in the private application source. Existing older sequences are retained.
Later rounds draw randomly within the assigned treatment. Mixed return rounds draw task type with equal probability. There are twelve active distributive and ten active integrative cases. Retired cases remain for saved historical records.

Scoring
No deal is zero; explicitly confirmed negative agreements are possible. Fee-case USD range is 800 to 2400, including cents. Let p=(fee-800)/100. Current distributive canonical buyer points=100-8*p and seller points=-28+8*p. Both role legal maxima are 100; the individually rational own maximum is 72 and joint maximum is 72. The mutually acceptable fee interval is 1150 to 2050.
New categorical cases use issueSchema arena-issues-v1, with options containing a/b points for the two canonical roles. Internal buyer/seller maps to those roles; displayed names can be candidate/manager, colleague, mayor/developer or another scenario role. Every complete proposal needs one choice index per issue. Fee/setup/payment placeholders are zero in categorical proposals, and no extra fee or salary can be inserted.
All new categorical cases have legal own maximum 100, mutually acceptable own maximum 72 and joint maximum 72. Exact finite ZOPA diagnostics and issue pairs are retained privately. This calibration does not establish equal empirical difficulty.

Research and privacy
The first five are fixed in order within treatment. Case and round position are therefore linked, including task type in mixed play. Self-selected AI delegation is observational. Preserve case, displayed/internal role, opening side, score/prompt/interaction version and counterpart approach in analysis. Randomized between-participant all-D versus all-I remains a separate admin choice.
These raw files include both roles' payoffs. They are editable public research assets, not a technical guarantee that a motivated participant cannot inspect the other role. AI runtime prompts receive only their own role values and public history. No credentials, participant records or private transcripts belong in this repository.

Hosting
The neutral public app is the existing play Worker on Sam's Cloudflare account. The protected /preview route shares its host/data and requires admin authentication. The separate owner-private Sites deployment is kept synchronized but has a separate database. Worker/D1 plans, current admission caps, real-time activity, API budget and usage are reviewed in the private console. No new capacity or paid-recruitment readiness claim is made by a source update.
