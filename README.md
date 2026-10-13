# Travel Companion

An open Codex skill for planning real-world, multi-day trips—from research and booking checks to a practical mobile itinerary, safety notes, photo references, and shared expense settlement.

中文：一个面向真实多日旅行的 Codex skill，覆盖行程研究、预约核对、手机旅行助手、安全提醒、拍照参考和共同记账结算。

## What it helps with

- Research places, transport, restaurants, tickets, opening hours, and practical travel constraints using current sources.
- Turn scattered notes and reservations into a day-by-day plan that is easy to use on a phone.
- Keep confirmed plans distinct from backups; retain the reason when a plan changes.
- Organize photo references by place without cluttering the itinerary.
- Add actionable safety, arrival, accommodation, luggage, and offline-access guidance.
- Design a shared travel ledger with clear currencies, split rules, and settlement results.

## Install in Codex

Clone or download this repository, then copy the `travel-companion` folder into your local skills directory:

```bash
git clone https://github.com/ianc1225/codex-travel-companion.git
mkdir -p ~/.agents/skills
cp -R codex-travel-companion/travel-companion ~/.agents/skills/
```

Restart Codex, then invoke it with:

```text
$travel-companion
```

You can also describe a multi-day trip naturally; Codex can select the skill when it matches the task.

## Example prompts

```text
Use $travel-companion to plan a 10-day Japan Kansai trip for three people. Research the itinerary first, verify reservations and transport, then build a mobile-friendly travel assistant with photo references, safety notes, and a shared expense ledger.
```

```text
使用 $travel-companion 帮我规划三人 10 天关西旅行：先调研和核对预约/交通，再做可手机使用的每日助手，包含拍照参考、安全提示和共享记账。
```

## Privacy and data boundaries

This repository contains only reusable workflow instructions. It intentionally does **not** include real addresses, tickets, reservation codes, passwords, expense data, private photos, or a completed person's trip plan. Keep those materials in the travel project where they belong; do not commit them to a public fork.

## Contributing

Issues and pull requests are welcome—especially improvements that make the workflow more practical across destinations, languages, and group-trip styles. Please do not contribute personal trip data or credentials.

## License

Released under the [MIT License](LICENSE).
