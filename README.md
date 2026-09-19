# ☯️⚖️ Karma and Reputation System

Make the player's actions matter.

Karma & Reputation System is an AI Dungeon script designed to give the player's actions more weight in the story and encourage the AI to treat their decisions as meaningful events with lasting consequences.

It is especially suited for scenarios where choices matter, where the player can shape how others perceive them, and where their actions can gradually lead them toward becoming a hero, a morally ambiguous character, or a villain.

The system is designed to be universal and scenario-agnostic, meaning it does not require a specific setting, character, or storyline.

---

# ✨ Main Features

| Feature | Description |
| --- | --- |
| ☯️ Karma | Tracks significant moral actions performed by the player on a scale from -100 to 100 |
| 🦸 Moral Alignment | Interprets the player's accumulated actions as Villainous, Ruthless, Neutral, Benevolent, or Heroic |
| 🗣️ Reputation | Tracks how the player is generally perceived by others |
| 👥 Public Perception | Influences whether NPCs tend toward fear, distrust, neutrality, respect, or admiration |
| 🚔 Authorities | Represents the general relationship between the player and authorities |
| 📜 Known Deeds | Records significant actions as concrete events rather than relying only on numerical values |
| 🧠 Knowledge Boundaries | Prevents NPCs from magically knowing about actions they could not plausibly know about |
| 🌎 Global NPC Influence | Allows the AI to naturally reflect the player's reputation in NPC behavior |
| 🔒 Player Agency | Never controls the player's thoughts, feelings, dialogue, decisions, or actions |
| 🔄 Universal Design | Works independently of any specific scenario setting or lore |
---

# 🎭 What does it actually do?

The main purpose of this script is not simply to display a Karma number.

It gives the AI additional context about what the player has actually done and encourages it to treat significant actions as established events in the world.

For example, if the player saves someone from an attack, the system may record:

+18 — Rescued someone from danger

The AI can then use that information naturally when appropriate.

Depending on the situation, NPCs might:

- trust the player more
- offer help
- admire them
- become cautious around them
- fear them
- refuse to cooperate
- alert authorities
- discuss their reputation
- seek the player's help

These reactions are not forced. The system provides the AI with the information needed to make them naturally.

The goal is to make the player's previous decisions matter beyond the immediate scene.

---
# ⚖️ Karma vs. Reputation

The system separates several concepts that are often treated as the same thing.

| Concept | Description |
| --- | --- |
| ⚖️ Karma | What the player actually did. |
| 🧭 Moral Alignment | The overall moral interpretation of the player's accumulated actions. |
| 🗣️ Reputation | How the player is generally perceived by society. |
| 👥 Public Perception | The emotional/social response the player's reputation tends to generate. |
| 🚔 Authorities | The general relationship between the player and law enforcement or other authorities. |
| 📜 Known Deeds | Concrete events that NPCs can actually know about and potentially discuss. |

This distinction is important because doing something good does not automatically mean everyone knows about it.

# 🧠 Knowledge & NPC Reactions

The system uses different levels of knowledge to determine what information NPCs can plausibly know.

| Knowledge Level | Description |
| --- | --- |
| 👤 Player History | Everything the player has actually done. |
| 🌎 Public Knowledge | What society could plausibly know about the player. |
| 👥 NPC Knowledge | What a specific NPC could plausibly know. |

NPCs are therefore not supposed to magically know about secret actions.

For example, if the player secretly saves someone in an isolated location with no witnesses, another NPC should not suddenly know exactly what happened.

The system instead encourages the AI to consider plausible sources of information such as:

- 👁️ Witnesses
- 📹 Cameras
- 📰 News reports
- 🚔 Police reports
- 🗣️ Other NPCs
- 💬 Information directly revealed by the player

---

# 📊 Karma Scale

Karma ranges from -100 to +100.

| Karma | Moral Alignment |
| --- | --- |
| -100 to -70 | Villainous |
| -69 to -30 | Ruthless |
| -29 to +29 | Neutral |
| +30 to +69 | Benevolent |
| +70 to +100 | Heroic |

### 🗣️ Reputation

| Reputation | Level |
| --- | --- |
| -100 to -70 | Infamous |
| -69 to -30 | Feared |
| -29 to +29 | Unknown |
| +30 to +69 | Respected |
| +70 to +100 | Admired |

### 👥 Public Perception

| Score | Perception |
| --- | --- |
| -100 to -50 | Fear / Hostility |
| -49 to -1 | Caution / Distrust |
| 0 to 39 | Neutral |
| 40 to 74 | Respect / Trust |
| 75 to 100 | Admiration / Support |

# 📝 Important Design Principles

The system follows a few important rules:

- Karma tracks significant actions, not every individual verb or micro-action.
- Actions that are part of the same event should not be repeatedly counted.
- Defensive actions can be treated as part of a larger rescue or protection event.
- NPC opinions do not directly change Karma.
- Secret actions remain secret unless there is a plausible way for someone to learn about them.
- Reputation does not mean every NPC will constantly talk about it.
- The system does not control the player's character.
- The system does not contain scenario-specific lore.

The intention is to influence how the AI interprets the player's actions, not to turn the story into a rigid statistics-based RPG.

---

# 🔧 Installation

Karma & Reputation System is designed to be installed using AI Dungeon's script installation system.

Install the script through the provided installation method and enable scripting for your scenario.

The system uses AI Dungeon's Input, Context, Output, and Library scripting architecture.

No scenario-specific modifications should be necessary.

You can install it manually coping each part and pasting in AI Dungeon's script editing.

---

# 🔗 Compatibility

🟡 Experimental Compatibility

The script is currently known to work alongside:

- Inner Self by LewdLeah
- Nynaleath's Basic Relationship System

However, compatibility with other scripts has not been extensively tested yet.

In particular, compatibility with:

- Auto-Cards
- other community scripts
- large script combinations

has not been fully tested.

If you discover a conflict or unexpected behavior, please report it through the repository's issue tracker.

⚠️ Script Interaction

Because multiple AI Dungeon scripts can modify the same Input, Context, and Output pipelines, combining several scripts may affect how they interact with each other.

Compatibility should therefore be considered experimental until tested in a specific combination.

---

# 🧩 Universal & Scenario-Agnostic

This script intentionally contains no scenario-specific characters, locations, factions, or lore.

It can therefore be used for:

- superhero scenarios
- fantasy adventures
- crime stories
- slice-of-life scenarios
- RPG scenarios
- political or social dramas
- morally complex narratives
- any scenario where player decisions should have consequences

The system provides the framework; the scenario provides the world.

---

# 📌 Example

A player witnesses someone being attacked and intervenes.

The system may record:

+18 — Rescued someone from danger [witnessed]

Later, the AI can use that established deed when appropriate.

A witness might remember the player as someone who helped.

A stranger who heard about the event might recognize their name.

Authorities might have a different reaction if the same incident involved excessive violence.

A person who never witnessed or heard about the event should not automatically know what happened.

The exact narrative consequences are left to the AI and the scenario.

---

# 🛠️ Current Status

Version: 1.0
Status: Experimental / Active Development

The core system is functional, but compatibility with combinations of community scripts is still being tested.

Feedback, bug reports, compatibility reports, and suggestions are welcome.

---
# 📝 License

Feel free to use in your scenarios, even the published ones.

It's free code, you can modify it and use to create your own scripts.

# ❤️ Credits

Created for AI Dungeon by Nynaleath.

It's not compulsory, but I'll appreciate any credits.

Hope it will be useful for your adventures ^⁠_⁠^
