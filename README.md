# Societee Pool Helper — via Switch

Track 01: Best Business Workflow
Team: Bob The Builder (Ayush Kumar, Ankit Kaushik Sharma, Suryansh Rai)
Flip the Switch Hackathon, WeMakeDevs x DevTools Academy x Switch AI

## Problem
Residents of one housing society want to book home services together
to get a bulk discount, but counting homes, tiers and prices by hand
in a group chat is slow and error-prone.

## Workflow
In a Telegram group called SOCIETEE, connected to Switch as a room,
residents tag an AI agent. The agent keeps the pool count in the
Switch room document and replies with the count, tier and price.

Commands:
- @codex join AC service pool, Flat 402
- @codex pool status

## How Switch is used
Switch is central — without it, the agents would not be in the
Telegram group at all, and there would be no shared room, rules or
room document. If you remove Switch, this workflow stops working.

Agents connected: Antigravity and Codex, via Switch Console on macOS.
Channel: Telegram group SOCIETEE, linked to a Switch room.
Room document: ac_service_pool

Services and tiers:
- AC service ₹1,499, car cleaning ₹499
- 5+ homes 10% off, 10+ 15%, 20+ 25%

Proven result:
- AC service: 5 homes, 10% off, ₹1,349.10 per home,
  5 homes left to the 15% tier at 10 homes
- Car cleaning: 0 homes, no discount yet, ₹499 per home,
  5 homes left to the 10% tier

## How to run it
1. Install Switch Console and Docker, start the local Switch server.
2. Add an agent (Codex / Antigravity) in Switch Console.
3. Connect Telegram in Switch Connectors, create a Telegram group,
   make the bot admin, link your Telegram account.
4. Invite the agent with /invite-agent @codex
5. Send the pool rules in pool-rules.md to @codex in the group.
6. Test with @codex pool status

## Demo video
https://youtu.be/uwiSCAkeXDM
