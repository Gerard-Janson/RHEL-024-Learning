# Command line assistant

Status: done_

## Goal

Understand RHEL 10's built-in Command Line Assistant (Lightspeed) and what's needed to use it, and try registering a system.

## Concepts involved

- Command Line Assistant — RHEL 10's built-in AI, backed by RHEL Lightspeed, answers questions in-terminal
- Registration required — needed for updates and to use Lightspeed
- Two ways to register — directly with Red Hat via `subscription-manager`, or via a company-run Satellite server

## Commands

```bash
# c — ask the Command Line Assistant a question directly in the terminal
$ c "Why should I register RHEL?"
```

```bash
# subscription-manager register — registers this system with Red Hat's CDN
# --username lets you skip the interactive username prompt
$ subscription-manager register --username <your-username>
```


```bash
# subscription-manager status — shows whether the system is currently registered/subscribed
$ subscription-manager status
```


```bash
# subscription-manager list --available — lists subscriptions available to attach
$ subscription-manager list --available
```

```bash
# subscription-manager list --consumed — shows subscriptions currently attached
$ subscription-manager list --consumed
```

```bash
# subscription-manager unregister — removes registration from this system
$ subscription-manager unregister
```

```bash
# insights-client --register — registers with Red Hat Insights (separate from Lightspeed;
# covers health checks, vulnerability scanning)
$ insights-client --register

```

## Notes
Only Red Hat has comand line assistant.In other distros you have to use shell-genie or ollama
