# AI Account Health Agent

A custom agent I built for my own book of business, about 60 mid market and enterprise accounts. It does the daily monitoring so my time goes to customers.

## What it does

It reads and condenses data from system dashboards. It scores each account, flags the ones slipping, writes a daily report and organizes the touchpoint schedule so no account goes quiet.

## Signals it reads

**CSAT.** The latest score and the direction over the last three surveys.

**NPS.** The latest score, plus comments that name a problem.

**Product usage.** Logins and active users compared with the account's own 90 day average.

**Usage by function.** Which features each account uses, such as integrations, reporting and campaign tools. A drop in one function often shows a problem before overall usage does.

**Sponsor engagement.** Whether the executive sponsor opened updates, joined calls and replied to requests.

**Daily user engagement.** Whether the people who use the product every day are still active.

**Renewal date.** Days remaining, and how far the renewal plan has progressed.

**Contact dates.** Days since my last touchpoint with the sponsor and with the daily users, compared with the cadence set for that account.

**Open issues.** Support tickets and integration problems still unresolved, and their age.

**Expansion signals.** Requests for new functions, new users or new integrations.

## How it scores

Each signal is rated Green, Yellow or Red, and the combined result sets the account's status. Renewal timing raises the priority, so a Yellow account 45 days from renewal ranks above a Yellow account 200 days out. The weights are defaults that I adjust per account type.

## What comes out

A daily report with accounts that need action today, accounts to watch, healthy accounts and the touchpoints due this week. Each flag states the reason and one recommended action. I make the call, and the agent does the looking.

## Example report

[sample-daily-report.md](sample-daily-report.md) shows the format. Every account in it is fictional and the numbers are made up to show the layout. No client data is stored in this repository.

## Built with

Claude and Claude Code.
