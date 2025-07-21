Hi

# Interface Specifications Language (ISL)

ISL is in and of itself simply a format for writing specifications for a project. There us a little bit of structure, but it differs from things like qucumber because it won't be parsed by a computer, just by AI.

### Other projects
kiro.dev came out the day after I first had this idea, and I tried it out.
Kiro.dev made three files, requirements.md, design.md, and tasks.md, with over 500 lines in total. This is WAY too much in my opinion. If I want to start a task, I want a *much* shorter plan. I want it to fit on my screen.

## Spec Structure

Here is an example of a project overview:

```
# Project Overview:

## 1 Code & Architecture

## 2 User Experience

### 2.1 Users should have a seamless experience

### 2.2 Each interaction should be simple

### 2.3 Calendar View

## 3 Testing & Quality

## 4 Deployment & Infrastructure

## 5 Security & Compliance

## 6 Monitoring & Analytics
```

Here is an example of an actual spec.
```
# 2.1.1 | Title: User can drag item to trash | Priority: MEDIUM

## Spec
Given: User has event
When: User starts drag
Then: Plus FAB should turn into a red trash can icon
Given: User drags the event to the trash can
When: user lets go
Then: event is deleted
OR
When the user drags an event in the calendar view, the plus button FAB should turn into a red trash can, that they can drag to in order to delete the event.
(sidenote: You can use a structure like given/when/then, or just freeform text. You can use whatever format you want for the spec because, in the end, the AI just needs to understand what you're saying.)

## References
[2.1](2.1)
[2.2](2.2)

## Links
Linear: DEV-276 | GitHub: #371
**Files:** /Strive/Presentation/Components/FloatingActionButton.swift /Strive/Presentation/Scenes/Calendar/CalendarView.swift /Strive/Presentation/Scenes/Calendar/EventView.swift /Strive/Presentation/Scenes/Calendar/EventsView.swift

## Ambiguity: NONE | Fulfilled: NO | Last Updated: 2025-01-14 | Last Tested: 2025-06-14
```

The current plan is that all spec files will be written in Markdown.

In this repository, you will also find tools that help you to quickly create and intetact with the specifications for a project.

For the first stage of the project, we'll be creating a TUI similar to Claude Code where you can "chat" with the specs.

Features of the TUI will include the following:
- The ability to generate specs from a project's code and or Claude Code conversations
- The ability to generate a "mind map" of your project to assist the AI in quickly navigating your code base
- The ability to generate prompts based on specs
- The ability to "chat" with your specs and quickly add or update specs.

## License
This project is licensed under the Apache 2.0 License - see the [LICENSE](LICENSE) file for details.
