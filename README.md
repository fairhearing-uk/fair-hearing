# Fair Hearing

**For owners and managers without an HR department** who need to deal with an employee's conduct fairly and by the book. Fair Hearing guides the person making the decision through a conduct disciplinary (misconduct or gross misconduct) in England, Scotland or Wales, following the Acas Code of Practice on disciplinary and grievance procedures, and drafts the letters for them to check and sign.

**This is process guidance, not legal advice. You make every decision.**

## Install

To install in Claude Code, run these two commands in your terminal:

```
claude plugin marketplace add fairhearing-uk/fair-hearing
claude plugin install fair-hearing@fairhearing-uk
```

## How to start

Describe what happened in your own words. In Claude Code, typing `/fair-hearing:triage` is the surest way to start.

## What it does

- **Starts your case.** Says what it assumes (the employee works in England, Scotland or Wales, is an employee, and you're the one deciding), so you only need to correct it if that's wrong. Then asks what happened and a few short questions, including whether you want to go informal or formal. Ends with a summary of what you told it.
- **Checks for red flags at every step.** If the case involves something such as pregnancy, health or disability, whistleblowing, trade union activity, an open grievance, possible discrimination, a criminal matter, Northern Ireland, someone who isn't an employee, or borderline length of service, it stops and tells you to take legal advice.
- **Walks you through each stage:** investigation, the invitation and the right to be accompanied, the hearing, the outcome and the appeal, or the informal route. Each stage gets a short plain-English checklist. You can ask to see the exact Acas Code wording at any point.
- **Drafts six letters:** hearing invitations (where a warning is possible, or where dismissal is possible), outcome letters, an appeal invitation and an appeal outcome letter. They are adapted from Acas's templates and given as plain text for you to copy into your own document.
- Up to date with the unfair dismissal changes that apply from 1 January 2027.

## What it won't do

- Decide for you, recommend a sanction, or say whether the evidence proves anything.
- Give legal advice, say whether a dismissal is fair, or estimate what a claim might be worth.
- Work out dates, notice or length of service.
- Draft outcome letters before the hearing, invent facts or evidence, or draft letters outside the six (for example suspension, investigation or settlement letters).
- Help with grievances, performance or capability, redundancy, or Northern Ireland.
- Help employees, or anyone acting for an employee. It is for the employer's side only.

## Known behaviours in 1.0.5

Fair Hearing is instructions for an AI model, and the model does not follow them perfectly every time. In testing we saw these:

- **It may stop you if you ask only about a grievance.** Fair Hearing covers conduct disciplinaries. If you ask it how to handle a grievance, it may tell you to take legal advice and go no further.
- **It may stop a case involving a long-serving employee whose employment could end on or after 1 January 2027.** It does this to be cautious about the change in the law on that date, even where the employee's service is well past the qualifying period.
- **If you ask it to start a disciplinary alongside an offer to pay someone to leave, it should stop and tell you to take legal advice.** On Claude's smaller, faster model (Haiku) it sometimes refuses in its own words without giving the stop message.
- **An employee who is about to reach two years' service should always be stopped for legal advice.** On Haiku, about 1 time in 50 in our tests, it carried on with its questions. If an employee is close to two years' service, or close to six months for employment ending on or after 1 January 2027, take legal advice whatever Fair Hearing says.
- **Very occasionally one word of the stop message is wrong** (for example "employee law solicitor" for "employment law solicitor"). The stop still applies.

## Letters say AI helped

Every letter is headed DRAFT and ends: "Prepared with the help of an AI drafting tool and reviewed by [manager name]." That last line tells the employee AI was used. Remove "DRAFT" yourself once you've checked the letter, and keep the last line.

## What it runs, sends or stores

Nothing. Fair Hearing is instructions and reference text only. It runs no scripts, connects to no server, and sends or stores nothing. What you type stays in your own Claude conversation, under your own account settings.

## Support

fairhearinguk@proton.me

See [SUPPORT.md](SUPPORT.md), [PRIVACY.md](PRIVACY.md) and [TERMS.md](TERMS.md).

## Licence and attribution

Fair Hearing's original content is licensed under [CC BY 4.0](LICENSE). Content from Acas and from legislation is used under the Open Government Licence v3.0 and credited in [ATTRIBUTION.md](ATTRIBUTION.md). Fair Hearing is not produced, reviewed or endorsed by Acas.
