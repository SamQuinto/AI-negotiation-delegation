Negotiation Arena editable configuration
Updated 8 November 2026, application v28

Public app: https://play.the-negotiation-arena.workers.dev/
Fresh participant preview: https://play.the-negotiation-arena.workers.dev/try
Protected administration: https://play.the-negotiation-arena.workers.dev/admin

Use these files
parameters.json: point equations, legal fees, outside options, timing and creative extras.
cases.json: original case stories, roles and fixed agenda.
ai-prompts.json: shared rules and separately named AI specialists, including dashboard review.
study-protocol.json: paid-visit timing, bonus rule, scope policy and follow-up wave fields.
update-log.json: documented app changes. Actual deployments have separate receipts.
AI_and_study_guide.txt: architecture, choice policy, measures and operating instructions.

Apply a change
Open Admin > Case files. Select parameters, cases or prompts, paste JSON and choose
Validate and apply JSON. Alternatively use the matching public raw GitHub link.
Study timing and bonuses are edited under Recruitment and timing.
Change a version label for substantive revisions. The app also hashes settings.
New sequences use revised settings; saved sequences retain their snapshots.
Additional negotiations inherit the original sequence's frozen task settings.

Default scoring
All amounts are USD. price = (fee - 800) / 100. Fees from 800 to 2400 are legal,
including cents. Distributive buyer points = 70 - 8 * price. Seller points =
-10 + 8 * price. No deal gives each side zero. The mutually acceptable price
interval is 925 to 1675. A buyer who agrees to 2400 receives -58 points.
Participants can explicitly confirm below-zero offers or agreements.
In integrative cases add the role's setup and payment adjustments. Form B swaps
the setup/payment adjustment mapping. The server calculates the resulting value.
Legacy keys human/opponent in parameters denote canonical BUYER/SELLER utilities;
the engine maps them to the actual participant role. Do not swap those JSON keys
when a participant happens to be the seller.

Study and tutorial
The default main study assigns each participant to distributive or integrative,
then draws five distinct cases of that type. A separate mixed schedule is available
in admin. Buyer/seller order is two of each plus a random fifth, shuffled. Opening
side is separately randomized. The common integrative tutorial has the participant
open and teaches typed offers, persuasive chat, the offer form and private AI help.
Completed profiles skip it on return. Fresh /try links deliberately start anew.
Practice: up to two minutes preparation, nine minutes chat and one final minute.
Paid main rounds: up to two minutes preparation, four minutes chat and one final
minute. General play uses the configured ten-minute main chat. There is no global
move-count cap within the clock. Refresh does not restart a deadline.

AI choice
Free-choice rounds have no selected role, coaching scope or execution permission.
A blue Last time marker is context only. Every round requires a new selection.
Changing role, scope or either permission asks one short reason question; unchanged
reselection does not. Reasons stay out of every AI context and enter the export.
Preparation, live coach and negotiator are process roles. Official offer and final
agreement permissions are separate. AI-led play skips preparation and pauses for
renewed authorization after at most two AI actions. Private steering is retained.

Research and data
Human SVI retains sixteen original human items and item-specific seven-position
anchors, two pages, no preset responses, N/A and reverse coding. It is scheduled
after rounds 1, 3 and 5. Every round asks willingness to continue and a short next
strategy. Own score is visible before SVI; this round's rank feedback follows SVI.
Primary outcomes use the common first five. Optional rounds, returns and paid
follow-up waves are separate. Self-selected delegation is observational.
Communication plots are experimental wording indicators, not validated traits or
ability. Detailed reviews use verified own-role facts and message evidence, save
to the profile and require five new completed negotiations after each review.

Privacy and release
This configuration repository is public replication material, including scoring
rules. It is not a confidential store. Do not add API keys, passwords, personal
records, real recruitment/completion codes or private participant transcripts.
The app's raw configuration and participant-data endpoints require researcher
access. Paid recruitment remains off until approved study details and actual
recruitment/completion routes are configured. No payments are sent by the app.

Raw files
https://raw.githubusercontent.com/SamQuinto/AI-negotiation-delegation/main/parameters.json
https://raw.githubusercontent.com/SamQuinto/AI-negotiation-delegation/main/cases.json
https://raw.githubusercontent.com/SamQuinto/AI-negotiation-delegation/main/ai-prompts.json
https://raw.githubusercontent.com/SamQuinto/AI-negotiation-delegation/main/study-protocol.json

Sources used as methodological references
https://doi.org/10.1073/pnas.2521774123
https://arxiv.org/html/2503.06416v3
https://docs.empirica.ly/guides/the-admin-panel
