# Anthropic Research Tools Role - Resume Customization Context

## Role Information
**Position:** Senior+ Software Engineer, Research Tools  
**URL:** https://job-boards.greenhouse.io/anthropic/jobs/4981828008  
**Locations:** San Francisco, CA | New York City, NY  

## Key Role Requirements

### Primary Focus
- Full-stack development for internal research tools
- Building infrastructure and applications for researchers
- Product thinking + rapid iteration
- High agency in ambiguous environments
- User empathy for technical users (researchers, not other engineers)

### Core Responsibilities
- Build full-stack applications researchers use daily
- Partner with research teams to understand workflows
- Design intuitive interfaces for complex research tasks
- Create reusable platforms and tools
- Rapid prototyping with user feedback
- Own complete product areas from conception to delivery

### Technical Stack
- React, TypeScript, Python
- Modern web technologies
- Experimentation platforms
- Data visualization
- Interactive interfaces

### Key Differentiators from Sandboxing Role
- **User:** Researchers (non-technical stakeholders) vs. other engineers
- **Focus:** Product thinking + UX vs. reliability + security
- **Domain:** Applications/interfaces vs. infrastructure/platform
- **Skills:** Rapid iteration, user empathy vs. incident response, observability

## Approved Changes

### 1. Byline
**Decision:** 
```
Software Engineer | Python Expert | Research Tools & Developer Platforms
```

**Rationale:**
- Drops "Backend" qualifier - role is explicitly full-stack
- "Research Tools & Developer Platforms" directly mirrors role title
- General enough to cover both scientific research tooling and technical workflow tools
- "Software Engineer" without qualifier lets skills section speak for itself

### 2. Open Source Addition: jobsearch-tracker

**Project URL:** https://github.com/joeblackwaslike/jobsearch-tracker

**Description:**
```
jobsearch-tracker — https://github.com/joeblackwaslike/jobsearch-tracker
Full-stack job search platform with dashboard, data visualizations, and AI-assisted workflows. Features include a Chrome extension for automatic tracking, multi-stage task orchestration with human-in-the-loop approval, iterative document refinement, and privacy-first integration design. Built with TanStack Start, React 19, Supabase, and shadcn/ui.
```

**Why This Matters for the Role:**

1. **Full-stack application** - TanStack Start/React/TypeScript frontend + Supabase backend
2. **Dashboard & data visualizations** - parallels research tool dashboards
3. **Workflow management** - structured processes for complex tasks
4. **Chrome extension** - browser integration for data capture
5. **AI-assisted workflows** - entire epic around AI integration (see PRD below)
6. **Human-in-the-loop approval** - multi-stage workflows with user review gates
7. **Iterative refinement** - document → feedback → new draft → approval loops
8. **Privacy-first design** - explicit consent modeling, data minimization
9. **Modern stack** - React 19, shadcn/ui, Tailwind, TanStack Router/Query
10. **Complete lifecycle** - authentication, database schema, RLS policies, testing (91 tests)

**Key Technical Alignments from AI Integration PRD:**

The PRD (https://github.com/joeblackwaslike/jobsearch-tracker/blob/2c435704397a4b13bcb4000a15370275ec8af9e8/docs/prds/prd-ai-integration.md) demonstrates:

- **Experiment orchestration patterns:** Inngest for durable task execution, retry logic, backoff
- **Human feedback collection:** Multi-stage approval workflows with iterative refinement
- **Visualization tools:** Dashboard, inbox, document previews, status tracking
- **Task state management:** `pending → running → awaiting_approval → approved → completed`
- **Error classification:** Transient vs. auth vs. rate-limit errors with appropriate handling
- **Privacy/safety thinking:** Consent modeling, data minimization, auditability
- **Building platforms:** Reusable task orchestration system, document versioning, integration health

This demonstrates the exact engineering discipline the role requires: understanding user workflows, building intuitive interfaces, rapid iteration, and complete ownership from conception to delivery.

## Items Still To Review

### 3. Summary Section
**Status:** Not yet reviewed  
**Next step:** Analyze current base summary against role requirements  
**Key considerations:**
- Need to emphasize full-stack (not just backend)
- Product thinking and user empathy
- Rapid iteration and prototyping
- Building tools for technical users
- Current fourth sentence about AI/LLM infrastructure still relevant

### 4. Skills Section
**Status:** Not yet reviewed  
**Considerations:**
- React/TypeScript should be more prominent
- Visualization experience
- Experimentation platforms
- Current AI/LLM section from Sandboxing patch still relevant

### 5. Work Experience
**Status:** Not yet reviewed  
**Considerations:**
- Magic bullets already strong (developer-facing SDK, tooling ecosystem)
- May want to emphasize "users loved it" angle more explicitly
- Product thinking and user feedback incorporation
- Rapid iteration and prototyping

## Patch Strategy

Following the same pattern as Sandboxing role:
- **base.yaml** - contains all universally better changes
- **anthropic_research_tools.yaml** - JSON Patch file with role-specific customizations

Changes will be compared against current base.yaml to produce the patch file.

## References

- **Job Description:** https://job-boards.greenhouse.io/anthropic/jobs/4981828008
- **jobsearch-tracker repo:** https://github.com/joeblackwaslike/jobsearch-tracker  
- **AI Integration PRD:** https://github.com/joeblackwaslike/jobsearch-tracker/blob/2c435704397a4b13bcb4000a15370275ec8af9e8/docs/prds/prd-ai-integration.md
- **Previous Sandboxing patch:** anthropic.yaml (for reference on patch format)