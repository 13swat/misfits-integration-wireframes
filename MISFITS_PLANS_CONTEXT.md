# Misfits + Plans: Complete Context Document

> Reference document for continuing work on the Misfits + Plans feature in new sessions.

---

## 1. Core Concept

**Misfits + Plans** is a universal IRL coordination layer that helps friends plan and coordinate real-world hangouts together.

### What It Is NOT
- Just a club meetup coordination tool
- A replacement for ticketing apps
- Another group chat

### What It IS
- A planning layer that sits on TOP of any IRL event
- A way to coordinate the "around the event" logistics (carpool, dinner, splitting costs)
- A friend-focused coordination tool for ANY hangout

---

## 2. Three Plan Sources

| Source | Description | Example |
|--------|-------------|---------|
| **Linked to Club Meetup** | Coordinate with friends attending the same Misfits club event | Marathon crew - 5 friends carpooling to Run Club event |
| **Standalone from Templates** | Use fun templates to quickly create any hangout | Birthday bash, Camping trip, Game night |
| **Imported from External Apps** | Scrape event from BookMyShow/Zomato/Insider and add planning layer | Import "Dune: Part Three" from BookMyShow, add pre-movie dinner & carpool |

### The External Scraping Angle (Key Differentiator)

```
BookMyShow: "Avengers opening night"
     ↓ (import to Misfits)
Misfits Plan:
  - Who's coming (invite friends)
  - Pre-movie dinner at 6 PM
  - Carpool from office
  - Split ticket costs
  - Post-movie discussion
```

**You become the coordination layer on top of every ticketing platform.**

---

## 3. Value Proposition

### For Users
- One place to see ALL upcoming plans (clubs + external events + friend plans)
- Easy coordination without messy WhatsApp groups
- Templates make planning fast
- Split costs, assign tasks, coordinate logistics

### For Misfits (Business)
- Higher K-factor (invite friends to any event, not just club meetups)
- Increased engagement (users return for planning, not just discovery)
- Network effects (more friends = more plans)
- Potential premium templates as monetization

### Competitive Positioning
| vs. WhatsApp Groups | vs. Partiful/IRL | vs. BookMyShow |
|---------------------|------------------|----------------|
| Structured > Chaos | India-focused, club integration | Planning layer on top, not competition |
| Tasks & assignments | Template marketplace | Scraping + coordination |
| Persistent plans | Misfits community built-in | Social layer they lack |

---

## 4. Key User Flows

### Flow 1: Club Meetup → Crew Plan
1. User sees club meetup in Misfits
2. Taps "Going with friends?" prompt
3. Creates a "Crew" (private plan linked to meetup)
4. Invites friends, adds carpool/dinner logistics
5. Friends receive invite, join crew
6. Coordinate via crew chat + tasks

### Flow 2: Import External Event
1. User taps "Create Plan" → "Import from Apps"
2. Pastes BookMyShow/Zomato URL
3. Event details auto-fetched
4. Selects coordination options (tickets, dinner, carpool, etc.)
5. Invites friends
6. Plan created with event as anchor

### Flow 3: Standalone Plan from Template
1. User taps "Create Plan" → "Use Template"
2. Browses template marketplace (Birthday, Camping, Game Night, etc.)
3. Selects template, customizes for their event
4. Invites friends
5. Template tasks auto-populated with timeline

---

## 5. Design System (From Actual Misfits App)

### Primary Colors
| Token | Hex | Use |
|-------|-----|-----|
| Primary Blue | `#1E7ACC` | Main brand color |
| Secondary Gold | `#FABB22` | Accent, highlights, focus states |
| Premium Purple | `#7B45BA` | Premium features |
| Success Green | `#006D3C` (light) / `#51DF8E` (dark) | Success states |
| Error Red | `#BA1A1A` (light) / `#FFB6B2` (dark) | Error states |

### Surface Colors (Light Mode)
| Level | Hex | Use |
|-------|-----|-----|
| Level 0 | `#FCFCFD` | Base background |
| Level 1 | `#FFFFFF` | Cards, containers |
| Level 2 | `#F4F4F5` | Elevated surfaces |
| Level 3 | `#EAEAEB` | Tertiary surfaces |
| Disabled | `#E5E5E5` | Disabled states |

### Surface Colors (Dark Mode)
| Level | Hex | Use |
|-------|-----|-----|
| Level 0 | `#191C20` | Base background |
| Level 1 | `#272A2F` | Cards |
| Level 2 | `#32353A` | Elevated |
| Level 3 | `#46474A` | Tertiary |

### Text Colors (Light Mode)
| Token | Hex | Use |
|-------|-----|-----|
| Neutral | `#191C20` | Main body text |
| Neutral Variant | `#46474A` | Secondary/hint text |
| Disabled | `#717175` | Disabled text |
| On Primary | `#FFFFFF` | Text on primary color |

### Typography
- **Font Family:** Lato
- **Weights:** 300 (Light), 400 (Regular), 600 (Semi-Bold), 700 (Bold), 900 (Black)

| Style | Size | Weight |
|-------|------|--------|
| Headline Large | 32px | 600 |
| Headline Medium | 28px | 600 |
| Headline Small | 24px | 600 |
| Title Large | 22px | 600 |
| Title Medium | 16px | 700 |
| Body Large | 16px | 400 |
| Body Medium | 14px | 400 |
| Body Small | 12px | 400 |
| Label Large | 14px | 700 |
| Label Small | 11px | 600 |

### Border Radius
- Small: 4px
- Medium: 8px
- Large: 12px
- XL: 16px
- Full/Pill: 100px

### Shadows (Light Mode)
```css
/* Card shadow */
shadow-card-light: 0 1px 2px rgba(0,0,0,0.04),
                   0 4px 8px -2px rgba(24,39,75,0.06),
                   0 12px 24px -4px rgba(24,39,75,0.08);

/* Glow effects */
shadow-glow-primary: 0 4px 14px -2px rgba(30,122,204,0.4);
shadow-glow-secondary: 0 4px 14px -2px rgba(245,166,35,0.4);
```

### Gradients
| Name | Gradient |
|------|----------|
| Primary | `#1E7ACC` → `#1565a8` |
| Secondary | `#F5A623` → `#e69500` |
| Suggest Button | `#6A2FA0` → `#DE3850` (Purple to Red) |

---

## 6. Design Direction (User Preferences)

### Vibe
**Playful & Fun** - Bright colors, rounded shapes, illustrations, casual tone

### Target Audience
**Mixed 18-34** - Appeals to both Gen Z (18-24) and Young Professionals (25-34)

### Design References
| App | What to Take |
|-----|--------------|
| **Partiful** | Playful event pages, bold gradients, confetti animations, meme-friendly |
| **IRL** | Clean social calendar, subtle colors, group avatars, minimal UI |
| **Discord** | Community-focused, feature-rich, dark mode excellence |

### Key Insight
User rejected initial theme explorations (Sunshine/Electric/Soft Social). Wants to share their own inspirations before finalizing design direction.

---

## 7. Wireframes Created

### Live URL
https://13swat.github.io/misfits-integration-wireframes/

### Screens Completed (12 total)

1. **Unified Home** - Shows clubs + imported events + standalone plans
2. **Your Clubs** - Club membership list
3. **Club Meetups** - Meetup list for a specific club
4. **Meetup Detail** - Event detail with "Going with friends?" prompt
5. **Create Crew Plan** - Create plan linked to meetup
6. **Invite Friends to Crew** - Friend selection for crew
7. **Crew Plan View** - Active plan with tasks, chat, attendees
8. **Friend Receives Invite** - Incoming invite screen
9. **My Plans Tab** - Hosting + Invited plans
10. **Create Plan** - Choose: Scratch / Template / Import
11. **Import Event** - Paste URL from BookMyShow/Zomato/Insider
12. **Browse Templates** - Template marketplace
13. **Template Detail** - Preview template before using

### Local Files
- Main wireframe: `/Users/rentalplaza/misfits-integration-wireframes/index.html`
- Design themes (rejected): `/Users/rentalplaza/misfits-integration-wireframes/design-themes.html`

---

## 8. Supported External Apps (for Import)

| App | Type | URL Pattern |
|-----|------|-------------|
| BookMyShow | Movies, Events, Shows | `in.bookmyshow.com/*` |
| Zomato | Restaurants, Events | `zomato.com/*` |
| Insider | Concerts, Comedy, Experiences | `insider.in/*` |
| Paytm Events | Events, Shows | `paytm.com/events/*` |
| District | Nightlife, Experiences | `district.in/*` |

---

## 9. Template Categories (Planned)

| Category | Examples |
|----------|----------|
| Celebrations | Birthday Party, Anniversary, Graduation |
| Travel | Camping Trip, Beach Day, Road Trip, Weekend Getaway |
| Food & Drink | Brunch Party, Potluck Dinner, Wine Tasting |
| Entertainment | Movie Marathon, Game Night, Karaoke Night |
| Fitness | Cycling Trip, Hiking Adventure, Yoga Retreat |
| Learning | Book Club, Study Group, Workshop |

---

## 10. Open Questions / To Decide

1. **Monetization for Templates** - Free vs. Premium templates? Creator marketplace?
2. **Scraping legality** - Terms of service considerations for BookMyShow/Zomato
3. **Chat integration** - In-app chat vs. WhatsApp deep link?
4. **Notification strategy** - Push notifications for plan updates?
5. **Design direction** - Awaiting user's design inspirations

---

## 11. File Structure

```
/Users/rentalplaza/misfits-integration-wireframes/
├── index.html                    # Main interactive wireframe
├── design-themes.html            # Theme exploration (rejected)
├── MISFITS_PLANS_CONTEXT.md      # This file
└── (GitHub Pages deployed)
```

---

## 12. Next Steps

1. **User to share design inspirations**
2. Create new design theme based on:
   - Actual Misfits color scheme (blue/gold)
   - User's inspirations
   - Playful & Fun vibe
3. Build detailed low-fidelity wireframes in chosen style
4. Define component library
5. Ready for high-fidelity mockups

---

*Last updated: March 2026*
*Session context for Misfits + Plans feature development*
