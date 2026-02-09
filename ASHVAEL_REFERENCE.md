# Ashvael Character Sheet - Complete Reference

## Campaign & Rules
- **Rules Version**: D&D 2024 (One D&D / 2024 Player's Handbook)
- **Campaign**: Spelljammer (no spoilers requested)
- **Character Level**: 5

## Character Details
- **Name**: Ashvael
- **Class**: Druid (Circle of Stars)
- **Species**: Half-Aasimar / Half-Tiefling
- **Background**: Guide
  - Skill Proficiencies: Survival (proficient), Stealth (NOT proficient - need to fix in sheet)
  - Tool Proficiency: Cartographer's Tools
  - Feat: Magic Initiate (Druid) - already implemented

## Feats
| Feat | Source | Effect |
|------|--------|--------|
| Magic Initiate: Druid | Guide Background | 2 cantrips (Produce Flame, Mending), Healing Word 1/day free, always prepared |
| War Caster | Level 4 ASI | Advantage on concentration saves, can cast somatic spells with hands full |

---

## Level Progression (1-10)

### Level 1
- **Proficiency Bonus**: +2
- **Spell Slots**: 2x 1st level
- **Cantrip Damage**: Base (1 die)
- **Class Features**:
  - Druidic (secret language)
  - Spellcasting
  - Druid Circle: Circle of Stars
  - Star Map (can cast Guiding Bolt free, WIS mod times per long rest = 4/day)
  - Starry Form (use Wild Shape to activate: Archer, Chalice, or Dragon)
- **Species Traits (Half-Aasimar)**:
  - Celestial Resistance (Necrotic, Radiant)
  - Darkvision 60 ft
  - Healing Hands (1/long rest, heal 1d4 per level)
  - Light Bearer (Light cantrip)
- **Species Traits (Half-Tiefling)**:
  - Infernal Legacy (varies)

### Level 2
- **Proficiency Bonus**: +2
- **Spell Slots**: 3x 1st level
- **Class Features**:
  - Wild Shape (2 uses per short rest)
  - Wild Companion (can use Wild Shape OR spell slot to cast Find Familiar as Fey)

### Level 3
- **Proficiency Bonus**: +2
- **Spell Slots**: 4x 1st level, 2x 2nd level
- **Species Feature**:
  - Celestial Revelation (1/long rest): Choose Inner Radiance, Necrotic Shroud, or Radiant Soul

### Level 4
- **Proficiency Bonus**: +2
- **Spell Slots**: 4x 1st level, 3x 2nd level
- **Class Features**:
  - Ability Score Improvement OR Feat
- **Feat Taken**: War Caster
  - Advantage on Constitution saves to maintain concentration
  - Can perform somatic components with hands full (shield/weapon)
  - Can cast certain spells as opportunity attack (not implemented yet)

### Level 5
- **Proficiency Bonus**: +3
- **Spell Slots**: 4x 1st level, 3x 2nd level, 2x 3rd level
- **Cantrip Damage**: Increases to 2 dice (level 5 scaling)
- **Class Features**:
  - Wild Shape improvement: CR 1/2 beasts (was CR 1/4)
  - Wild Shape: Gain 5 temp HP (equal to druid level)

### Level 6
- **Proficiency Bonus**: +3
- **Spell Slots**: 4x 1st, 3x 2nd, 3x 3rd
- **Class Features**:
  - Circle of Stars: Cosmic Omen (reaction to add/subtract d6 from rolls within 30ft)

### Level 7
- **Proficiency Bonus**: +3
- **Spell Slots**: 4x 1st, 3x 2nd, 3x 3rd, 1x 4th

### Level 8
- **Proficiency Bonus**: +3
- **Spell Slots**: 4x 1st, 3x 2nd, 3x 3rd, 2x 4th
- **Class Features**:
  - Ability Score Improvement OR Feat

### Level 9
- **Proficiency Bonus**: +4
- **Spell Slots**: 4x 1st, 3x 2nd, 3x 3rd, 3x 4th, 1x 5th

### Level 10
- **Proficiency Bonus**: +4
- **Spell Slots**: 4x 1st, 3x 2nd, 3x 3rd, 3x 4th, 2x 5th
- **Class Features**:
  - Circle of Stars: Twinkling Constellations (change Starry Form constellation at start of each turn)
- **Cantrip Damage**: Still 2 dice (next increase at level 11)

---

## Free Resources (per rest)

| Resource | Uses | Recharge | Source |
|----------|------|----------|--------|
| Guiding Bolt | 4/day | Long Rest | Star Map (WIS mod) |
| Healing Word | 1/day | Long Rest | Magic Initiate: Druid |
| Healing Hands | 1/day | Long Rest | Aasimar Ancestry |
| Celestial Revelation | 1/day | Long Rest | Aasimar Ancestry (level 3) |
| Wild Shape | 2/rest | Short Rest | Druid Class |

---

## Ability Scores (Normal Form)
| Ability | Score | Modifier | Save |
|---------|-------|----------|------|
| STR | 8 | -1 | -1 |
| DEX | 14 | +2 | +2 |
| CON | 15 | +2 | +2 |
| INT | 8 | -1 | -1 |
| WIS | 18 | +4 | +7 (prof) |
| CHA | 13 | +1 | +1 |

---

## UI/UX Preferences

### Spell Casting Flow
- Free resource spells appear IN the Cast Spell menus (not separate buttons)
- When selecting a spell with free uses OR slot options, show ALL options:
  - Free use (X/day remaining) - if available
  - 1st level slot
  - 2nd level slot (upcast) - with damage/healing preview
  - 3rd level slot (upcast) - with damage/healing preview
- Guiding Bolt: Shows in "Cast Spell (Action)" with free + slot options
- Healing Word: Shows in "Cast Spell (Bonus)" with free + slot options

### Summoning & Companions
- **Support MULTIPLE companions simultaneously** (e.g., Familiar + Summon Beast)
- Show separate stat blocks for each active companion
- Summon Beast: Must select environment (Air/Land/Water) when casting
- Wild Companion (Find Familiar): Select familiar form when summoning
- When concentration ends, dismiss only the concentration-based companion
- Companion stat blocks show:
  - Name, AC, HP (editable), Speed
  - Attack information (to-hit, damage)
  - Clickable abilities that show full description

### Wild Shape
- When transforming, update:
  - STR, DEX, CON scores (visual indicator)
  - Skill modifiers (recalculate based on new ability scores)
  - AC (use beast's AC)
  - Speed (use beast's speed)
- **DO NOT show beast HP** - keep showing character's HP
- **Add 5 temp HP** when transforming (druid level)
- Keep INT, WIS, CHA and proficiency bonuses
- Show beast's attack information
- **DISABLE spell casting** while in Wild Shape beast form
  - Grey out or hide Cast Spell buttons
  - Show warning if user tries to cast
- When Wild Shape ends, restore all stats to normal

### Starry Form
- Uses Wild Shape resource but is NOT beast transformation
- CAN still cast spells in Starry Form
- Show form-specific bonus action (Archer attack) if applicable

### Action Bar
- Wild Companion should be in the MIDDLE of the action bar (not at the end)
- Large touch targets for mobile (min 44px)

### General UI
- Collapsible spell level sections to reduce scrolling
- Tap features to see full detailed description
- Show damage/healing previews when selecting spells
- Concentration warnings when casting new concentration spell

---

## Cantrip Scaling (Level 5)

| Cantrip | Level 1-4 | Level 5-10 | Level 11-16 | Level 17+ |
|---------|-----------|------------|-------------|-----------|
| Produce Flame | 1d8 | 2d8 | 3d8 | 4d8 |
| Thorn Whip | 1d6 | 2d6 | 3d6 | 4d6 |
| Guidance | +1d4 | +1d4 | +1d4 | +1d4 |
| Druidcraft | N/A | N/A | N/A | N/A |
| Light | N/A | N/A | N/A | N/A |

---

## Spells Known/Prepared

### Always Prepared (cannot change)
- **Guiding Bolt** (Star Map - Circle of Stars)
- **Healing Word** (Magic Initiate: Druid feat)

### Prepared Spells (can change on long rest)
- Druids prepare WIS mod + Druid level spells = 4 + 5 = 9 spells
- (List needs to be confirmed with user)

---

## Inventory System (Planned)
- Equipment slots: Armor, Shield, Weapon (main), Weapon (off-hand), etc.
- When equipping armor/shield, update AC display
- When equipping weapon, add attack option
- Track attunement slots (max 3)
- Track carrying capacity

---

## Technical Details
- **Platform**: PWA hosted on GitHub Pages
- **URL**: https://shivori.github.io/ashvael/
- **Device**: iPhone 15 Pro (primary)
- **Browser**: Safari for iOS
- **Local files**: `c:\Users\Lirid\Nextcloud\DND\Character sheets\ashvael-pwa\`
- **GitHub**: Shivori/ashvael

---

## Error Checking
- Always check browser console (F12) for JavaScript errors after changes
- Service Worker errors on file:// protocol are expected (only works on http/https)
- CORS errors on file:// protocol are expected (test on GitHub Pages for full functionality)

---

## Change Log

### Session 1 (Initial)
- Created PWA with manifest and service worker
- Added spell casting with free resources
- Added Wild Shape beast forms
- Added companion stat blocks
- Set up GitHub Pages hosting

### Session 2
- Fixed orphaned JavaScript code causing errors
- Added clickable ability descriptions for companions
- Fixed Wild Shape skill modifier updates

### Session 3 (Current)
- **Multiple Companions**: Now supports both Familiar AND Summon Beast simultaneously
  - Each companion shown with separate stat block
  - Different colors: Blue for Familiar, Purple for Beast
- **Cantrip Damage**: Updated to 2 dice for level 5
  - Produce Flame: 2d8
  - Thorn Whip: 2d6
  - Starry Wisp: 2d8
- **Always Prepared Spells**:
  - Guiding Bolt (Star Map) and Healing Word (Magic Initiate) now shown as always prepared
  - Removed separate "Free" buttons - now in Cast Spell menus
- **Wild Companion**: Moved to middle of action bar (after Cast Spell)
- **Wild Shape Fixes**:
  - Added safety checks for missing element IDs
  - Spell buttons are disabled during Wild Shape
- **Fixed JS Errors**: Added null checks to prevent crashes

### Session 4 - Inventory System
- **Complete Equipment System Implemented**:
  - Equipment slots: Main Hand, Off Hand, Armor, Head, Neck, Hands, Feet, Ring 1, Ring 2
  - Starting gear: Scimitar (main hand), Shield (off hand), Hide Armor (equipped), Shortbow (in inventory)
  - Two-handed weapon switching: Automatically unequips shield when equipping bow
  - Auto AC calculation from equipped armor + shield
- **Add Equipment Forms**:
  - Weapon form: type, hands, damage die, modifier (STR/DEX/finesse), magic properties
  - Armor form: type, base AC, max DEX, stealth disadvantage, magic properties
  - Shield form: AC bonus, magic properties
  - Accessory form: slot, attunement, effects
- **Attunement tracking**: Shows attuned items (max 3)
- **Updated Starting Gold**: 3 GP (from Guide background)

### Session 5 - Magic Item Effects System (Phase 1 & 2)
- **Phase 1 - Basic Magic Effects**:
  - Damage resistances/immunities
  - Condition immunities
  - Extra damage (always or command word)
  - Extra damage vs creature types
  - Speed bonuses (fly, swim, climb)
  - Advantage on checks/saves
  - Light sources
  - Darkvision
- **Phase 2 - Charges & Spells**:
  - Charge-based items (wands, staffs): configurable max charges, recharge dice, break chance
  - Spells from charges with different costs
  - Item-granted spells (at-will, 1/day, 2/day, 3/day)
  - Item spells appear in Cast Spell menu
  - Recharge on short/long rest with roll notification
  - Magic Item Charges card on Stats tab
- **Wild Shape Skills Fix** (in progress):
  - Created dynamic skill calculation system
  - Skills now use formula: ability mod + proficiency bonus (if proficient) + static bonus
  - Physical skills (STR/DEX based) recalculate when Wild Shape changes ability scores
  - Mental skills (INT/WIS/CHA based) unchanged in Wild Shape
  - All skill elements now have IDs for dynamic updates

### Session 5 - Corrections Made
- **Stealth**: Now correctly marked as PROFICIENT (+5 = DEX +2 + Prof +3)
- **Guide Background**: Gives Stealth + Survival proficiency (not Insight)

### Session 6 - Completed Features
- **Druid Armor Proficiency**: Removed medium armor (only Light + Shields now)
- **Collapsible Sections**: All cards expandable/collapsible with state saved to localStorage
  - Skills, Character Info, Resource Slots, Actions cards all collapsible
  - Magic Item Charges integrated into Resource Slots card
- **Ammunition Tracking**:
  - Auto-decrement arrows/bolts on ranged attacks
  - Shows ammo count in attack selection menu
  - Disables attack when out of ammo
  - "Add Ammo" button in inventory to replenish
- **Thrown Weapons**:
  - Added "melee/thrown" weapon type option
  - Thrown weapons appear in BOTH melee AND ranged attack sections
  - When thrown: weapon unequips and goes to "thrown weapons" list
  - "Reclaim" buttons to pick up thrown weapons
  - Added sample Dagger to starting inventory
- **Adventuring Gear Improvements**:
  - Enhanced gear data structure with descriptions, weight, consumable flag, units
  - Click any gear item to see full details in modal
  - Tool proficiency info shows related checks and common uses (Cartographer's Tools)
  - +/- buttons for consumable items (rations, torches, rope)
  - "Use" button in detail modal for consumables
  - "Add Gear" modal with quantity, weight, unit, consumable options
  - Icons distinguish gear types: 🛠️ tools, 📦 consumables, 🎒 general
- **Custom Spell Details** (for Magic Items):
  - When adding "Other (Custom)" spell to magic item, full spell editor appears
  - Captures: School, Casting Time, Range, Duration, Concentration, Ritual
  - Components (V/S/M with material details)
  - Damage/Healing dice, Save DC type
  - Full description text, At Higher Levels scaling
  - Custom spell details display in spell modal when casting
- **Equipment Reformatting**:
  - Verified DEFAULT_INVENTORY uses consistent new format
  - Fixed starting gold in background description (3 GP, not 7 GP)
  - Added Tent and Cartographer's Tools to starting equipment description
  - Cleaned up duplicate HTML comments

### All Feature Backlog Items Complete!

---

## Answered Questions
- **Background**: Guide (skill proficiencies: Survival, tool: Cartographer's Tools)
- **Prepared Spells**: User will select in-app
- **Feats**: Magic Initiate (from Background) + War Caster (from Level 4 ASI)

---

## Starting Equipment (from Guide Background + existing)

### Currently Owned
| Item | Type | Notes |
|------|------|-------|
| Scimitar | Weapon (melee) | 1d6 slashing, finesse, one-handed |
| Dagger | Weapon (melee/thrown) | 1d4 piercing, finesse, 20/60 ft thrown |
| Shield | Armor | +2 AC |
| Shortbow | Weapon (ranged) | 1d6 piercing, two-handed, 80/320 ft |
| 20 Arrows | Ammunition | |
| Quiver | Container | |
| Hide Armor | Armor | AC 12 + DEX (max 2) = AC 14 |
| Cartographer's Tools | Tool | Proficient |
| Bedroll | Adventuring Gear | |
| Tent | Adventuring Gear | |
| Traveler's Clothes | Clothing | |
| 3 GP | Currency | Starting gold |

---

## Inventory System Design

### Equipment Slots
| Slot | Current | Notes |
|------|---------|-------|
| Main Hand | Scimitar | One-handed weapon |
| Off Hand | Shield | +2 AC |
| Armor | Hide Armor | AC 12 + DEX (max 2) |
| Head | Empty | Hats, helmets, circlets |
| Neck | Empty | Amulets, necklaces |
| Hands | Empty | Gloves, gauntlets |
| Feet | Empty | Boots |
| Ring 1 | Empty | |
| Ring 2 | Empty | |

### Weapon Switching Logic
- **Two-handed weapons** (shortbow, greataxe, etc.) = uses BOTH hand slots
- When equipping two-handed: automatically unequips shield
- When equipping one-handed + shield: automatically unequips two-handed
- **Versatile weapons**: Can be used one or two-handed (different damage)

### Weapon Creation Fields
```
- Name
- Type: Melee / Ranged / Mixed (thrown)
- Hands: One-handed / Two-handed / Versatile
- Damage Die: d4, d6, d8, d10, d12
- Damage Type: Slashing, Piercing, Bludgeoning, etc.
- Modifier: STR / DEX / Finesse (choose)
- Range (if ranged): Normal/Long
- Properties: Light, Heavy, Finesse, Thrown, etc.
- Magic Item: Yes/No
  - If Yes:
    - Requires Attunement: Yes/No
    - Attack Bonus: +1, +2, +3
    - Damage Bonus: +1, +2, +3
    - Special Effect: (text description)
    - Grants Spells: (list)
```

### Armor Creation Fields
```
- Name
- Type: Light / Medium / Heavy / Shield
- Base AC (or bonus for shield)
- Max DEX bonus (if applicable)
- Stealth Disadvantage: Yes/No
- Magic Item: Yes/No
  - If Yes:
    - Requires Attunement: Yes/No
    - AC Bonus: +1, +2, +3
    - Special Effect: (text description)
```

### Attunement
- Maximum 3 attuned items
- Track which items require attunement
- Warning when at limit
