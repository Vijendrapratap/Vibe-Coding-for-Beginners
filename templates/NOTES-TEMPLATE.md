# Project: [YOUR PROJECT NAME]

> This file contains instructions for the AI agent to build your product.
> Fill this out carefully - it's the blueprint the AI will follow.

---

## Project Overview

**Product Name:** [Your product name]

**Description:** [2-3 sentences describing what you're building and what problem it solves]

**Target User:** [Who will use this?]

**MVP Goal:** [What does success look like for this first version?]

---

## Technology Stack

**Frontend:**
- Framework: [e.g., Next.js 14, React 18, vanilla HTML/CSS/JS]
- Styling: [e.g., Tailwind CSS, CSS Modules, styled-components]
- State Management: [e.g., React Context, Redux, none]

**Backend:**
- Platform: [e.g., Supabase, Firebase, Vercel Functions, Node.js]
- Database: [e.g., PostgreSQL (Supabase), Firestore, MongoDB]
- Authentication: [e.g., Supabase Auth, Firebase Auth, Auth0]

**Hosting & Deployment:**
- Hosting: [e.g., Vercel, Netlify, Railway]
- Domain: [your domain or "TBD"]
- CI/CD: [e.g., Vercel auto-deploy, GitHub Actions, manual]

**Third-Party Services:**
- [Service 1]: [Purpose, e.g., Stripe for payments]
- [Service 2]: [Purpose, e.g., SendGrid for emails]
- [Service 3]: [Purpose, e.g., Cloudinary for images]

---

## Database Schema

> Define all data structures your app needs

### Table 1: [table_name]
```
table_name:
  - id: [type, e.g., uuid, primary key]
  - [field_name]: [type and description]
  - [field_name]: [type and description]
  - created_at: [timestamp]
  - updated_at: [timestamp]
```

**Example:**
```
users:
  - id: uuid, primary key
  - email: text, unique, not null
  - full_name: text
  - avatar_url: text, nullable
  - created_at: timestamp

recipes:
  - id: uuid, primary key
  - user_id: uuid, foreign key to users.id
  - title: text, not null
  - ingredients: text, not null
  - instructions: text, not null
  - image_url: text, nullable
  - created_at: timestamp
```

### Relationships
- [Table A] → [Table B]: [relationship type and description]

**Example:**
- users → recipes: One-to-many (one user can have many recipes)

---

## Core Features (Detailed Specifications)

### Feature 1: [Feature Name]

**Description:** [What does this feature do?]

**User Actions:**
1. [Step-by-step what the user does]
2. [Next step]
3. [Result]

**Technical Implementation:**
- **Components needed:**
  - [Component 1 name and purpose]
  - [Component 2 name and purpose]
- **API endpoints (if applicable):**
  - [Endpoint 1: Method, path, purpose]
  - [Endpoint 2: Method, path, purpose]
- **Database operations:**
  - [What data is read/written/updated/deleted]

**Acceptance Criteria:**
- [ ] [Specific criterion 1]
- [ ] [Specific criterion 2]
- [ ] [Specific criterion 3]

**Edge Cases to Handle:**
- [What happens if X goes wrong?]
- [How to handle Y situation?]

---

### Feature 2: [Feature Name]

**Description:** [What does this feature do?]

**User Actions:**
1. [Step-by-step what the user does]
2. [Next step]
3. [Result]

**Technical Implementation:**
- **Components needed:**
  - [Component 1 name and purpose]
  - [Component 2 name and purpose]
- **API endpoints (if applicable):**
  - [Endpoint 1: Method, path, purpose]
  - [Endpoint 2: Method, path, purpose]
- **Database operations:**
  - [What data is read/written/updated/deleted]

**Acceptance Criteria:**
- [ ] [Specific criterion 1]
- [ ] [Specific criterion 2]
- [ ] [Specific criterion 3]

**Edge Cases to Handle:**
- [What happens if X goes wrong?]
- [How to handle Y situation?]

---

### Feature 3: [Feature Name]

[Repeat structure above for each core feature]

---

## Step-by-Step Implementation Plan

> This is the order in which the AI should build features

### Phase 1: Project Setup
- [ ] Initialize [framework] project with TypeScript (if applicable)
- [ ] Install and configure [styling solution]
- [ ] Set up project structure (folders, routing)
- [ ] Configure environment variables
- [ ] Set up [backend service] and obtain credentials
- [ ] Test basic "Hello World" deployment

### Phase 2: Authentication & User Management
- [ ] Set up authentication provider ([service name])
- [ ] Create sign-up page/form
- [ ] Create login page/form
- [ ] Implement logout functionality
- [ ] Create protected route wrapper/middleware
- [ ] Test authentication flow
- [ ] Add error handling for auth failures

### Phase 3: Core Feature 1 - [Feature Name]
- [ ] Create [list components/pages needed]
- [ ] Implement [specific functionality]
- [ ] Add [form/UI elements]
- [ ] Connect to database
- [ ] Add validation
- [ ] Test happy path
- [ ] Test edge cases
- [ ] Add loading and error states

### Phase 4: Core Feature 2 - [Feature Name]
- [ ] [Break down into implementation steps like Phase 3]

### Phase 5: Core Feature 3 - [Feature Name]
- [ ] [Break down into implementation steps]

### Phase 6: Polish & User Experience
- [ ] Apply consistent styling across all pages
- [ ] Add loading spinners/skeletons
- [ ] Add error messages and success notifications
- [ ] Implement responsive design (mobile, tablet, desktop)
- [ ] Add empty states (when no data exists)
- [ ] Optimize images and assets
- [ ] Add page titles and meta tags

### Phase 7: Testing & Bug Fixes
- [ ] Test all user flows from start to finish
- [ ] Test on different browsers (Chrome, Firefox, Safari)
- [ ] Test on mobile devices
- [ ] Fix any bugs discovered
- [ ] Test edge cases (empty inputs, long text, etc.)
- [ ] Verify all acceptance criteria met

### Phase 8: Deployment
- [ ] Set up production database
- [ ] Configure environment variables on hosting platform
- [ ] Deploy to [hosting service]
- [ ] Test production deployment
- [ ] Set up custom domain (if applicable)
- [ ] Verify all features work in production

---

## Design Guidelines & Styling

**Overall Aesthetic:** [modern/minimal/playful/professional/corporate]

**Color Palette:**
- Primary: [color code]
- Secondary: [color code]
- Accent: [color code]
- Background: [color code]
- Text: [color code]
- Error: [color code, e.g., red]
- Success: [color code, e.g., green]

**Typography:**
- Headings: [font family, weights]
- Body text: [font family, size, line height]
- Buttons: [font family, size, weight]

**Component Style:**
- Buttons: [rounded/square, shadow/flat, size]
- Inputs: [style, border, focus state]
- Cards: [shadow, border, padding]
- Spacing: [tight/comfortable/spacious]

**Layout:**
- Max content width: [e.g., 1200px, full width]
- Padding/margins: [e.g., consistent 16px/24px]
- Grid/Flexbox: [preference]

**Responsive Breakpoints:**
- Mobile: [e.g., < 640px]
- Tablet: [e.g., 640px - 1024px]
- Desktop: [e.g., > 1024px]

**Reference:**
- [Link to design inspiration or similar product]
- [Figma/design file if you have one]

---

## Environment Variables

**Required Environment Variables:**

```
# Backend/Database
[VARIABLE_NAME]=[description of what this is]
[VARIABLE_NAME]=[description of what this is]

# Authentication
[VARIABLE_NAME]=[description of what this is]

# Third-party Services
[VARIABLE_NAME]=[description of what this is]

# Optional
[VARIABLE_NAME]=[description of what this is]
```

**Example:**
```
# Supabase
NEXT_PUBLIC_SUPABASE_URL=your-project-url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your-anon-key

# Optional: Analytics
NEXT_PUBLIC_GA_ID=your-google-analytics-id
```

**Where to get these:**
- [Variable 1]: [Instructions on where/how to obtain]
- [Variable 2]: [Instructions on where/how to obtain]

---

## Important Notes & Special Requirements

**Security Considerations:**
- [Important security note 1]
- [Important security note 2]

**Performance Requirements:**
- [Performance requirement 1]
- [Performance requirement 2]

**Accessibility:**
- [Accessibility requirement 1]
- [Accessibility requirement 2]

**Browser Support:**
- Minimum: [e.g., Latest 2 versions of Chrome, Firefox, Safari, Edge]
- Not supporting: [e.g., Internet Explorer]

**Things to Avoid:**
- [Specific thing not to do]
- [Another thing to avoid]
- [Common mistake to watch for]

**Specific Requirements:**
- [Any unique requirements for this project]
- [Constraints or limitations to be aware of]

---

## Testing Checklist

### Functionality Testing
- [ ] All features work as described
- [ ] Forms validate correctly
- [ ] Database operations succeed
- [ ] Authentication flows work
- [ ] Error messages display properly
- [ ] Success messages display properly

### User Experience Testing
- [ ] Navigation is intuitive
- [ ] Loading states are clear
- [ ] Buttons and links are clickable/visible
- [ ] Forms are easy to fill out
- [ ] Error recovery is smooth

### Cross-Browser Testing
- [ ] Works in Chrome
- [ ] Works in Firefox
- [ ] Works in Safari
- [ ] Works in Edge

### Responsive Testing
- [ ] Mobile (320px - 640px)
- [ ] Tablet (641px - 1024px)
- [ ] Desktop (1025px+)

### Performance Testing
- [ ] Page loads in under 3 seconds
- [ ] Images are optimized
- [ ] No unnecessary re-renders

---

## Questions for AI Agent

**When unclear about implementation, AI should:**
1. [Your preference, e.g., "Choose the simplest approach"]
2. [Your preference, e.g., "Ask me before adding dependencies"]
3. [Your preference, e.g., "Prioritize readability over optimization"]

**Communication style:**
- [e.g., "Explain technical decisions in simple terms"]
- [e.g., "Let me know when each phase is complete"]
- [e.g., "Flag any potential issues before proceeding"]

**If you encounter blockers:**
- [Your preference on how AI should handle blockers]

---

## Project Status

**Current Phase:** [Setup / Development / Testing / Deployment]

**Completed:**
- [ ] [What's been done]
- [ ] [What else is done]

**In Progress:**
- [ ] [What's currently being worked on]

**Next Up:**
- [ ] [What's coming next]

**Blockers:**
- [Any current blockers or issues]

---

## Version History

**v1.0** - [Date] - Initial NOTES.md created
**v1.1** - [Date] - [What changed]

---

## Additional Resources

**Documentation Links:**
- [Framework docs]: [URL]
- [Service docs]: [URL]
- [Other resource]: [URL]

**Similar Projects for Reference:**
- [Project name]: [What to reference from it]

**Community/Support:**
- [Where to get help if needed]

---

**Ready to Build?** Once this file is complete, share it with your AI agent and begin Stage 5: Building!
