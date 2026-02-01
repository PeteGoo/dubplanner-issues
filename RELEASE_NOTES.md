# DubPlanner Release Notes

---

## Week of January 26 - February 1, 2026

### New Features

#### Real-Time Ticket Updates
- **Instant sync from your issue tracker** - When tickets are updated in your issue tracker (status changes, assignee changes, week label changes), the planner now updates automatically in real time — no need to refresh
- **Multi-user collaboration** - Changes made by teammates appear instantly across all connected browsers

#### Crash Analytics
- **Improved error detection** - Behind-the-scenes error tracking helps us identify and fix issues faster, improving overall reliability

### Improvements

#### Reliability
- **Smarter conflict resolution** - When multiple users edit the planner simultaneously, updates are now resolved using version tracking instead of timestamps, preventing lost changes
- **Faster visual feedback** - Planner updates now appear instantly when changes are made, with background syncing handled seamlessly
- **Enhanced data privacy** - Sensitive ticket content is no longer stored in real-time sync data

### Bug Fixes

- **Fixed ticket status bounce-back** - Resolved an issue where ticket status changes would briefly revert to their old state before showing the correct update
- **Fixed tooltip flickering** - Tooltips on issue cards no longer flicker when hovering over them
- **Fixed dropped updates with multiple windows** - Simultaneous edits from two browser windows no longer cause updates to be lost

---

## Week of January 19-26, 2026

### New Features

#### Estimate Display
- **View ticket estimates in the planner** - Estimates now appear on ticket cards in both the planner grid and backlog views
- **T-shirt size support** - Teams using T-shirt sizing (XS, S, M, L, XL) see human-readable labels instead of numeric values
- **Cell and week totals** - See aggregate estimates per user/week and in week headers (for numeric estimation teams)
- **Toggle visibility** - New "Show Estimates" option in the display settings dropdown lets you show or hide estimates

#### Project Favourites
- **Star your favorite projects** - Add frequently-used projects to your favourites for quick access
- **Instant visibility** - Favourited projects now appear immediately in the sidebar without waiting for the team to load
- **Persistent storage** - Your favourites are saved and sync across sessions

#### Support Request Form
- New support request form when your workspace isn't yet enabled, making it easy to request access

### Improvements

#### User Interface
- **Teams sorted alphabetically** - Teams in the sidebar are now sorted A-Z for easier navigation
- **Consistent folder icon colors** - Project folder icons now have consistent colors based on the project, making them easier to identify at a glance
- **Removed unused Vacation Mode toggle** - Cleaned up the header menu by removing the non-functional toggle

### Bug Fixes

- **Fixed in-progress tickets not appearing** - Tickets that were in-progress but didn't have a week label assigned now correctly appear in the planner
- **Fixed availability calculation error** - Resolved an issue where null date parameters could cause errors in project availability calculations
- **Fixed favourite projects not loading** - Favourite projects now properly appear even before the full team data loads

---
