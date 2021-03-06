<p align="center">
  <img align="center" src="https://i.imgur.com/ijYtOhk.png" width="125" alt="icon">
</p>
<br>
  <h2 align="center">Sketch Accessibility Assistant</h2>
 <p align="center">
  <img src="https://i.imgur.com/OvLMEjK.png" width="500" alt="Accessibility Assistant in action.">
</p>
  <p align="center">
    <a href="mailto:ygis@mit.edu">
      <img src="https://img.shields.io/badge/Sketch-68+-blue.svg?style=flat" alt="Contact">
    </a>
    <a href="https://opensource.org/licenses/MIT">
      <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License: MIT license">
    </a>
  </p>
</h1>

The Accessibility Assistant ensures that your Sketch elements pass AA+ compliance based on the Web Content Accessibility Guidelines. This is a contribution to the Assistants feature launch for Sketch 68. Unlike an accessibility plugin, an assistant automatically detects accessibility infractions and sends out a notification. If you'd like to learn more about Sketch Assistants and how they differ from Sketch plugins, please [read the documentation on Sketch's website.](https://www.sketch.com/docs/assistants/)

## Rules

- [Shapes must meet AA color contrast compliance.](https://github.com/ygev/sketch-accessibility-assistant/tree/main/src/rules/aa-contrast-shape)
- [Text must meet AA color contrast compliance.](https://github.com/ygev/sketch-accessibility-assistant/tree/main/src/rules/aa-contrast-text)
- [Text must meet AAA color contrast compliance.](https://github.com/ygev/sketch-accessibility-assistant/tree/main/src/rules/aaa-contrast-text)
- [Text must not be justified.](https://github.com/ygev/sketch-accessibility-assistant/tree/main/src/rules/text-not-justified)
- [Line spacing must be at least 1.5x times the font size.](https://github.com/ygev/sketch-accessibility-assistant/tree/main/src/rules/text-line-height)
- [Letter spacing must be at least 0.12x times the font size.](https://github.com/ygev/sketch-accessibility-assistant/tree/main/src/rules/text-letter-spacing)

**⚠️ One-click downloads with Sketch are currently down. Please download it directly from GitHub or [npm](https://www.npmjs.com/package/sketch-accessibility-assistant) and Add from Archive.**

~~👉 Click [here](https://add-sketch-assistant.now.sh/api/main?pkg=@ygev/sketch-accessibility-assistant)
to add to your Sketch document.~~

## Known Bugs
- Layers inside groups are not detected yet.
- Layers outside the artboard are not detected yet.
- Very sensitive detection of overlap between layer coordinates. Planning to change it to 80%+ overlap, rather than 1%+ to avoid false negatives.
