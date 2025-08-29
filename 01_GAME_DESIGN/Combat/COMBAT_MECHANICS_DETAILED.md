# ⚔️ DETAILED COMBAT MECHANICS & EXAMPLES

## 🎯 COMBAT PHILOSOPHY

Our combat system combines **tactical depth** with **visceral action**, where player skill matters as much as character stats. Every class feels unique through distinct resource mechanics, not just different colored spells.

---

## 🎮 CORE COMBAT FLOW

### Basic Combat Loop (All Classes)

```
1. POSITIONING → 2. RESOURCE GENERATION → 3. ABILITY EXECUTION → 4. REACTION/ADAPTATION
     ↑                                                                        ↓
     ←────────────────────────── 5. RESET ←─────────────────────────────────
```

### Time-To-Kill (TTK) Targets
- **PvE Standard Mob**: 8-15 seconds
- **PvE Elite**: 30-60 seconds  
- **PvP 1v1**: 15-30 seconds
- **PvP Group Fight**: 5-10 seconds (focused target)

---

## 🔥 COMBAT EXAMPLE: KORGARI SEIGNEUR DE GUERRE

### Resource: Adrénaline (0-100)
- **Generates**: +5 per basic attack, +10 when hit
- **Decays**: -2 per second out of combat
- **Threshold Bonuses**:
  - 25+: +10% attack speed
  - 50+: +15% damage
  - 75+: Lifesteal 20%
  - 100: Unlock "Brasier Incarné" ultimate

### Ability Rotation Example

#### Opening Sequence (0 Adrénaline)
```
1. [Charge Volcanique] → Gap closer, +15 Adrénaline
2. [Frappe Cendrée] → Basic attack x3, +15 Adrénaline (total: 30)
3. [Cri de Guerre] → AoE taunt, +10 Adrénaline (total: 40)
4. [Chaîne de Lave] → Pull enemy, costs 20 Adrénaline (total: 20)
```

#### Mid-Combat (Building Phase)
```
5-8. [Frappe Cendrée] x4 → +20 Adrénaline (total: 40)
9. [Éruption] → AoE damage, costs 30 Adrénaline (total: 10)
10. Take damage from boss → +30 Adrénaline (total: 40)
```

#### Burst Window (High Adrénaline)
```
11-14. [Frappe Cendrée] x4 → +20 Adrénaline (total: 60)
15. [Rage Sismique] → Damage buff, maintains Adrénaline
16-18. [Frappe Cendrée] x3 → +15 Adrénaline (total: 75)
19. [Déferlement] → 3-hit combo, costs 50 Adrénaline
```

#### Ultimate Execution (100 Adrénaline)
```
20. Build to 100 Adrénaline
21. [BRASIER INCARNÉ] → Transform into lava elemental for 15s
    - All abilities enhanced
    - Constant AoE burn aura
    - 50% damage reduction
    - Resets to 0 after transformation
```

### Visual/Audio Feedback
- **Screen Effect**: Red vignette intensifies with Adrénaline
- **Character**: Glowing veins appear at 50+, full fire aura at 75+
- **Sound**: Heartbeat intensifies, volcanic rumbling at high levels
- **Controller**: Vibration pulses match heartbeat (console)

---

## 🩸 COMBAT EXAMPLE: BLOOD MAGE

### Resource: Blood Charges (0-3)
- **Generation**: Specific abilities grant charges
- **Consumption**: Empowered abilities consume all charges
- **Visual**: Floating blood orbs orbit character

### Ability Rotation Example

#### Setup Phase (0 Charges)
```
1. [Lacération] → Damage + Bleed, grants 1 Blood Charge
2. [Drain Vital] → Channel 2s, grants 1 Blood Charge (total: 2)
3. [Pacte Sanglant] → Sacrifice 20% HP, grants 1 Blood Charge (total: 3)
```

#### Burst Execution (3 Charges)
```
4. [NOVA ÉCARLATE] → Consumes all 3 charges
   - 1 charge: 400 damage
   - 2 charges: 900 damage + slow
   - 3 charges: 1500 damage + fear + heal allies
```

#### Recovery Loop
```
5. [Transfusion] → Heal self using enemy's blood
6. [Marque Sanguine] → Mark target for bonus damage
7. Begin new charge generation cycle
```

### Talent Modifications
- **"Sang Épais"**: 4 maximum charges instead of 3
- **"Hémophilie"**: Charges decay over 30s, but grant 5% lifesteal each
- **"Sang Maudit"**: Charges spread to nearby enemies on consumption

---

## 🎵 COMBAT EXAMPLE: PRODIGE (Musical Combat)

### Resource: Énergie (0-100%, regenerates steadily)
- **Regen Rate**: 10% per second baseline
- **Combo System**: Chaining abilities in rhythm grants bonus effects

### Musical Combat Flow

#### Opening Melody (100% Énergie)
```
1. [Prélude] → Buff allies' attack speed (20% Énergie)
   ♪ ♫ Sets 120 BPM rhythm
2. [Staccato] → Quick damage burst (15% Énergie)
   - Hit ON BEAT: 2x damage
   - Hit OFF BEAT: Normal damage
3. [Crescendo] → Building damage over 3s (25% Énergie)
   - Must maintain rhythm for full effect
```

#### Chorus Phase (40% Énergie remaining)
```
4. Wait 2 beats for regen → 60% Énergie
5. [Harmonique] → Group heal if 2+ allies nearby (30% Énergie)
6. [Dissonance] → AoE interrupt (20% Énergie)
```

#### Finale (Building to Ultimate)
```
7. [Mélodie Continue] → Passive regen boost for 5s
8. Regen to 100% Énergie
9. [SYMPHONIE DÉVASTATRICE] → 5-second channel
   - Creates expanding rings of damage
   - Allies inside gain massive buffs
   - Enemies are slowed and damaged
   - MUST maintain rhythm or symphony breaks
```

### Rhythm Gameplay Mechanics
- **Beat Indicator**: UI pulses with the rhythm
- **Perfect Timing**: Abilities flash gold when ready
- **Combo Counter**: Displays current chain (breaks if off-beat)
- **Audio Layers**: Music builds with successful combos

---

## ⚙️ COMBAT EXAMPLE: ZETHIR MAÎTRE DES RUNES

### Resource: Runes (5 types, 3 slots)
- **Fire Rune**: Direct damage
- **Water Rune**: Slows/Freezes
- **Earth Rune**: Shields/Armor
- **Lightning Rune**: Chain damage
- **Void Rune**: Debuffs

### Rune Combination Examples

#### Defensive Combo: Earth-Earth-Water
```
1. [Inscription: Terre] → First rune slot
2. [Inscription: Terre] → Second rune slot  
3. [Inscription: Eau] → Third rune slot
4. [ACTIVATION] → "Forteresse Gelée"
   - Creates ice wall that blocks projectiles
   - Slows enemies passing through
   - Grants 500 shield to allies behind it
```

#### Offensive Combo: Fire-Lightning-Fire
```
1. [Inscription: Feu] → First rune slot
2. [Inscription: Foudre] → Second rune slot
3. [Inscription: Feu] → Third rune slot
4. [ACTIVATION] → "Tempête Incendiaire"
   - Lightning strikes spread fire
   - Each strike creates burning ground
   - Chain reaction between burning enemies
```

#### Utility Combo: Void-Earth-Lightning
```
1. [Inscription: Vide] → First rune slot
2. [Inscription: Terre] → Second rune slot
3. [Inscription: Foudre] → Third rune slot
4. [ACTIVATION] → "Prison Dimensionnelle"
   - Creates gravity well
   - Pulls enemies to center
   - Lightning cage prevents escape
```

### Advanced Mechanics
- **Overcharge**: Using same rune 3x causes explosion but 10s cooldown
- **Quick Cast**: Pre-set combinations for instant activation
- **Rune Echo**: 20% chance to not consume a rune on activation

---

## 🌿 COMBAT EXAMPLE: SYLVANI SYLVESTRE

### Environmental Interaction Combat

#### Forest Zone Abilities
```
1. [Racines Anciennes] → Roots emerge from ground
   - In forest: 3 second root
   - In plains: 1.5 second root
   - In desert: 0.5 second slow
   
2. [Appel de la Meute] → Summon beasts
   - Forest: 3 wolves for 30s
   - Mountain: 2 bears for 20s
   - Swamp: 5 insects swarm for 15s
```

#### Seasonal Modifications (if Winter)
```
- [Floraison] becomes [Épines de Givre]: Damage + slow
- [Régénération Naturelle] → 50% less effective
- [Communion] → Summons ice elementals instead
```

#### Weather Synergy (if Raining)
```
- All nature spells: +20% growth speed
- Healing abilities: +30% effectiveness
- New ability available: [Déluge Verdoyant]
```

---

## 🎯 UNIVERSAL COMBAT MECHANICS

### Dodge System
- **Invincibility Frames**: 0.3 seconds
- **Stamina Cost**: 25% of max
- **Cooldown**: 1 second
- **Distance**: 3 meters (4.5 for Caelir race)

### Interrupt System
```
Cast Types:
- Instant: Non-interruptible
- Fast (0.5-1s): Interrupt stuns for 0.5s
- Normal (1-2s): Interrupt stuns for 1s
- Long (2s+): Interrupt stuns for 2s
```

### Combo System
- **Light Attack**: Fast, low damage, generates resource
- **Heavy Attack**: Slow, high damage, costs resource
- **Ability Weaving**: Can cast instant abilities between attacks
- **Animation Canceling**: Dodge/block cancels attack recovery

### Crowd Control Diminishing Returns
```
1st CC: 100% duration
2nd CC (within 15s): 75% duration
3rd CC: 50% duration
4th CC: 25% duration
5th+ CC: Immune for 10s
```

---

## 📊 DAMAGE CALCULATION

### Basic Formula
```
Final Damage = (Base Damage × Stat Modifier × Level Modifier) 
               × (1 - Armor Reduction) × (1 - Resistance) 
               × Critical Multiplier × Elemental Bonus
```

### Example Calculation
```
Korgari Seigneur de Guerre - [Frappe Cendrée]
Base Damage: 100
Strength Modifier: 1.5 (50 Strength)
Level Modifier: 1.2 (Level 20)
Enemy Armor: 20% reduction
Fire Resistance: 10% reduction
Critical Hit: 2.0x
Vs Nature Enemy: 1.15x (Korgari racial)

Final = 100 × 1.5 × 1.2 × 0.8 × 0.9 × 2.0 × 1.15 = 298 damage
```

---

## 🏹 RANGE AND POSITIONING

### Attack Ranges
- **Melee**: 2-3 meters
- **Extended Melee** (spears): 4-5 meters
- **Short Range** (shotgun): 8-10 meters
- **Medium Range** (most spells): 20-25 meters
- **Long Range** (bows, rifles): 30-40 meters
- **Extreme Range** (artillery): 50+ meters

### Line of Sight
- **Hard Cover**: Blocks all attacks
- **Soft Cover**: 50% miss chance
- **Elevation Advantage**: +10% damage, +5m range
- **Fog of War**: Can't target beyond 60m

---

## 💀 DEATH AND REVIVAL

### Death Mechanics
1. **Downed State** (PvP only): 15 seconds to revive
   - Can crawl slowly
   - One defensive ability available
   - Allies can revive in 3 seconds
   
2. **Death**: Return to nearest graveyard
   - **Resurrection Sickness**: -25% stats for 2 minutes
   - **Soul Walk**: Ghost form to retrieve body
   - **Durability Loss**: 10% on armor

### Combat Resurrection
- **Battle Res**: Some classes can resurrect in combat
- **30 second cast**: Interruptible
- **Cooldown**: 10 minutes
- **Target returns**: 50% HP/Mana

---

## 🎮 SKILL EXPRESSION EXAMPLES

### Animation Canceling Combo (Maître d'Armes)
```
Frame Data:
[Heavy Strike] → 30 frames (1.0s)
- Damage frames: 15-20
- Recovery frames: 21-30 (cancelable)

Optimal Combo:
1. [Heavy Strike] → Cancel at frame 21 with →
2. [Dash Strike] → Cancel at frame 18 with →
3. [Whirlwind] → Full animation
Total: 1.8s for 3 abilities instead of 3.0s
```

### Predictive Casting (Tisseur de Destin)
```
Temporal Mechanics:
1. [Premonition] → See enemy's next ability (3s preview)
2. Pre-cast [Temporal Shield] where attack will land
3. Enemy uses [Charge] as predicted
4. Shield automatically activates, perfect counter
5. [Rewind] to reset enemy position
```

---

## 🏆 HIGH-LEVEL PLAY EXAMPLES

### World First Raid Clear Rotation (Blood Mage)
```
Phase 1 (100-75% Boss HP):
0:00 [Pacte] → [Drain] → [Lacération] → Build 3 charges
0:08 [Nova Écarlate] → 1500 damage burst
0:10 [Marque] → Begin charge rebuild
[Repeat cycle, weaving defensive CDs]

Phase 2 (75-50% Boss HP):
Save charges for add phase
[Nova] precisely when adds spawn for cleave

Phase 3 (50-25% Boss HP):
Coordinate with raid for burn phase
Stack [Marque] with other debuffs
[Nova] during 10% damage taken window

Phase 4 (25-0% Boss HP):
[Sacrifice] healers' HP for emergency charges
Perfect [Nova] timing or raid wipes
```

### Top 100 PvP Arena Tactics (Prodige)
```
2v2 Arena vs Chimère/Ingénieur:

Opening:
- Start [Prélude] before gates open
- [Dissonance] to interrupt Ingénieur turret
- [Staccato] burst on Chimère before mutations

Kiting Phase:
- Maintain max range (25m)
- [Harmonique] partner when focused
- Save [Crescendo] for kill windows

Execution:
- Bait Chimère defensive
- [SYMPHONIE] when both enemies grouped
- Partner follows up with burst
- Match won in 47 seconds
```

---

## 📈 COMBAT METRICS & TELEMETRY

### Key Performance Indicators
- **APM** (Actions Per Minute): 40-80 optimal
- **Resource Efficiency**: 85%+ usage before capping
- **Combo Success Rate**: 70%+ for Prodige class
- **Interrupt Timing**: <0.5s reaction for competitive
- **Positioning Score**: Time in optimal range
- **Damage Uptime**: 75%+ for DPS roles

### Skill Rating Calculation
```
Combat Rating = (Damage Done / Damage Taken) 
                × Objective Score × Survival Time 
                × Mechanical Execution Score
```

---

## 🛡️ DEFENSIVE MECHANICS

### Active Mitigation
- **Block**: 50% damage reduction, costs stamina
- **Parry**: 100% physical negation, 0.5s window
- **Absorb**: Magic shield with HP value
- **Evasion**: 50% dodge chance for 2s

### Passive Defenses
- **Armor**: Reduces physical damage (up to 75% cap)
- **Resistance**: Reduces magic damage per element
- **Tenacity**: Reduces CC duration
- **Fortitude**: Chance to ignore interrupts

---

## 🎯 COMBAT ACCESSIBILITY OPTIONS

### Difficulty Modifiers
- **Auto-Aim Assist**: Slight magnetism for abilities
- **Extended Timing Windows**: +0.2s for combos
- **Visual Indicators**: Enhanced telegraphs
- **Colorblind Modes**: Full element color customization
- **One-Button Combos**: Simplified rotations option

### Information Display
- **Floating Combat Text**: Fully customizable
- **Damage Meters**: Built-in DPS/HPS tracking
- **Buff/Debuff Timers**: Large icon option
- **Resource Warnings**: Audio/visual alerts
- **Ability Cooldown Sweeps**: Clock-style or numeric

---

*This document represents our vision for engaging, skill-based combat that remains accessible while rewarding mastery.*