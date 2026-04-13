# DubPlanner Release Notes

---

## Week of April 13-19, 2026

### New Features

#### Ticket Detail Side Panel
- **Click any ticket to open its details** - Clicking a ticket in the planner now opens a side panel on the right with the full ticket details — status, assignee, estimate, week, milestone, parent, and description — plus a link out to the issue tracker
- **Edit status, assignee, and week inline** - Change a ticket's status, assignee, or scheduled week directly from the panel, with a Save/Cancel flow and a prompt before losing unsaved changes
- **Resizable panel** - Drag the panel's left edge to make it wider or narrower; your preferred width is remembered across sessions

#### Rich Markdown in Ticket Descriptions
- **Full Markdown rendering** - Ticket descriptions now render links, bulleted and numbered lists, task-list checkboxes, tables, blockquotes, fenced code blocks, strikethrough, and auto-linked URLs — both in the hover tooltip and in the new ticket detail panel

### Improvements

#### Cleaner collapsed sidebar
- **Hide team icons when the sidebar is collapsed** - The collapsed sidebar now shows only the logo and user avatar, removing the unlabelled team icons that made it hard to tell what was what

---

## Week of March 23-29, 2026

### New Features

#### Sign Up Page
- **Dedicated Sign Up experience** - First-time users now have a dedicated Sign Up page, separate from the Login page, with consistent branding across both

### Improvements

#### Stay signed in to Linear longer
- **Linear OAuth refresh token support** - DubPlanner now refreshes your Linear session automatically so you do not have to sign in as often

#### Sidebar polish
- **Long names no longer introduce scrollbars** - Team and project names in the sidebar are truncated cleanly instead of forcing horizontal scroll

---

## Week of March 2-8, 2026

### New Features

#### Onboarding Wizard for Linear
- **Guided label setup on first login** - New Linear users are walked through setting up the Week labels DubPlanner needs, so the planner works from day one
- **Works even in restricted workspaces** - DubPlanner can now create Week labels in Linear workspaces where label creation is normally restricted, via a temporary permission prompt
- **Reconfigure Labels anytime** - Organization Settings has a new Reconfigure Labels button to re-run the setup wizard whenever you need to

#### Pricing Plans and Billing
- **Tiered pricing plans** - DubPlanner now has a tiered plan model with a free trial, paid plans, and per-seat billing powered by Stripe
- **Automatic Stripe seat sync** - Disabling, enabling, or deleting a member automatically adjusts your Stripe subscription seat count so billing stays accurate

#### User Management
- **Disable and delete members** - Organization Settings now includes a full user management screen for disabling and deleting team members
- **Created and Last Seen dates** - The Members screen now shows each member's Created date and Last Seen date

### Improvements

#### Organization Settings available for everyone
- **Organization Settings is live by default** - The Organization Settings menu is now available for all workspaces, not just those with the feature flag enabled

### Bug Fixes

- **Switching projects between teams now works reliably** - Switching to a project on a different team no longer shows a blank screen
- **Role changes apply immediately** - Changing a member's role in Organization Settings now updates the UI without requiring a page refresh
- **Label wizard no longer tries to recreate existing labels** - The onboarding wizard correctly detects existing Week labels and leaves them alone
- **Label wizard sees all 52 week labels** - Pagination is now handled correctly so the wizard finds every existing Week label
- **Label wizard handles archived and team-scoped labels** - Archived or team-scoped Week labels are now handled correctly during setup
- **"Looks Good" button closes the label wizard** - Confirming existing labels now exits the wizard as expected instead of leaving it open

---

## Week of February 23 - March 1, 2026

### Bug Fixes

- **Presence indicator tooltips no longer appear behind other UI** - Fixed a layering issue where presence indicator tooltips could be hidden behind other elements on the page

---

## Week of February 16-22, 2026

### New Features

#### Show Completed Toggle
- **Hide or show completed tickets** - New toggle in display options lets you filter out completed, done, and finished tickets from the planner grid. Your preference is remembered across sessions

#### Resizable Sidebar
- **Drag to resize the sidebar** - You can now drag the right edge of the sidebar to make it wider or narrower, so long team and project names are no longer cut off. Your preferred width is saved across page reloads

#### Remember Last Project
- **Pick up where you left off** - Opening DubPlanner now takes you straight to the last project you were working on, instead of showing an empty project selection screen

### Improvements

#### Visual Polish
- **Completed tickets are visually de-emphasised** - Tickets with a completed or done status now appear at reduced opacity, making it easier to focus on active work
- **Tooltips on controls** - Header and sidebar buttons now show helpful labels on hover, including toggle sidebar, open in issue tracker, favourite, and display options
- **Wider dropdown menus** - Display options and filter menus are now slightly wider to avoid text being cut off
- **Cleaner milestone tooltips** - Milestone tooltip popups no longer show an unwanted border frame

### Bug Fixes

- **Fixed noisy connection indicator** - The "Connected" status badge is now hidden during normal use to reduce visual clutter. It still appears when there's a connection problem

---

## Week of February 9-15, 2026

### New Features

#### Display Density Slider
- **Single density control** - Replaced the separate cell width and height dropdowns with one easy-to-use slider offering five sizes: Chip, Compact, Normal, Card, and Large Card

#### Expand Rows Toggle
- **Show all tickets at once** - New toggle in display settings expands grid rows to show every ticket in a cell, removing the need to scroll through per-cell arrows

#### Show Archived Tickets
- **View completed work** - New toggle in settings lets you include archived and completed tickets on the planner grid

#### Create Issue from Grid
- **Quick issue creation** - Right-click any cell or press `C` to create a new issue directly from the grid, automatically pre-filled with the cell's assignee and week

#### Rich Ticket Descriptions
- **Formatted description tooltips** - Ticket description tooltips now render Markdown formatting including bold, italic, code blocks, and headings

### Bug Fixes

- **Fixed invisible Delete button in dark mode** - The Delete button now displays correctly in dark mode with proper theme colors
- **Fixed missing error messages** - API error messages now properly appear in toast notifications instead of failing silently
- **Fixed duplicate week label errors** - Moving tickets between weeks no longer causes duplicate week label errors

---

## Week of February 2-8, 2026

### New Features

#### Project Change Notifications
- **Stay in sync with your team** - A banner alert now appears when a project is updated or deleted by another user, with options to refresh or dismiss

### Improvements

#### Session Handling
- **Smoother re-authentication** - Expired issue tracker sessions now prompt you to re-login instead of showing confusing server errors

### Bug Fixes

- **Fixed authentication lookup for some workspaces** - Resolved an issue where issue tracker authentication could fail for certain workspace configurations

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
