# Requirements — Personal Portfolio (one-page, static)

## Overview
A single static `index.html` file for Clary Mae F. Llaguno's personal portfolio.
All styles inline in one `<style>` block. No framework, no build step, no
backend, no JavaScript. All content written directly in the HTML. Must work
well on a phone.

## Requirement 1: Header identity

**User Story:** As a visitor, I want to immediately see who this person is and
what they do, so that I know whether to keep reading.

### Acceptance Criteria
1. WHEN the page loads THEN THE SYSTEM SHALL display the full name "Clary Mae F. Llaguno".
2. WHEN the page loads THEN THE SYSTEM SHALL display one line describing the role beneath the name.
3. WHEN viewed at 390px wide THEN THE SYSTEM SHALL show both name and role without horizontal scrolling.

## Requirement 2: Exactly three projects

**User Story:** As a visitor, I want to see a small number of representative
projects, so that I can judge capability quickly instead of skimming a long list.

### Acceptance Criteria
1. WHEN the page loads THEN THE SYSTEM SHALL display exactly three project blocks.
2. WHEN each project block is rendered THEN THE SYSTEM SHALL show a title, a single sentence describing it, and one link.
3. WHEN a project link is activated THEN THE SYSTEM SHALL navigate to that project.

## Requirement 3: Contact footer

**User Story:** As a visitor, I want a clear way to reach this person, so that
I can follow up.

### Acceptance Criteria
1. WHEN the page loads THEN THE SYSTEM SHALL display a footer containing an email link, a GitHub link, and a LinkedIn link.
2. WHEN the email link is activated THEN THE SYSTEM SHALL open the user's mail client addressed to clarymaellaguno21@gmail.com.
3. WHEN the GitHub or LinkedIn link is activated THEN THE SYSTEM SHALL navigate to the respective profile.

## Requirement 4: Technical constraints

**User Story:** As the owner, I want the page to be fully static and portable,
so that it can be hosted anywhere with zero tooling.

### Acceptance Criteria
1. WHEN the file is inspected THEN THE SYSTEM SHALL be a single `index.html` with all CSS inside one `<style>` block in `<head>`.
2. WHEN the file is inspected THEN THE SYSTEM SHALL contain no `<script>` element and no external JS, CSS, or framework dependency.
3. WHEN the page is rendered THEN THE SYSTEM SHALL use a dark background, exactly one accent colour, and generous spacing.
4. WHEN viewed on a phone (<=760px) THEN THE SYSTEM SHALL stack the three project cards into a single column.
