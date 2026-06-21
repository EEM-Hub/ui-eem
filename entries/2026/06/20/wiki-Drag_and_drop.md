---
source: sources/wiki-Drag_and_drop.md
source_url: https://en.wikipedia.org/wiki/Drag_and_drop
---

## Drag and Drop in Graphical User Interfaces

Drag and drop is a pointing device gesture in graphical user interfaces where a user selects a virtual object by "grabbing" it and moving it to a different location or onto another virtual object. It can invoke actions or create associations between abstract objects. While fast and easy to learn, its discoverability is a usability concern — users may not realize an item is draggable or what the resulting action will be.

## Key Concepts

- **Basic sequence**: Move pointer to object → press and hold button to "grab" → drag to desired location → release button to "drop"
- **Fitts' Law tradeoff**: Dragging requires more physical effort than free pointer movement, reducing speed and precision, but it "chunks" two operands (object + destination) into a single action
- **Selection vs. drag conflict**: When the same button selects and drags, imprecise movement can cause unintended drags
- **Hidden target problem**: Drop targets may be obscured by other windows; Mac OS X addressed this with Exposé
- **Touch screen variant**: Uses long press then drag; iOS 11 introduced cross-app drag and drop on iPad (same-app only on iPhone)
- **End-user programming**: Drag-and-drop block programming (pioneered by AgentSheets) provides four affordances: composable blocks, editable blocks, nestable blocks for tree structures, geometric arrangement for syntax definition

## Commands and Syntax

- **HTML5 Drag and Drop API**: The HTML5 spec includes native drag-and-drop support for three categories:
  - Drag and drop text/HTML codes
  - Drag and drop HTML elements (sends element ID to destination parent)
  - Drag and drop files
- **OS/2 Workplace Shell**: Uses secondary (right) mouse button for drag-and-drop, reserving primary button for selection/clicking
- **Mac OS history**: System 7 added document-to-app icon dropping; System 7.5 extended to clipboard operations (copy/move text), clipping files, and cross-application drops

## Relationships

- **Pointing device gestures**: Drag and drop is one type alongside mouse gestures, point-and-click, and snapping
- **Visual programming languages**: Drag-and-drop is a foundational interaction pattern for block-based programming (AgentSheets, Scratch-style environments, Unreal Engine Blueprints, GameMaker, Construct 2)
- **Website builders**: Powers no-code platforms (Wix, Squarespace, GoDaddy, Weebly) — over 21 million websites built with drag-and-drop builders as of May 2025
- **Common User Access (CUA)**: OS/2's drag-and-drop usage was part of the CUA standard, distinguishing native apps from cross-platform ports
- **Shader editors**: Used in node-based material/shader editing in tools like Blender

## Exam-Relevant Points

- Drag and drop "chunks" two operands into one action (Buxton, 1986) — key HCI principle
- HTML5 drag-and-drop: when dragging an HTML element to move it, the element's **ID** is sent to the destination parent
- iOS 11 drag-and-drop distinction: **cross-app on iPad**, **same-app only on iPhone**
- Original Macintosh (128K) used "click and drag" for file manipulation; System 7 added document-to-app dropping; System 7.5 extended to text/clipboard operations
- OS/2 Workplace Shell used the **secondary mouse button** for drag-and-drop (unlike Mac/Windows which use primary)
- Wix holds ~33% market share of drag-and-drop website builders (~7M sites), followed by Squarespace (~25%), GoDaddy (~19%)
- AgentSheets introduced the modern concept of drag-and-drop block programming with four core affordances (composable, editable, nestable, geometrically arranged)
