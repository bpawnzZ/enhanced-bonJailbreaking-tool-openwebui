# Enhanced bonJailbreaking Tool for Open-WebUI

This tool implements an advanced Best-of-N (BoN) Jailbreaking method to help bypass restrictions in LLM chatbots within Open-WebUI. It uses sophisticated prompt augmentation techniques to modify user inputs in ways that are more likely to elicit responses from restricted models.

## Key Features

- **Advanced Prompt Augmentation**: Applies multiple transformation strategies to prompts including:
  - Roleplay scenarios (educational, business, creative, etc.)
  - Perspective shifts (academic, technical, philosophical, etc.)
  - Structural changes (shuffling, reversing, repeating)
  - Contextual framing (hypothetical, fictional, narrative)

- **Best-of-N Sampling**: Tries multiple variations of a prompt to find one that successfully bypasses restrictions

- **Fallback Strategies**: Implements secondary augmentation techniques when initial attempts fail:
  - Rephrasing
  - Simplification
  - Context expansion
  - Metaphorical framing
  - Question-based reformulation

- **Success Tracking**: Maintains a record of successful augmentations for analysis and improvement

## How It Works

1. The tool takes a user's original prompt
2. Applies random augmentations from a set of available strategies
3. Checks if the augmented prompt is likely to bypass restrictions
4. If successful, returns the augmented prompt
5. If unsuccessful, tries fallback strategies
6. Tracks successful augmentations for future reference

## Usage

The tool is designed to be integrated into Open-WebUI's chat interface. When a user's prompt is detected as potentially restricted, the tool automatically attempts to generate a bypass version.

## Configuration

The tool's behavior can be customized through various parameters:
- Maximum number of samples to try
- Available augmentation types
- Roleplay scenarios
- Bypass detection keywords
- Fallback strategies

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

Based on original work by JPLHughes:
- [BoN Jailbreaking Article](https://jplhughes.github.io/bon-jailbreaking/)
- [Original Repository](https://github.com/jplhughes/bon-jailbreaking)
