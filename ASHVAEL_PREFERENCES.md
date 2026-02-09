# Ashvael Character Sheet - Development Preferences

## User Setup
- **Device**: iPhone 15 Pro (primary use)
- **Platform**: PWA hosted on GitHub Pages (https://shivori.github.io/ashvael/)
- **Browser**: Safari for iOS
- **Backup location**: Nextcloud sync folder

## App Behavior Preferences

### Spell Casting Flow
- **Free resource spells should appear in Cast Spell menus** (not separate buttons)
- When selecting a spell with free uses OR slot options, show ALL options:
  - Free use (X/day remaining)
  - 1st level slot
  - 2nd level slot (upcast) - with damage/healing preview
  - 3rd level slot (upcast) - with damage/healing preview
- Example: Healing Word in "Cast Spell (Bonus)" shows:
  - "Free (1/day)" option
  - "1st Level Slot" option
  - "2nd Level Slot (Upcast) - 4d4+4 healing"
  - "3rd Level Slot (Upcast) - 6d4+4 healing"

### Summoning Spells
- **Summon Beast**: Must select environment (Air/Land/Water) when casting
  - Companion stat block updates based on environment choice
  - Shows correct speed, abilities, and attacks for chosen type
- **Wild Companion (Find Familiar)**: Select familiar form when summoning
- When concentration ends, companion stat block should disappear automatically

### Companion Stat Block
- Show: Name, AC, HP (editable), Speed
- Show: Attack information (to-hit, damage)
- Abilities should be **clickable** to show full description
  - Example: Tap "Flyby" to see "Doesn't provoke opportunity attacks when flying out of reach"
  - Example: Tap "Keen Hearing/Sight" to see full description
- Dismiss button to remove companion
- Auto-remove when HP reaches 0
- Auto-remove when concentration ends (for Summon Beast)

### UI/UX Preferences
- Large touch targets for mobile (min 44px)
- **Collapsible sections**: ALL cards should be expandable/collapsible (like spell lists)
- Tap features to see full detailed description
- Show damage/healing previews when selecting spells
- Concentration warnings when casting new concentration spell

### Magic Item Charges Display
- **Prefer integrating with Resource Slots** rather than separate card
- Show charges as visual bars with current/max count
- Click to open modal for casting spells from charges

### Ammunition & Thrown Weapons
- When attacking with bow (uses Arrows) or crossbow (uses Bolts):
  - Auto-decrement ammunition quantity
  - Need function to add ammunition and update quantity
- Thrown weapons (daggers, javelins, etc.):
  - Should appear in BOTH melee AND ranged attack options
  - When thrown: weapon gets unequipped until reclaimed
  - Add "Reclaim" button for thrown weapons
- Weapon type options should be: Melee, Ranged, Thrown, Melee/Thrown

### Inventory & Gear
- **Adventuring Gear**: Click item to see full info
  - Show description, weight, uses
  - **Adjustable quantities** for consumables (rations, torches, rope, etc.)
  - Track usage (ate a ration, used a torch, cut rope, etc.)
- **Tool Proficiencies**: Click tools to see full usage info
  - What checks they can be used for
  - Required materials/components
  - DC examples

### Wild Shape
- When transforming, update:
  - STR, DEX, CON scores (visual indicator)
  - **Skill modifiers recalculate dynamically** using formula:
    - skill mod = ability mod + proficiency bonus (if proficient)
  - Only physical skills (STR/DEX based) change
  - Mental skills (INT/WIS/CHA based) stay the same
  - AC (use beast's AC)
  - Speed (use beast's speed)
- **DO NOT show beast HP** - keep showing character's HP
- **Add 5 temp HP** when transforming (druid level)
- Keep INT, WIS, CHA and proficiency bonuses
- Show beast's attack information
- **DISABLE spell casting** while in Wild Shape beast form

### Data Persistence
- Save all state to localStorage
- Version state schema to handle updates gracefully
- Auto-reset corrupted state

## Technical Notes
- PWA with offline support via service worker
- Files hosted on GitHub: Shivori/ashvael
- Local development folder: `c:\Users\Lirid\Nextcloud\DND\Character sheets\`
- GitHub Pages URL: https://shivori.github.io/ashvael/

## Update Workflow
1. Edit files in `Character sheets\ashvael-pwa\` folder
2. Commit and push to GitHub
3. Changes go live automatically on GitHub Pages

## Character Details (Ashvael)
- Level 5 Circle of Stars Druid
- Half-Aasimar/Half-Tiefling
- Key features: Star Map, Starry Form, Wild Shape, Wild Companion
- Free resources:
  - Guiding Bolt: 4/long rest (Star Map)
  - Healing Word: 1/long rest (Magic Initiate)
  - Healing Hands: 1/long rest (Ancestry)
  - Celestial Revelation: 1/long rest (Ancestry)
  - Wild Shape: 2/short rest

## Character Corrections to Apply
- **Druid Armor Proficiency**: NO medium armor proficiency (only Light armor + shields)
  - Medium armor only available with Warden subclass option
  - Need to update Character Info section
- **Skill Proficiencies**:
  - Guide Background gives: Stealth + Survival (NOT Insight)
  - Stealth is PROFICIENT (+5)
  - Insight is NOT proficient (+4 is just WIS mod)

## Custom Spell Requirements (for Item Spells)
When adding a custom spell to an item, capture:
- School of magic (Abjuration, Conjuration, etc.)
- Casting time: Action, Bonus Action, or Reaction
- Range: Self, Touch, or X feet
- Area effect (optional): Cube, Sphere, Cone, Line, Cylinder + dimensions
- Components: V (Verbal), S (Somatic), M (Material with details)
- Duration: Instantaneous, 1 minute, 10 minutes, 1 hour, 8 hours, 24 hours, Until dispelled
- Concentration: Yes/No
- Ritual: Yes/No
- Damage/Healing dice (optional)
- DC save (optional) + effect on fail (half damage, no effect, etc.)
- Full description text
- At higher levels: scaling damage/healing, increased duration, increased summon HP, etc.
- Companion info (optional): for summon spells
