# Ashvael Character Sheet - Complete Reference

## Campaign & Rules
- **Rules Version**: D&D 2024 (2024 Player's Handbook)
- **Campaign**: Spelljammer (no spoilers requested)
- **Character Level**: 5

---

# PART 1: D&D 2024 CORE RULES

## Proficiency System

### Proficiency Bonus by Level
| Level | Proficiency Bonus |
|-------|-------------------|
| 1-4   | +2 |
| 5-8   | +3 |
| 9-12  | +4 |
| 13-16 | +5 |
| 17-20 | +6 |

**Current (Level 5): +3**

### Armor Proficiency Rules (2024 PHB)

**If wearing armor you are NOT proficient with:**
- Disadvantage on any ability check, saving throw, or attack roll that involves Strength or Dexterity
- **You CANNOT cast spells** while wearing non-proficient armor

> **IMPORTANT FOR IMPLEMENTATION**: If Ashvael equips Medium or Heavy armor (not proficient), the app must:
> 1. Show warning about disadvantage
> 2. **DISABLE all spell casting buttons**
> 3. Show message explaining why spells are disabled

### Shield Proficiency Rules (2024 PHB)

**If using a shield you are NOT proficient with:**
- Same penalties as non-proficient armor (disadvantage, cannot cast spells)
- Druids are proficient with shields (non-metal)

### Weapon Proficiency Rules (2024 PHB)

**When attacking with a weapon you are NOT proficient with:**
- **DO NOT add proficiency bonus to the attack roll**
- Damage roll is unaffected (still add ability modifier)

**Attack Roll Formula:**
- Proficient: d20 + ability modifier + proficiency bonus
- NOT Proficient: d20 + ability modifier (NO proficiency bonus)

> **IMPORTANT FOR IMPLEMENTATION**: When calculating attack bonus for non-proficient weapons:
> - Proficient attack: DEX mod (+2) + Prof (+3) = **+5**
> - Non-proficient attack: DEX mod (+2) only = **+2**

---

## Combat Rules (2024 PHB)

### Action Economy (Per Turn)

| Resource | Amount | Examples |
|----------|--------|----------|
| Movement | Speed (30 ft) | Move up to speed, can split before/after actions |
| Action | 1 | Attack, Cast Spell, Dash, Dodge, Help, etc. |
| Bonus Action | 1 (if available) | Healing Word, Two-Weapon Fighting, Wild Shape |
| Reaction | 1 per round | Opportunity Attack, Shield spell, Absorb Elements |
| Free Object Interaction | 1 | Draw/sheathe weapon, open door |

### Actions in Combat

| Action | Description |
|--------|-------------|
| **Attack** | Make one weapon attack (or more with Extra Attack) |
| **Cast a Spell** | Cast a spell with casting time of 1 Action |
| **Dash** | Gain extra movement equal to speed |
| **Disengage** | Movement doesn't provoke opportunity attacks |
| **Dodge** | Attacks against you have Disadvantage, Advantage on DEX saves |
| **Help** | Give ally Advantage on next check or attack |
| **Hide** | Make Stealth check to become Hidden |
| **Ready** | Prepare action for trigger (uses Reaction when triggered) |
| **Search** | Make Perception or Investigation check |
| **Use an Object** | Interact with object requiring action (use item, drink potion) |

### Making an Attack Roll

1. **Roll d20**
2. **Add modifiers:**
   - Ability modifier (STR for melee, DEX for ranged/finesse)
   - Proficiency bonus (if proficient with weapon)
   - Magic bonus (if magic weapon)
3. **Compare to AC:**
   - Roll total >= AC = Hit
   - Roll total < AC = Miss
   - Natural 20 = Critical Hit (always hits, double damage dice)
   - Natural 1 = Critical Miss (always misses)

### Damage Roll

1. **Roll weapon's damage dice**
2. **Add ability modifier** (same as attack, usually STR or DEX)
3. **Add magic bonus** (if applicable)
4. **Double dice on Critical Hit** (roll twice as many damage dice, add modifiers once)

### Armor Class (AC) Calculation

| Armor Type | AC Formula | Ashvael Note |
|------------|------------|--------------|
| No Armor | 10 + DEX mod | 10 + 2 = 12 |
| Light Armor | Base AC + DEX mod | Leather: 11 + 2 = 13 |
| Medium Armor | Base AC + DEX mod (max +2) | Hide: 12 + 2 = 14 |
| Heavy Armor | Base AC (no DEX) | NOT PROFICIENT |
| Shield | +2 to AC | Adds to above |

**Ashvael's Current AC (Leather + Shield): 11 + 2 (DEX) + 2 (Shield) = 15**

### Saving Throws

**Formula: d20 + ability modifier + proficiency bonus (if proficient)**

Ashvael's Saving Throw Proficiencies (Druid):
- **Intelligence: +2** (proficient: -1 + 3)
- **Wisdom: +7** (proficient: +4 + 3)

### Concentration

- Only one Concentration spell at a time
- Must make Constitution saving throw when taking damage to maintain
- **DC = 10 or half damage taken, whichever is higher**
- War Caster feat: Advantage on Concentration saves

### Opportunity Attacks

- Trigger: Hostile creature moves OUT of your reach
- Uses Reaction
- Make one melee attack against the creature
- Disengage action prevents opportunity attacks

---

## Spellcasting Rules (2024 PHB)

### Spell Slots

Spell slots are expended when casting spells and recover on Long Rest.

**Ashvael's Slots (Level 5 Druid):**
| Level | Slots |
|-------|-------|
| 1st | 4 |
| 2nd | 3 |
| 3rd | 2 |

### Upcasting

Many spells can be cast at higher levels for increased effect:
- Healing Word: 1d4+WIS per level above 1st
- Guiding Bolt: 1d6 per level above 1st
- Cure Wounds: 1d8 per level above 1st

### Spellcasting Focus

- Druids can use a Druidic Focus (Star Map, staff, yew wand, etc.)
- Focus replaces Material components (unless component has a gold cost)
- Ashvael uses Star Map as focus

### Ritual Casting

- Druids can cast ritual spells without expending a slot
- Takes 10 extra minutes to cast
- Spell must be prepared AND have ritual tag

### Cantrip Scaling

Cantrips increase in power at levels 5, 11, and 17.

| Level | Damage Dice |
|-------|-------------|
| 1-4 | 1 die |
| 5-10 | 2 dice |
| 11-16 | 3 dice |
| 17+ | 4 dice |

**Ashvael (Level 5):**
- Produce Flame: 2d8 fire
- Thorn Whip: 2d6 piercing
- Starry Wisp: 2d8 radiant

---

# PART 2: ASHVAEL - CHARACTER DETAILS

## Basic Information
- **Name**: Ashvael
- **Class**: Druid 5 (Circle of Stars)
- **Species**: Half-Aasimar / Half-Tiefling (Homebrew)
- **Background**: Guide
- **Level**: 5
- **Proficiency Bonus**: +3

---

## Ability Scores

| Ability | Score | Modifier | Save (Prof?) |
|---------|-------|----------|--------------|
| Strength | 8 | -1 | -1 |
| Dexterity | 14 | +2 | +2 |
| Constitution | 15 | +2 | +2 |
| Intelligence | 8 | -1 | +2 (Prof) |
| Wisdom | 18 | +4 | +7 (Prof) |
| Charisma | 13 | +1 | +1 |

---

## Species: Half-Aasimar / Half-Tiefling (Homebrew)

### Aasimar Traits (2024 PHB)

| Trait | Description |
|-------|-------------|
| **Creature Type** | Humanoid |
| **Size** | Medium (5-6 feet) |
| **Speed** | 30 feet |
| **Celestial Resistance** | Resistance to Necrotic and Radiant damage |
| **Darkvision** | See in dim light (60 ft) as if bright, darkness as dim (grayscale) |
| **Healing Hands** | Action: Touch one creature, heal HP equal to 1d4 x your Proficiency Bonus. 1/Long Rest |
| **Light Bearer** | Know the Light cantrip. Charisma is spellcasting ability |

### Celestial Revelation (Level 3+)
**1/Long Rest, transform for 1 minute with one of:**

| Form | Effect |
|------|--------|
| **Heavenly Wings** | Gain flying speed equal to walking speed |
| **Inner Radiance** | At end of each of YOUR turns, 10 ft emanation deals Radiant damage = Proficiency Bonus |
| **Necrotic Shroud** | Creatures of choice in 10 ft make CHA save or Frightened of you until end of next turn |

> **CHOICE MADE**: Ashvael can choose any form each time Celestial Revelation is used.

### Tiefling Traits (Partial - Homebrew)
As half-Tiefling, specific traits are determined by DM. Currently using:
- Visual characteristics (appearance)
- Specific infernal legacy features (TBD with DM)

---

## Background: Guide (2024 PHB)

### Skill Proficiencies
- **Stealth** (DEX) - Proficient
- **Survival** (WIS) - Proficient

### Tool Proficiency
- **Cartographer's Tools** - Proficient

### Feat Granted
- **Magic Initiate: Druid**

### Starting Equipment
| Item | Description |
|------|-------------|
| Bedroll | Sleeping gear for camping |
| Tent (2-person) | Shelter for 2 people |
| Tinderbox | Fire-starting kit |
| Traveler's Clothes | Durable traveling outfit |
| Waterskin | Holds 4 pints of water |
| 50 ft Hempen Rope | Standard rope |
| Quiver | Holds up to 20 arrows |
| 20 Arrows | Ammunition |
| Cartographer's Tools | Map-making supplies |
| **3 GP** | Starting gold |

---

## Class: Druid (2024 PHB)

### Hit Points
- **Hit Die**: d8
- **HP at 1st Level**: 8 + CON modifier (10 HP)
- **HP at Higher Levels**: 1d8 (or 5) + CON modifier per level
- **Current Max HP at Level 5**: 8 + 5 + 5 + 5 + 5 + (CON mod x 5) = 38 HP
  - (8 + 4x5 + 2x5 = 8 + 20 + 10 = 38 HP)

### Proficiencies

#### Armor Proficiencies
| Armor Type | Proficient? | Notes |
|------------|-------------|-------|
| Light Armor | YES | Padded, Leather, Studded Leather |
| Medium Armor | NO | NOT proficient (only with Warden subclass) |
| Heavy Armor | NO | NOT proficient |
| Shields | YES | Non-metal only (wood, bone, etc.) |

> **IMPORTANT**: Ashvael wearing Medium or Heavy armor CANNOT cast spells.

#### Weapon Proficiencies
| Weapon Type | Proficient? |
|-------------|-------------|
| Simple Weapons | YES |
| Martial Weapons | NO |

**Simple Weapons (Proficient):**
Club, Dagger, Greatclub, Handaxe, Javelin, Light Hammer, Mace, Quarterstaff, Sickle, Spear, Light Crossbow, Dart, Shortbow, Sling

**Martial Weapons (NOT Proficient):**
Battleaxe, Flail, Glaive, Greataxe, Greatsword, Halberd, Lance, Longsword, Maul, Morningstar, Pike, Rapier, Scimitar, Shortsword, Trident, War Pick, Warhammer, Whip, Blowgun, Hand Crossbow, Heavy Crossbow, Longbow, Net

> **CORRECTED (Session 8)**: Scimitar replaced with Sickle (simple weapon).

#### Tool Proficiencies
- **Herbalism Kit** - Proficient (from Druid class)
- **Cartographer's Tools** - Proficient (from Guide background)

#### Saving Throws
- **Intelligence** - Proficient
- **Wisdom** - Proficient

#### Skills (Choose 2 from Druid list)
Druids choose from: Arcana, Animal Handling, Insight, Medicine, Nature, Perception, Religion, Survival

> **CHOICE MADE**: Nature, Perception
> Background (Guide) grants: Stealth, Survival

### Druid Starting Equipment (Official 2024)
Choose Option A or B:

**Option A:**
- Leather Armor
- Shield
- Sickle (NOT Scimitar - Scimitar is martial)
- Druidic Focus (Staff, Sprig of Mistletoe, Totem, or Wooden Staff)
- Explorer's Pack
- Herbalism Kit
- 9 GP

**Option B:**
- 50 GP to buy equipment

> **CHOICE MADE**: Option A selected
> **Druidic Focus Choice**: Quarterstaff (acts as both focus and weapon, 1d6/1d8 bludgeoning)

### Explorer's Pack Contents (Official 2024)
| Item | Qty | Description |
|------|-----|-------------|
| Backpack | 1 | Holds 1 cubic foot / 30 lbs of gear |
| Bedroll | 1 | Sleeping bag for camping |
| Mess Kit | 1 | Tin utensils (plate, cup, fork, spoon, knife) |
| Tinderbox | 1 | Flint, fire steel, tinder for starting fires |
| Torches | 10 | Each burns 1 hour, 20 ft bright/20 ft dim light |
| Rations | 10 | One day's worth of food each |
| Waterskin | 1 | Holds 4 pints of water |
| Hempen Rope | 50 ft | Standard rope, can be cut |

---

## Druid Class Features

### Level 1 Features

#### Druidic (Language)
- Secret language known only to Druids
- Can use to leave hidden messages
- Others can spot messages with DC 15 Perception, but can't decipher without magic

#### Spellcasting
- **Spellcasting Ability**: Wisdom
- **Spell Save DC**: 8 + Prof + WIS = 8 + 3 + 4 = **15**
- **Spell Attack Bonus**: Prof + WIS = 3 + 4 = **+7**
- **Spellcasting Focus**: Druidic Focus (Star Map)
- **Ritual Casting**: Can cast prepared ritual spells without slot (takes 10 min longer)
- **Preparing Spells**: Can prepare WIS mod + Druid level spells after Long Rest
  - Ashvael can prepare: 4 + 5 = **9 spells**

#### Primal Order
Druids choose Magician or Warden at level 1.

| Order | Benefit |
|-------|---------|
| **Magician** | Know extra cantrip from Druid list |
| Warden | Martial weapon proficiency, Medium armor proficiency |

> **CHOICE MADE**: Magician (extra cantrip)
> Note: This is why Ashvael is NOT proficient with medium armor.

### Level 2 Features

#### Wild Shape
**Uses**: 2 per Short or Long Rest

**Transformation Rules (Level 5):**
- Max CR: 1/2 (was 1/4 at levels 2-4)
- No flying speed allowed (until level 8)
- No swimming speed unless you've seen the beast
- Duration: Druid level / 2 hours = 2.5 hours
- Bonus Action to activate OR use action for Wild Companion

**What Changes in Wild Shape:**
- Gain beast's STR, DEX, CON
- Gain beast's HP as Temp HP (Level 5: gain 5 temp HP)
- Gain beast's AC (natural armor)
- Gain beast's Speed
- Gain beast's attacks and special abilities
- Skills recalculate using new ability scores

**What Stays the Same:**
- INT, WIS, CHA scores
- Proficiencies (skills, saves)
- Personality, alignment, memories
- Class features
- Languages (can understand but not speak)

**Wild Shape Restrictions:**
- **CANNOT cast spells** (no verbal components in beast form)
- Cannot talk
- Cannot use equipment (melds into form)
- Concentration on existing spells continues

**Reverting:**
- Bonus Action to revert
- Automatic when temp HP drops to 0
- Automatic when duration ends
- Automatic if knocked Unconscious

#### Wild Companion
Instead of Wild Shape, can expend a use to cast **Find Familiar** (as a Fey, no material components).

### Level 5 Features

#### Wild Shape Improvement
- Max CR increases to 1/2
- Gain temporary HP equal to Druid level (5)
- Can transform into beasts with swimming speed

---

## Subclass: Circle of Stars

### Level 2: Star Map

**Feature:**
- A Tiny object (constellation map) that serves as Spellcasting Focus
- While holding it:
  - Know the **Guidance** cantrip
  - Can cast **Guiding Bolt** without expending a slot (WIS mod times per Long Rest = 4)
- If lost, can create new one during Long Rest (1 hour meditation)

### Level 2: Starry Form

**Activation**: Bonus Action, expends Wild Shape use

**Duration**: 10 minutes

**Effect**: Body becomes luminous, stars appear on skin

**Choose one constellation when activating:**

| Constellation | Effect |
|---------------|--------|
| **Archer** | Bonus Action: Make ranged spell attack (60 ft), deal 1d8+WIS Radiant damage |
| **Chalice** | When casting healing spell, you OR another creature in 30 ft regains 1d8+WIS HP |
| **Dragon** | Minimum roll of 10 on INT/WIS checks and Concentration saves |

**Key Differences from Wild Shape:**
- Can still cast spells
- Keep your normal form (humanoid appearance with starry effects)
- No beast stat replacements
- Uses Wild Shape resource but is NOT a beast transformation

> **IMPORTANT FOR IMPLEMENTATION**: When in Starry Form:
> - Spell casting remains ENABLED
> - If Archer: Add bonus action attack option
> - If Chalice: Add healing bonus to Cast Spell
> - If Dragon: Apply minimum 10 to relevant rolls

### Level 6: Cosmic Omen (Future)

After Long Rest, roll a die. Result determines feature:

| Roll | Omen | Effect |
|------|------|--------|
| Even | Weal | Reaction: Creature in 30 ft adds d6 to attack/save/check |
| Odd | Woe | Reaction: Creature in 30 ft subtracts d6 from attack/save/check |

Uses = Proficiency Bonus per Long Rest

### Level 10: Twinkling Constellations (Future)

- At start of each turn, can change to different Starry Form constellation
- Also: Archer = 2d8+WIS, Chalice = 2d8+WIS

---

## Feats

### Magic Initiate: Druid (from Guide Background)

**Cantrips (2):**
| Cantrip | Casting Time | Range | Effect |
|---------|--------------|-------|--------|
| Produce Flame | Action | Self | Create flame, throw as ranged attack (30 ft), 2d8 fire (level 5) |
| Mending | 1 Minute | Touch | Repair single break/tear in object |

**1st Level Spell (1):**
| Spell | Effect |
|-------|--------|
| Healing Word | Bonus Action, 60 ft, heal 1d4+WIS (can upcast) |

- Spell can be cast 1/Long Rest free OR with spell slots
- Always prepared (doesn't count against prepared limit)
- Uses Wisdom for spellcasting

> **CHOICE MADE**: Produce Flame, Mending, Healing Word

### War Caster (Level 4 ASI)

| Benefit | Description |
|---------|-------------|
| **Advantage on Concentration** | Advantage on CON saves to maintain Concentration |
| **Somatic Components** | Can perform somatic components while holding weapon/shield |
| **Opportunity Spell** | Can cast spell instead of opportunity attack (spell must target only that creature, 1 Action casting time) |

---

## Free Resources Summary

| Resource | Uses | Recharge | Source | Effect |
|----------|------|----------|--------|--------|
| Guiding Bolt | 4 | Long Rest | Star Map | 4d6 radiant, grants Advantage on next attack |
| Healing Word | 1 | Long Rest | Magic Initiate | 1d4+WIS healing, Bonus Action, 60 ft |
| Healing Hands | 1 | Long Rest | Aasimar | Touch, heal 1d4 x Prof Bonus (3d4) HP |
| Celestial Revelation | 1 | Long Rest | Aasimar (3+) | Transform 1 min (Wings/Radiance/Shroud) |
| Wild Shape | 2 | Short/Long Rest | Druid | Transform into beast or use for Starry Form/Wild Companion |

---

## Skill Proficiencies

| Skill | Ability | Proficient? | Modifier | Source |
|-------|---------|-------------|----------|--------|
| Acrobatics | DEX | No | +2 | |
| Animal Handling | WIS | No | +4 | |
| Arcana | INT | No | +3 | +4 from Magician (WIS mod) |
| Athletics | STR | No | -1 | |
| Deception | CHA | No | +1 | |
| History | INT | No | -1 | |
| Insight | WIS | No | +4 | |
| Intimidation | CHA | No | +1 | |
| Investigation | INT | No | -1 | |
| Medicine | WIS | No | +4 | |
| Nature | INT | **YES** | +6 | Druid class + Magician (+4 WIS) |
| Perception | WIS | **YES** | +7 | Druid class |
| Performance | CHA | No | +1 | |
| Persuasion | CHA | No | +1 | |
| Religion | INT | No | -1 | |
| Sleight of Hand | DEX | No | +2 | |
| Stealth | DEX | **YES** | +5 | Guide background |
| Survival | WIS | **YES** | +7 | Guide background |

> **SKILLS CONFIRMED**:
> - From Druid class: Nature, Perception
> - From Guide background: Stealth, Survival
> - Magician feature adds WIS mod (+4) to Arcana and Nature checks

---

## Senses

| Sense | Range | Description |
|-------|-------|-------------|
| Darkvision | 60 ft | See dim light as bright, darkness as dim (grayscale only) |
| Passive Perception | 14 | 10 + Perception modifier (+4) |
| Passive Investigation | 9 | 10 + Investigation modifier (-1) |
| Passive Insight | 14 | 10 + Insight modifier (+4) |

---

# PART 3: OFFICIAL STARTING EQUIPMENT

## Complete Starting Equipment List

### From Druid Class (Option A)
| Item | Type | Properties | Notes |
|------|------|------------|-------|
| Leather Armor | Light Armor | AC 11 + DEX | Proficient |
| Shield | Shield | +2 AC | Proficient (non-metal) |
| Sickle | Simple Melee | 1d4 slashing, Light | Proficient |
| Quarterstaff | Simple Melee / Focus | 1d6 bludgeoning (1d8 versatile) | Acts as Druidic Focus |
| Herbalism Kit | Tool | — | Proficient |
| Backpack | Adventuring Gear | Holds 30 lbs | — |
| Bedroll | Adventuring Gear | — | — |
| Mess Kit | Adventuring Gear | Tin utensils | — |
| Tinderbox | Adventuring Gear | Fire starting | — |
| Torches | Adventuring Gear | 10 total, consumable | 1 hour burn each |
| Rations | Adventuring Gear | 10 days, consumable | — |
| Waterskin | Adventuring Gear | 4 pints | — |
| Hempen Rope | Adventuring Gear | 50 ft, consumable | Can be cut |
| 9 GP | Currency | — | — |

### From Guide Background
| Item | Type | Notes |
|------|------|-------|
| Bedroll | Adventuring Gear | (Already from Explorer's Pack) |
| Tent (2-person) | Adventuring Gear | Shelter |
| Tinderbox | Adventuring Gear | (Already from Explorer's Pack) |
| Traveler's Clothes | Clothing | Outfit |
| Waterskin | Adventuring Gear | (Already from Explorer's Pack) |
| Hempen Rope (50 ft) | Adventuring Gear | (Already from Explorer's Pack) |
| Quiver | Container | Holds 20 arrows |
| Arrows | Ammunition | 20 arrows |
| Cartographer's Tools | Tool | Proficient |
| 3 GP | Currency | — |

### From Circle of Stars Subclass
| Item | Type | Notes |
|------|------|-------|
| Star Map | Druidic Focus | Grants Guidance cantrip, 4 free Guiding Bolts/day |

### Consolidated Equipment List
Removing duplicates from overlapping packs:

| Item | Qty | Type | Notes |
|------|-----|------|-------|
| Leather Armor | 1 | Light Armor | Equipped |
| Shield (Wooden) | 1 | Shield | Equipped |
| Sickle | 1 | Simple Weapon | 1d4 slashing, Light |
| Quarterstaff | 1 | Simple Weapon / Focus | 1d6 (1d8 versatile) bludgeoning |
| Star Map | 1 | Focus | Primary focus, grants Guidance + Guiding Bolt |
| Dagger | 1 | Simple Weapon | 1d4 piercing, Finesse, Thrown (20/60) |
| Shortbow | 1 | Simple Weapon | 1d6 piercing, Range 80/320 |
| Arrows | 20 | Ammunition | For shortbow |
| Quiver | 1 | Container | Holds arrows |
| Herbalism Kit | 1 | Tool | Proficient |
| Cartographer's Tools | 1 | Tool | Proficient |
| Backpack | 1 | Container | Holds 30 lbs |
| Bedroll | 1 | Gear | Camping |
| Tent (2-person) | 1 | Gear | Shelter |
| Mess Kit | 1 | Gear | Eating utensils |
| Tinderbox | 1 | Gear | Fire starting |
| Torches | 10 | Gear (Consumable) | 1 hour burn each |
| Rations | 10 | Gear (Consumable) | 1 day food each |
| Waterskin | 1 | Gear | Holds 4 pints |
| Hempen Rope | 50 ft | Gear (Consumable) | Can be cut |
| Traveler's Clothes | 1 | Clothing | Outfit |
| **Gold Pieces** | **12** | Currency | 9 (Druid) + 3 (Guide) |

> **NOTE**: Dagger and Shortbow are commonly added as they are simple weapons Druids are proficient with.

---

# PART 4: GEAR DESCRIPTIONS

## Tools

### Herbalism Kit
**Contents**: Pouches for herbs, clippers, mortar and pestle, glass jars, distilling equipment

**Uses**:
- Identify plants with Herbalism Kit check
- Create antitoxin, healing potions (with DM rules)
- Prepare herbal remedies
- Craft poultices and salves

**Related Checks**: Medicine, Nature, Survival

### Cartographer's Tools
**Contents**: Quill, ink, parchment, compass, calipers, ruler

**Uses**:
- Create accurate maps
- Determine your position on a map
- Estimate distance between locations
- Navigate unfamiliar terrain

**Related Checks**: Nature, Survival, Investigation

## Adventuring Gear

| Item | Description |
|------|-------------|
| **Backpack** | A backpack can hold one cubic foot or 30 pounds of gear. You can also strap items to the outside. |
| **Bedroll** | A sleeping bag for keeping warm and dry while camping outdoors. Roll it up and strap to backpack. |
| **Mess Kit** | A tin box containing a plate, cup, and eating utensils (fork, spoon, knife). The lid doubles as a pan. |
| **Tinderbox** | Contains flint, fire steel, and tinder. Using it to light a torch or start a campfire takes 1 minute. |
| **Torch** | Burns for 1 hour, providing bright light in a 20-foot radius and dim light for an additional 20 feet. Can be used as improvised weapon (1 fire damage). |
| **Rations (1 day)** | Dried, preserved food sufficient for one day. Consists of jerky, dried fruit, hardtack, and nuts. |
| **Waterskin** | A leather pouch that holds up to 4 pints of liquid. One pint of water per day prevents dehydration. |
| **Hempen Rope (50 ft)** | Has 2 HP and can be burst with DC 17 Strength check. Can be cut into smaller lengths. |
| **Tent (2-person)** | A canvas shelter that accommodates two Medium creatures. Takes 10 minutes to set up or break down. |
| **Traveler's Clothes** | A set of durable, practical clothes for traveling: boots, trousers, shirt, vest, belt, and cloak. |
| **Quiver** | A leather container that holds up to 20 arrows or bolts. |
| **Arrows (20)** | Ammunition for bows. |

---

# PART 5: SPELLS

## Cantrips Known

| Cantrip | Source | Casting Time | Range | Effect |
|---------|--------|--------------|-------|--------|
| Produce Flame | Magic Initiate | Action | Self/30 ft | Light, or throw for 2d8 fire damage |
| Mending | Magic Initiate | 1 Minute | Touch | Repair break/tear in object |
| Guidance | Star Map | Action | Touch | +1d4 to ability check, Concentration |
| Druidcraft | Druid | Action | 30 ft | Minor nature effects |
| Thorn Whip | Druid | Action | 30 ft | 2d6 piercing, pull 10 ft |
| Starry Wisp | Druid | Action | 60 ft | 2d8 radiant, reveal Invisible |
| Light | Light Bearer | Action | Touch | Object sheds bright light 20 ft |

> **CANTRIP CHOICES MADE**:
> - Magic Initiate: Produce Flame, Mending
> - Druid Class: Druidcraft, Thorn Whip, Starry Wisp (Magician grants extra)
> - Star Map: Guidance
> - Aasimar: Light

## Always Prepared Spells

| Spell | Level | Source | Free Uses |
|-------|-------|--------|-----------|
| Guiding Bolt | 1st | Star Map | 4/Long Rest |
| Healing Word | 1st | Magic Initiate | 1/Long Rest |

## Prepared Spells (Level 5: 9 slots)

Druids can change prepared spells after each Long Rest.

> **CURRENT PREPARED SPELLS**: (to be confirmed with player)

---

# PART 6: IMPLEMENTATION NOTES

## Proficiency Enforcement

### Weapon Attacks
```
IF weapon.category == 'martial' AND CLASS_PROFICIENCIES.weapons does NOT include 'martial':
  attackBonus = abilityMod (NO proficiency bonus)
  showWarning("Not proficient - no proficiency bonus to attack")
ELSE:
  attackBonus = abilityMod + proficiencyBonus
```

### Armor/Shield Equipping
```
IF armor.type == 'medium' OR armor.type == 'heavy':
  IF CLASS_PROFICIENCIES.armor does NOT include armor.type:
    showWarning("Not proficient - disadvantage on STR/DEX, CANNOT cast spells")
    DISABLE all spell casting buttons
    SET canCastSpells = false
```

### Wild Shape
```
IF inWildShape AND wildShapeType == 'beast':
  DISABLE all spell casting buttons
  SET canCastSpells = false

IF inStarryForm:
  KEEP spell casting ENABLED
```

## Inventory Corrections (All Fixed in Session 8)

| Issue | Status |
|-------|--------|
| Scimitar → Sickle | ✓ Fixed |
| Hide Armor → Leather Armor | ✓ Fixed |
| Add Quarterstaff | ✓ Fixed |
| Add Herbalism Kit | ✓ Fixed |
| Add Mess Kit | ✓ Fixed |
| Gear descriptions | ✓ Fixed |

---

# PART 7: CHANGE LOG

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

### Session 3
- Multiple Companions support (Familiar AND Summon Beast)
- Cantrip Damage updated to 2 dice for level 5
- Always Prepared Spells shown correctly
- Wild Companion moved to middle of action bar
- Wild Shape spell disable fixes

### Session 4 - Inventory System
- Complete Equipment System with slots
- Add Equipment forms (weapon, armor, shield, accessory)
- Magic item effects (Phase 1 & 2)
- Attunement tracking

### Session 5 - Magic Items & Corrections
- Charge-based items (wands, staffs)
- Spells from charges
- Wild Shape skills fix
- Stealth proficiency correction

### Session 6 - Collapsible UI & Consumables
- All cards collapsible with state saved
- Ammunition auto-decrement
- Thrown weapons system
- Adventuring gear improvements
- Custom spell details for magic items

### Session 7 - Tools & Proficiency
- Clickable tools with proficiency info
- Reclaim button for thrown weapons
- Weapon categories (Simple/Martial)
- Improved custom spell editor
- Added proficiency warnings

### Session 8 - Rules Reference & Corrections (Current)
- Created comprehensive D&D 2024 rules reference
- Document proficiency enforcement rules
- Identified inventory corrections needed
- Added official starting equipment

---

# PART 8: QUESTIONS/CONFIRMATIONS NEEDED

1. ~~**Druid Skill Proficiencies**~~ → **ANSWERED**: Nature + Perception

2. **Currently Prepared Spells**: What 9 spells are currently prepared?

3. **Shortbow/Dagger**: Did you add these separately, or should they not be in inventory?
   - Official Druid starting equipment doesn't include ranged weapons
   - (Keeping them as common simple weapon additions)

4. **Tiefling Traits**: What specific Infernal Legacy features (if any) from the Tiefling half?
