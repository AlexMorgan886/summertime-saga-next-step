# Summertime Saga Next Step Tool

The Summertime Saga Next Step Tool helps players who are unsure what to do next identify the type of guide or resource most likely to help.

Instead of trying to guess the exact next scene, the tool uses the information provided by the player to recommend a relevant resource, such as a character guide, walkthrough, progression reference, or troubleshooting guide.

**Interactive tool:**  
https://summersagahub.com/summertime-saga-stuck-next-step/

## What the Tool Does

The tool is designed for situations where a player has lost track of their progression or is unsure which resource to consult.

It can help narrow down situations such as:

- Being unsure how to continue a character route
- Finishing an event but not knowing where to look next
- Not knowing which guide applies to a particular problem
- Suspecting that a requirement has not been completed
- Being stuck between different parts of the game's progression
- Having a general progression question

The result points the player toward the type of resource most likely to help.

## What the Tool Does Not Do

The tool does not inspect the player's game files or save data.

It does not:

- Read or upload save files
- Access the game installation
- Determine the player's exact story state
- Guarantee the exact next scene
- Modify game files
- Install or download game files

The recommendation is intended to reduce the amount of searching required to find the appropriate documentation.

## How It Works

The basic process is:

```text
Player describes the problem
          ↓
Tool evaluates the selected information
          ↓
Situation is assigned to a resource category
          ↓
Relevant guide or resource is recommended
```

The decision system is based on predefined categories and resource mappings rather than access to a player's private game data.

## Resource Categories

The project currently uses categories such as:

- `character_progress`
- `story_progress`
- `event_requirement`
- `location_problem`
- `general_stuck`
- `technical_problem`

These categories can be expanded as new use cases are identified.

## Example Situations

### Character Progress

> I completed an event with a character but don't know how to continue.

The tool can direct the player toward the relevant character documentation.

### Story Progress

> I finished what I was doing and don't know which part of the story to follow next.

The tool can recommend the appropriate progression or walkthrough resource.

### Technical Problem

> I think I completed the requirement but the event isn't working.

The tool can direct the player toward troubleshooting information.

### General Stuck Situation

> I'm completely stuck and don't know which guide I should use.

The tool provides a starting point based on the information entered.

## Project Structure

```text
.
├── README.md
├── LICENSE
├── CHANGELOG.md
├── CONTRIBUTING.md
├── CODE_OF_CONDUCT.md
├── SECURITY.md
│
├── docs/
│   ├── how-it-works.md
│   ├── decision-rules.md
│   ├── troubleshooting.md
│   └── faq.md
│
├── data/
│   ├── routes.json
│   └── guide-mappings.json
│
└── examples/
    ├── example-inputs.json
    └── example-results.json
```

## Data and Decision Rules

The decision system uses structured data to separate the classification logic from the resource mappings.

This makes it possible to update or expand the tool without rewriting the entire project.

The project documentation explains the categories and mapping structure in more detail.

## Limitations

Game progression can vary depending on the player's previous actions, version, and other circumstances.

For that reason, the tool should be treated as a guide-selection utility rather than an exact progression simulator.

If the recommended resource does not resolve the problem, the player can consult the broader documentation available through SummersagaHub.

## Related Resources

### SummersagaHub

Main website and player-support resources:

https://summersagahub.com/

### Stuck? Find Your Next Step

Interactive version of this project:

https://summersagahub.com/summertime-saga-stuck-next-step/

### Save Compatibility Checker

Check compatibility between supported game versions:

https://summersagahub.com/summertime-saga-save-compatibility-checker/

### Version History

Reference information about game versions:

https://summersagahub.com/summertime-saga-version-history/

### iOS Support Guide

Installation and troubleshooting information for iOS users:

https://summersagahub.com/summertime-saga-ios-support-guide/

## Contributing

Contributions are welcome when they improve the accuracy, clarity, or usefulness of the project.

Useful contributions include:

- Correcting an incorrect resource mapping
- Suggesting a new decision category
- Improving documentation
- Adding representative test cases
- Reporting unclear or misleading results

See [CONTRIBUTING.md](CONTRIBUTING.md) for contribution guidelines.

## Project Status

This repository contains the documentation, decision rules, data structures, and supporting material for the SummersagaHub Next Step Tool.

The project can be expanded as new player situations and documentation resources are identified.

## License

This project's original code and documentation are released under the MIT License.

See [LICENSE](LICENSE) for details.

## About

SummersagaHub is an independent player-support and documentation project.

This repository is not affiliated with or endorsed by the creators of Summertime Saga.
