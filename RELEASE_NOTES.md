# DubPlanner Release Notes

---

## Week of August 10-16, 2026

### New Features

#### Custom Views — plan across several projects at once
- **Build a view from any projects you choose** - Create a named view from the new "Views" group in the sidebar, pick projects from any team, and the planner opens with all of their work on one board.
- **Or follow a Linear initiative** - Point a view at an initiative and it tracks that initiative's projects (including sub-initiatives) automatically, so projects added later show up without you editing the view. These views are named after the initiative they follow.
- **Weeks line up across projects** - Projects that started at different times are aligned to real calendar weeks, so a column means the same point in time for everyone on the board.
- **Everything you can do in a project, you can do in a view** - Drag tickets between weeks and people, change status, assignee and milestone, create new issues (you're asked which project, and it remembers your last choice per view), and group the Backlog by project.
- **See where each ticket comes from** - Every card carries a colour dot matching its project in the sidebar, and the header shows how many projects are in the view with a list that links to each project's own planner.
- **Plan together in a view** - Teammates' live updates and presence avatars work across every project in a view, and are visible to anyone working in those projects directly.
- **Clear about what it can't do** - Dropping a ticket into a week before its own project starts is refused with an explanation instead of quietly moving it somewhere else, and if a project can't be loaded the view names it in a banner rather than silently showing less work.

#### Book time off straight from the planner grid
- **Availability from a cell's right-click menu** - Right-click a person's week in the grid and use the new Availability submenu to add a vacation, add an absence scoped to just this project, or remove an entry that overlaps that week.
- **Confirm before it's booked** - Choosing "Add Vacation" opens Manage Availability prefilled with that week's Monday–Friday, so a mis-clicked cell is a dialog you can adjust or cancel rather than a booking you have to undo.
- **Edit from the grid too** - "Edit Availability…" opens the same dialog on that person's entries, and the dialog's tabs now show how many entries each one holds.

#### Search the sidebar
- **Jump to any project or view by name** - A search box at the top of the sidebar finds projects across every team and your saved views in one ranked list — no expanding teams to hunt for a project.
- **Search by team name as well** - Typing a team's name surfaces its projects, which helps when the same project name appears in more than one team.
- **Keyboard-friendly** - Type, arrow up and down through the results, and press Enter to go there. If one team can't be reached, the rest of the results still appear alongside a notice.

### Improvements

#### Finding projects
- **Better ranking in the Custom View project picker** - The picker now sorts prefix matches to the top and lets you find a project by its team name, matching how sidebar search behaves.

#### Views
- **Confirmation before deleting a view** - Deleting a view now asks first, and spells out that only the view is removed — your projects, tickets and milestones are untouched.
- **Opens on the current week** - Views now scroll to the current week when you open them, the same as a single project does.

### Bug Fixes

- **Manage Availability could fail to open** - The availability dialog could return a server error the first time it was opened; the missing database configuration behind it is now in place.
- **Filtered-out tickets no longer vanish** - Changing a ticket's status or assignee while a filter was active (such as hiding completed work) could silently drop the hidden tickets from the board until you reloaded.
- **Removing someone's last availability entry now updates the grid** - Deleting a person's only vacation or absence left the shading on their row until a refresh.

---

## Week of June 8-14, 2026

### New Features

#### Collapse backlog groups
- **Tidy up long backlogs** - When the Backlog is grouped (by milestone or status), each group now has a chevron to collapse or expand it, so you can fold away the groups you're not working on. The item count stays visible on collapsed groups.

#### Control how ticket hover details appear
- **Turn hover details on or off** - A new "Hover Details" toggle in the Display menu lets you disable the detailed popup that appears when hovering a ticket — handy now that the detail panel shows the same information. Your choice is remembered between visits.
- **A calmer hover** - The hover popup now waits about a second before appearing instead of flashing up the instant your cursor passes over a ticket.

### Improvements

#### Backlog grouping
- **Your grouping is remembered** - The Backlog "Group by" choice now persists between visits, so the list stays organized the way you left it.

#### Milestone navigation
- **Open a milestone from the backlog** - When the backlog is grouped by milestone, click a milestone's group header to open its detail panel, and the backlog automatically scrolls to keep the focused milestone in view as you step between them.

#### Milestone details
- **Formatted descriptions** - Milestone descriptions in the detail panel now render Markdown, so lists, links, and other formatting display properly.

### Bug Fixes

- **Hover popups no longer pile up** - Moving the cursor across several tickets used to queue a burst of delayed popups that all appeared at once; the pending popup is now cancelled as soon as you move on.
- **The side panel no longer squeezes the Backlog** - Opening a ticket or milestone's detail panel used to shrink the Backlog and distort its layout; the panel now overlays the view instead, and closing it (Esc or the close button) brings the full Backlog back.

---

## Week of June 1-7, 2026

### New Features

#### What-If Mode — experiment with your plan without touching Linear
- **Try out alternate plans safely** - Create named "What-If" scenarios where you can rearrange the plan — move tickets across weeks and people, change milestones, send work to the backlog, or unassign it — and none of it is saved to Linear until you choose to apply.
- **Add placeholder tickets** - Sketch in not-yet-created work as placeholders (double-click a cell, right-click → Create Issue, or press C); they only become real tickets when you apply the scenario.
- **Review and apply in one step** - A review panel summarizes every change, showing each ticket's move, reassignment, and milestone change as a clear "from → to", then applies them all to Linear at once.
- **See your changes at a glance** - An amber banner marks What-If mode and any ticket your scenario changes is outlined, so it's obvious what's different from the live plan.
- **Collaborate live** - Teammates viewing the same scenario see updates in real time.

#### Milestone focus and navigation
- **Focus a single milestone** - Click a milestone to open it in a side panel and dim everything else, so you can concentrate on one milestone's work.
- **Step through milestones** - Back/forward arrows in the milestone panel cycle through your milestones, plus a "No Milestone" view that highlights tickets not yet assigned to any milestone.
- **Set milestones faster** - Choose a milestone when creating an issue, and change a ticket's milestone straight from its right-click menu (the current one is checked).

#### Group the backlog
- **Group By selector** - Organize the Backlog & Unscheduled list by grouping items — including by status — to make a long backlog easier to work through.

### Improvements

#### Accurate Linear statuses
- **Real workflow states** - Ticket status, colors, and completion now reflect your project's actual Linear workflow states (your real Todo / In Progress / Done and any custom states) instead of generic ones.

#### Milestones in the right order
- **Match Linear's ordering** - Milestones now appear in the same order you've arranged them in Linear, everywhere they're shown.

#### Backlog toolbar
- **Responsive layout** - The backlog toolbar now collapses gracefully on narrower screens.

#### Quick-create button
- **Create an issue from anywhere** - A floating "+" button now sits in the bottom-right corner and opens the new issue dialog with a single click — the same as pressing C — making it easy to add work on touch devices or without reaching for the keyboard.

### Bug Fixes

- **In-app notifications now appear** - Confirmation and warning toasts (for example after creating an issue) now show up correctly.

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
