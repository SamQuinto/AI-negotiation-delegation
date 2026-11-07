Negotiation Arena case files

parameters.json contains the payoff rules, fee domain, outside options (BATNAs), timing and creative-catalogue point adjustments. cases.json contains the role text and fixed agenda for each original case.

Edit and apply
1. Open your protected /admin page and choose Case files.
2. Open the current raw JSON, or edit these files in a repository you control.
3. Paste the edited JSON into the editor and select Validate and apply JSON.
4. For a public GitHub file, paste its raw.githubusercontent.com link and select Load and apply. For a private repository, use the authenticated GitHub Raw view and paste the JSON.
5. Change the rules version when you make a substantive change. A content hash is also saved automatically, so changing values without changing the label cannot silently merge leaderboard cohorts.

Changes apply to new participant sequences. Ongoing sequences keep their case library, rules, assignment and difficulty. Additional rounds inherit the original sequence's rules. Historical economic outcomes are read from saved end-of-round metrics.

Default scoring
All amounts are USD. price = (fee - 800) / 100. Any fee from 800 to 2400 is legal, to the nearest cent.
Distributive buyer points: 100 - 8 * price.
Distributive supplier points: 20 + 8 * price.
Both sides have a 30-point outside option. The mutually acceptable fee range is therefore 925 to 1675. Negative agreements are legal: 2400 gives the buyer -28 points. The interface requires explicit confirmation before a participant sends or accepts a below-BATNA deal.

For integrative cases, add each side's setup and payment adjustments to its base-plus-fee score. Form B swaps which issue uses each adjustment vector. The admin console derives a separate ZOPA for each issue package. The agents receive only their own private point sheet.

Defaults and design
The default main study randomly assigns each player to distributive or integrative for five distinct cases. Mixed-within-player is a separate admin schedule, with a randomized 3/2 split. Opening side is randomized independently in main rounds. Practice always prompts the player to open.
Practice preparation is 60 seconds and chat is 210 seconds. Main preparation is 120 seconds and chat is 600 seconds. AI-led modes skip participant preparation. The final decision window is at most 60 seconds after the original chat deadline; refreshing cannot restart it. The default action cap is eight.

Keep supplier point tables in a private repository for studies where participants should not see them. No API keys or participant data belong in this configuration repository. The app's own raw download endpoints require researcher access.

Research interpretation
The full 16-item Subjective Value Inventory retains seven discrete response steps and is presented as two pages of sliders. Practice and additional rounds are excluded from primary first-five analyses. Delegation is self-selected, so outcome associations are observational. AI agents respect their point floor; participants can override their own BATNA with confirmation. Report below-BATNA and manual-override outcomes separately.
Review participant information and the approved protocol if you change timing, data handling, incentives or study design. Paid recruitment is not enabled by these files.

References
Curhan and Vaccaro materials: https://arxiv.org/html/2503.06416v3
Empirica admin concepts: https://docs.empirica.ly/guides/the-admin-panel
