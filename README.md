# Ticket Fairy event marketing skills

Promote events with buyer messaging, discounts, referrals, advertising measurement and social media.

Official [Ticket Fairy](https://www.ticketfairy.com) agent skills, selected from the
[canonical collection](https://github.com/theticketfairy/agent-skills). Install this collection or the individual skills you
need; their names and instructions are the same in both repositories.

## Install

```sh
npx skills add theticketfairy/event-marketing-skills
```

List the available skills without installing:

```sh
npx skills add theticketfairy/event-marketing-skills --list
```

Or select one skill:

```sh
npx skills add theticketfairy/event-marketing-skills --skill email-and-market-to-buyers
```

The current Skills CLI requires Node.js 22.20 or later. Skills install to your
current project by default. Choose the supported agent in the CLI. See the [Skills CLI documentation](https://skills.sh/docs/cli).

## Skills

| Skill | When to use it |
| --- | --- |
| [`email-and-market-to-buyers`](skills/email-and-market-to-buyers/SKILL.md) | Send Ticket Fairy emails and SMS to buyers, design emails, and build event websites and landing pages. Use when an organiser wants to reach their buyers or promote an event. |
| [`run-promotions-and-discounts`](skills/run-promotions-and-discounts/SKILL.md) | Create Ticket Fairy promo codes, group discounts and promoter links. Use when an organiser wants to give some buyers a better price. |
| [`grow-sales-with-referrals`](skills/grow-sales-with-referrals/SKILL.md) | Set up Ticket Fairy referral rewards and see who brought in each sale. Use when an organiser wants buyers to bring their friends. |
| [`track-advertising-campaigns`](skills/track-advertising-campaigns/SKILL.md) | Connect advertising pixels and conversion tracking to Ticket Fairy and see which campaigns sold tickets. Use when an organiser runs paid ads for an event. |
| [`run-event-social-media`](skills/run-event-social-media/SKILL.md) | Connect Instagram and TikTok to Ticket Fairy, draft and schedule posts, answer comments and messages, and run follower presales. Use when an organiser promotes events on social media. |

## Authority and recovery

A skill grants no account permission and does not authorise sending messages,
creating tickets, refunding orders or taking payment. Keep each action within the
person's approved scope and current role. Buyer discovery is public and read-only;
buyer purchases use a separately supported handler and explicit approval of the
final tickets, total and currency, or continue in the official browser checkout.
Organiser credentials do not grant purchase authority. Keep credentials out of chat
and logs. After an uncertain change, recover its original result before
retrying; never issue a new refund, send or ticket grant to resolve uncertainty.

## Documentation and maintenance

- [Official guides](https://www.ticketfairy.com/guides), read live with the public
  [guides MCP server](https://www.ticketfairy.com/docs/mcp).
- [Developer documentation](https://www.ticketfairy.com/developers).
- [Published skill index](https://www.ticketfairy.com/.well-known/agent-skills/index.json).
- [Agent rules](AGENTS.md) and [canonical source](https://github.com/theticketfairy/agent-skills).

`SOURCE.json` records the canonical revision and skill hashes. Make instruction
changes in the canonical repository, then use its
`scripts/build_skill_repositories.py` to copy the reviewed release into this
repository. Do not maintain an independent fork of a skill here.

GitHub publication does not prove skills.sh indexing. Its
[FAQ](https://skills.sh/docs/faq) describes automatic listing through anonymous
Skills CLI installation telemetry. No installation count or indexing status is
claimed by this repository.

## Licence

MIT. See [LICENSE](LICENSE).
