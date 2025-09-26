# Mind Matters - Mental Health Platform Design Guidelines

## Design Approach
**Reference-Based Approach**: Drawing inspiration from healthcare platforms like BetterHelp and mental wellness apps like Headspace, combined with productivity tools like Notion for clean, professional interfaces. The design prioritizes trust, accessibility, and emotional comfort.

## Core Design Elements

### A. Color Palette
**Primary Colors:**
- Light Mode: Soft teal (180 65% 45%) for trust and calm
- Dark Mode: Deep teal (180 55% 25%) maintaining brand consistency
- Background: Warm whites (45 15% 98%) in light, deep navy (210 25% 8%) in dark

**Accent Colors:**
- Gentle lavender (260 35% 75%) for therapeutic warmth
- Soft sage green (120 25% 70%) for growth and healing
- Warm coral (15 65% 75%) sparingly for positive actions

**Gradients:**
- Hero sections: Subtle teal to lavender (180 65% 45% to 260 35% 75%)
- Cards and backgrounds: Light sage to warm white overlays

### B. Typography
**Primary:** Inter (Google Fonts) - clean, accessible, professional
**Headings:** Poppins (Google Fonts) - friendly yet authoritative
**Body:** 16px base, increased line height (1.6) for readability
**Weights:** Regular (400), Medium (500), Semibold (600)

### C. Layout System
**Spacing Units:** Consistent use of Tailwind units 4, 6, 8, 12, 16, 24
- Component padding: p-6, p-8
- Section margins: mb-12, mb-16, mb-24
- Card spacing: gap-6, gap-8
- Container max-width: max-w-7xl with generous horizontal padding

### D. Component Library

**Navigation:**
- Clean horizontal nav with role-based menu items
- Soft shadows and rounded corners (rounded-lg)
- Sticky positioning with backdrop blur

**Cards:**
- Elevated cards with subtle shadows
- Rounded corners (rounded-xl)
- Hover states with gentle lift animations
- Consistent padding (p-6, p-8)

**Forms:**
- Generous spacing between fields (space-y-6)
- Rounded inputs (rounded-lg) with focus rings in brand colors
- Multi-step forms for complex registration flows
- Progress indicators for questionnaires

**Buttons:**
- Primary: Solid teal with white text
- Secondary: Outline with teal border
- Rounded style (rounded-lg)
- Adequate padding (px-6 py-3)

**Dashboard Elements:**
- Grid-based layout for feature cards
- Quick action buttons with icons
- Status indicators for appointments/sessions
- Clean sidebar navigation

**Chatbot Interface:**
- Conversational bubble design
- Distinct styling for bot vs user messages
- Typing indicators and smooth message animations
- Questionnaire cards with radio/checkbox styling

### E. Animations
Minimal and purposeful:
- Subtle fade-ins for page transitions
- Gentle hover lifts for interactive elements
- Smooth chatbot message appearances
- No distracting or excessive motion

## Images
**Hero Section:** Large, calming hero image showing diverse people in peaceful, supportive environments (therapy session, meditation, support group). Image should have a warm, soft treatment with gradient overlay.

**Therapist Profiles:** Professional headshots in circular frames
**Dashboard Icons:** Simple, outline-style icons from Heroicons
**Background Elements:** Subtle geometric patterns or soft abstract shapes in brand colors

## Key Principles
1. **Trust-First Design:** Professional appearance with warm, approachable elements
2. **Accessibility:** High contrast ratios, clear typography, intuitive navigation
3. **Emotional Safety:** Calming colors, generous whitespace, non-threatening interface
4. **Role Clarity:** Clear visual distinctions between user types and their interfaces
5. **Mobile-First:** Responsive design prioritizing mobile mental health access