I think that it could be really cool if you were able to chat with your specs before you started working on any feature or anything. The idea being that you can clearly define the problem before you start agentic coding.

I want this to be something that people can use for anything, not just coding projects.



First draft:

# PRJ 1.0 | Add Item to Cart | HIGH

## Spec
given/when/then
or, whatever you want

## References
Other related specs

## Links
JIRA: CART-123 | GitHub: #456 | Linear: DEV-123
Files: ./src/cart/CartActions.js

## Ambiguity: NONE | Fulfilled: NO | Last Updated: 2025-01-14 | Last Tested: 2025-06-14

Example:

---

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

---

# 2.1.1 | User can drag item to trash | MEDIUM

## Spec
Given: User has event
When: User starts drag
Then: Plus FAB should turn into a red trash can icon
Given: User drags the event to the trash can
When: user lets go
Then: event is deleted
OR
When the user drags an event in the calendar view, the plus button FAB should turn into a red trash can, that they can drag to in order to delete the event.

## References
[2.1](2.1)
[2.2](2.2)

## Links
Linear: DEV-276 | GitHub: #371
**Files:** /Strive/Presentation/Components/FloatingActionButton.swift /Strive/Presentation/Scenes/Calendar/CalendarView.swift /Strive/Presentation/Scenes/Calendar/EventView.swift /Strive/Presentation/Scenes/Calendar/EventsView.swift

## Ambiguity: NONE | Fulfilled: NO | Last Updated: 2025-01-14 | Last Tested: 2025-06-14




---

# Here are some more notes


I think that the best thing would be if the context/specs automatically updated as the user used Claude Code, Cursor etc.

Like maybe some sort of instructions that explain to it how to proactively update the specs files as it goes.


# Thoughts on Kiro

I felt like it was completely overwhelming. It produced so much text for the Requirements, design, and task list that there was no way I was going to actually read and verify all of it.
