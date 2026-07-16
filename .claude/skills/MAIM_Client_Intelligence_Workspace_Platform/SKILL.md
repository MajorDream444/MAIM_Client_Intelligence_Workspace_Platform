```markdown
# MAIM_Client_Intelligence_Workspace_Platform Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill introduces the core development patterns and workflows for the `MAIM_Client_Intelligence_Workspace_Platform` repository. The codebase is primarily written in TypeScript and is structured without a specific framework, focusing on modular, platform-agnostic client intelligence tooling. This guide covers coding conventions, documentation update workflows, testing patterns, and useful automation commands.

## Coding Conventions

### File Naming
- **Style:** `snake_case`
- **Example:**  
  ```
  user_profile.ts
  client_data_manager.ts
  ```

### Import Style
- **Relative imports are used.**
- **Example:**
  ```typescript
  import { fetchData } from './data_utils';
  import { User } from '../models/user';
  ```

### Export Style
- **Named exports are preferred.**
- **Example:**
  ```typescript
  // In user_profile.ts
  export function getUserProfile(id: string) { ... }

  // In another file
  import { getUserProfile } from './user_profile';
  ```

### Commit Message Patterns
- **Conventional commits are used.**
- **Prefix example:** `docs:`
- **Average length:** ~42 characters
- **Example:**
  ```
  docs: update client boundary documentation
  ```

## Workflows

### Update Platform Documentation
**Trigger:** When documentation needs to be standardized or updated to reflect platform-only or client-agnostic requirements.  
**Command:** `/update-platform-docs`

1. **Identify** documentation files that reference clients or non-platform-specific content.
2. **Edit** the documentation to remove or generalize client-specific references.
3. **Commit** changes with a message indicating the documentation update (e.g., `docs: update platform documentation`).

**Files commonly involved:**
- `docs/client-intelligence-workspace.md`
- `README.md`
- `docs/BUILD_SEQUENCE.md`
- `CODEX.md`
- `docs/CLIENT_001_SHEETAL_BOUNDARY.md`
- `STAGE.md`
- `docs/REPO_BOUNDARY.md`

**Example Workflow:**
```bash
# 1. Open docs/client-intelligence-workspace.md
# 2. Remove or generalize any client-specific references
# 3. Save changes

git add docs/client-intelligence-workspace.md
git commit -m "docs: update platform documentation"
git push
```

## Testing Patterns

- **Test files:** Named with the pattern `*.test.*`
- **Testing framework:** Not explicitly detected (review repo for specifics)
- **Example:**
  ```
  user_profile.test.ts
  ```

- **Typical test structure:**
  ```typescript
  import { getUserProfile } from './user_profile';

  describe('getUserProfile', () => {
    it('should return a user profile for a valid ID', () => {
      // test logic here
    });
  });
  ```

## Commands

| Command                | Purpose                                                        |
|------------------------|----------------------------------------------------------------|
| /update-platform-docs  | Standardize or update documentation for platform requirements. |

```