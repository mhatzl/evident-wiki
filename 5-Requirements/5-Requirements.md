This section contains requirements for the system.

## Requirements Overview

**High-Level Active Requirements:**

- [req:cap](5-REQ-cap) ... Contains requirements about capturing events
- [req:event](5-REQ-event) ... Contains requirements about the structure of an event
- [req:pub](5-REQ-pub) ... Contains requirements about how events are published
- [req:qa](5-REQ-qa) ... Contains requirements about general quality assurance
- [req:subs](5-REQ-subs) ... Contains requirements about event-subscriptions

**Important Active Requirements:**

- [req:event.id](5-REQ-event.id) ... Contains requirements about event-IDs
- [req:pub](5-REQ-pub) ... Contains requirements about how events are published

## Requirements Tag

Tags help to easily reference requirements.
Requirement tags may be grouped to create a hierarchy of requirements.
Tags of sub-requirements are separated by a dot "." from the parent requirement tag.

**Note:** Tags must not include any whitespace or `-` to keep tags readable in wiki titles.

## Requirement Phases

A requirement goes through the following phases:

1. Requirements are **proposed**, by creating feature-request issues
2. Once a requirement has enough information available to be implemented, it is **ready**, and must be documented in the wiki with a unique tag for tracing 
3. A requirement in **proposed** or **ready** state may be **declined**, meaning that it will not be implemented, and must be removed from the wiki if it already exists
4. When the implementation of a requirement is merged, the requirement gets **active**, and the number of times the requirement is referenced is added to the wiki

   **Example:**

   ```
   # my_req: Some implemented requirement
   
   **References**

   - in branch main: 2
   ```

5. If a requirement is replaced or removed by another requirement, the requirement gets **deprecated**.

   Since the requirement might still be **active** in some branches, `deprecated` must be set manually to the branches
   the requirement is deprecated.

   The *references* list may be replaced by `**deprecated**` if the requirement is **deprecated** in all branches. 

   **Note:** A link should be added in the **deprecated** requirement, pointing to the new requirement for better traceability.

   **Examples:**

   ```
   # my_req: Got deprecated in latest version

   **References**

   - in branch main: deprecated
   - in branch stable: 2
   ```

   ```
   # my_req: Deprecated in all supported versions

   **deprecated**

   Deprecated by [req:new_req].
   ```
