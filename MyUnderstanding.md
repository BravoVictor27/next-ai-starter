# Project Understanding

## Overview
This is a Next.js template designed for building full-stack web applications, optimized for AI coding assistants. The project uses modern tools and libraries and includes Storybook for component development.

## File Structure Analysis

### Configuration Files
- `package.json` & `package-lock.json`: Node.js project configuration and dependencies
- `next.config.ts`: Next.js configuration
- `tailwind.config.ts`: Tailwind CSS configuration
- `tsconfig.json`: TypeScript configuration
- `components.json`: Component configuration (likely for shadcn/ui)
- `postcss.config.mjs`: PostCSS configuration
- `vercel.json`: Vercel deployment configuration

### Core Directories
- `/src`: Main source code directory
  - `/app`: Next.js app router directory
  - Contains authentication pages (`/auth/signin`, `/auth/signout`)
- `/public`: Static assets
- `/prisma`: Database schema and migrations
- `/scripts`: Utility scripts
- `/.storybook`: Storybook configuration

### AI Assistant Related Files
These files are currently using "cursor" naming and might need to be updated to "Windsurf":
- `.cursor-tasks.md`: Task list for AI assistance
- `.cursor-template.xml`: Template configuration
- `.cursor-updates`: Change log file
- `.cursorrules`: Rules and guidelines for AI assistance

## "Cursor" References Analysis

### Files to Consider for Renaming
1. `.cursor-tasks.md` → `.windsurf-tasks.md`
2. `.cursor-template.xml` → `.windsurf-template.xml`
3. `.cursor-updates` → `.windsurf-updates`
4. `.cursorrules` → `.windsurf-rules`

### Code References
1. **UI Elements**: Found in component files with `cursor-not-allowed` CSS classes
   - Location: `src/app/auth/signin/page.tsx`
   - Location: `src/app/auth/signout/page.tsx`
   - Note: These are safe to keep as they are CSS properties unrelated to the tool name

2. **Package Dependencies**:
   - `cli-cursor` and `restore-cursor` in `package-lock.json`
   - Note: These are npm packages unrelated to the tool name and should not be modified

3. **Documentation**:
   - Reference in `README.md` mentioning "Cursor" as an AI coding assistant
   - This should be updated to reference "Windsurf" instead

### Git Configuration
- `.gitignore` contains `.cursor-scratchpad` which should be updated to `.windsurf-scratchpad`

## Recommendations for "Cursor" to "Windsurf" Migration
1. Rename the four main configuration files
2. Update content within these files to reference "Windsurf" instead of "Cursor"
3. Update `.gitignore` entry
4. Update README.md reference
5. No changes needed for:
   - CSS classes containing "cursor"
   - NPM packages with "cursor" in their names
   - Any other technical references to cursor as a concept

## Project Dependencies and Features
- Next.js framework
- TypeScript
- Tailwind CSS for styling
- Storybook for component development
- Authentication system
- Prisma for database management
- Inngest for background jobs/tasks

## Development Guidelines
The project follows modern web development practices with:
- Component-driven development (Storybook)
- Type safety (TypeScript)
- Utility-first CSS (Tailwind)
- Server-side rendering (Next.js)
- Automated AI assistance workflow
