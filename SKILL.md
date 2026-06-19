---
name: reusable-bag-collection-organizer
displayName: Reusable Bag Door-Station Organizer
description: Create a printable reusable bag collection map and weekly reset card that sorts existing bags by size, assigns safe door stations, and builds simple grab-and-return rules without requiring purchases.
version: 1.1.0
license: MIT-0
language: en
tags: [sustainability, inventory-management, habit-tracking, eco-friendly]
---

# Reusable Bag Door-Station Organizer

## Purpose

Use this prompt-only skill when a user wants to turn a messy collection of reusable shopping bags, totes, insulated bags, produce bags, or folding bags into a small household system. The deliverable is a printable bag-zone map plus a weekly reset card.

This skill uses the bags and storage spots the user already has. It does not require buying organizers, installing hardware, or storing items where they block movement.

## Safety Boundary

Keep all storage out of unsafe walk paths. Do not recommend placing bags on stairs, landings, tight hallways, door swing areas, emergency exits, heater vents, cooktops, appliance controls, wet floors, or anywhere that creates a trip, fire, access, or visibility hazard.

Do not require purchases. If the user asks about products, redirect to no-purchase options first: folding, grouping, labeling, using an existing bin, using an existing shelf, or moving bags to a safer current location.

Do not give structural installation advice. If a hook, shelf, or rack seems loose, overloaded, or uncertain, mark it as not approved for bag storage and choose a different location.

## Use This Skill When

Use this skill when the user wants to:

- Stop reusable bags from piling up in closets, cars, kitchens, or entryways.
- Know which bags to grab before grocery trips, errands, school runs, work commutes, returns, or library visits.
- Separate large totes, compact bags, insulated bags, produce bags, and damaged bags.
- Create a visible door station without making the home less safe or more cluttered.
- Build a weekly reset so bags return to their stations after use.

Do not use this skill for emergency go-bags, evacuation kits, hazardous material storage, structural mounting plans, or product shopping lists.

## Best Inputs

Ask only for the details needed to build the organizer:

- Bag types and approximate counts: large totes, small totes, insulated bags, produce bags, folding bags, damaged bags, or unknown bags.
- Current storage locations and where bags usually pile up.
- Common exits or transition points: front door, mudroom, garage shelf, car trunk, stroller area, work bag area, or kitchen command spot.
- Weekly routines: grocery day, school days, work commute, farmers market, returns, library, gym, or pet errands.
- Safety constraints: narrow halls, stairs, mobility aids, children, pets, renters, door clearance, or shared entryways.
- Preference for a one-zone, two-zone, car-plus-door, or person-specific system.

If the user does not know counts, give them a five-minute gather-and-sort step before creating the map.

## Workflow

1. **Gather bags.** Ask the user to collect reusable bags from closets, counters, vehicles, hooks, laundry areas, and kitchen corners.
2. **Sort by function.** Group bags into large totes, compact totes, insulated bags, produce bags, foldable bags, return bags, and damaged or questionable bags.
3. **Reduce excess.** Keep a practical working set and move overflow to a secondary storage spot. Do not tell the user to buy anything.
4. **Screen locations for safety.** Reject any location that blocks walking, doors, stairs, exits, appliance access, heat sources, or visibility.
5. **Assign stations.** Map each bag type to a safe station such as an existing shelf, bin, hook, drawer, car trunk spot, or bag-in-bag bundle.
6. **Create grab rules.** Write simple rules for common trips, such as "grocery trip: two large totes plus one insulated bag" or "quick errand: one folding bag in work bag."
7. **Create return rules.** Add a reset action for after unloading: empty, check for receipts or food, fold, and return to the assigned station.
8. **Build the printable card.** Produce a bag-zone map and weekly reset card that can be posted near the station.

## Output Format

Return the result in this order:

1. **Bag-Zone Map**
   - Station name
   - Safe location
   - Bag types stored there
   - Maximum count
   - Why this location works
   - Safety notes

2. **Keep, Move, Repair, Retire**
   - Keep in daily use
   - Move to overflow
   - Wash or repair before use
   - Retire, recycle, or donate if appropriate and safe

3. **Grab Rules**
   - Grocery trip
   - Quick errand
   - Cold items or insulated trip
   - Returns or library trip
   - Work, school, stroller, or car option if relevant

4. **Return Rules**
   - Empty the bag
   - Remove receipts, crumbs, or loose items
   - Air out damp bags before storing
   - Fold or nest bags by type
   - Return each bag to its mapped station

5. **Weekly Reset Card**
   - Count bags at each station
   - Bring stray bags back from car, kitchen, work bag, or closet
   - Check insulated bags for forgotten items
   - Remove damaged bags from the active set
   - Confirm no bags are blocking walk paths, doors, stairs, or exits

6. **Printable Mini Card**
   - A compact version with station names, grab rules, and reset day.

## Style Guidelines

- Keep the plan practical, visible, and low-effort.
- Prefer existing storage and simple folding over buying new products.
- Use clear count limits so the station does not become another pile.
- Make unsafe locations visibly rejected rather than silently ignored.
- Use household-friendly language and avoid shaming clutter.

## Example Prompts

Copy and paste one of these into your AI assistant with your details filled in:

1. **Too many bags everywhere:** "My reusable grocery bags are piling up in the kitchen, car trunk, and front closet. I have about 10 large totes, 5 insulated bags, 8 produce bags, and some that are ripped. I do groceries on Saturdays, farmers market on Sundays, and quick errands midweek. Create a door-station organizer using what I already have."

2. **Small apartment entryway:** "I live in an apartment with a narrow entryway. My reusable bags keep ending up on the floor by the door. I have a small shelf and a coat hook already. I use 2-3 bags for weekly groceries and 1 insulated bag for frozen items. Can you design a station that doesn't block the door or hallway?"

3. **Family car-and-door system:** "We're a family of four and bags accumulate in both cars and the mudroom. We need a simple grab-and-return routine. I want one station by the garage door for big totes and one small bag in each car for quick stops. Also need a weekly reset so bags don't stay in cars forever."


## Usage Scenarios

### Scenario 1

**User Input:** "Add 3 cotton tote bags and 2 insulated bags. I use the cotton ones for grocery runs every Saturday."

**Expected Output:** Confirmation of 5 bags added. Generates a weekly usage schedule: cotton totes auto-assigned to Saturday grocery runs; insulated bags tagged for cold-item trips.

### Scenario 2

**User Input:** "Which bags have been unused for over a month? Do any need washing?"

**Expected Output:** Report listing idle bags (>30 days unused) and those exceeding cleaning-threshold cycles. Suggests rotation order to even out wear.

### Scenario 3

**User Input:** "Log that I lent my foldable nylon bag to a friend on 6/15. Remind me in 2 weeks to check if it's returned."

**Expected Output:** Record created with lent status, borrower note, and a reminder scheduled for 6/29. Bag is excluded from rotation until returned.


### Scenario 4: 家里囤了30个帆布袋怎么办
**User input:** "每次买奶茶/书店/品牌活动就送帆布袋，现在家里堆了三四十个。扔了可惜，留着占地方。怎么系统处理？"
**Expected output:** 帆布袋整理方案——第一步：分类淘汰（留5个最好看的+5个质量最好的实用型，其余全部洗干净叠好）；第二步：利用渠道（闲鱼打包卖"福袋"10元5个不挑款、公司团建捐给社区当环保袋、剪刀裁开做收纳分隔板）；第三步：日常循环（所有帆布袋集中放在玄关一个收纳盒里，每次出门随机拿一个用完放回，谁拿谁洗）；第四步：源头控制（买奶茶时主动说不要袋子存手机备忘录减一次、自带无纺布折叠袋）。关键：超过15个就是负担，保持5-10个的合理库存。

## Quality Bar

A strong result lets the user gather bags, sort them, assign safe stations, and print a reset card in under 20 minutes. It should reduce clutter without requiring purchases or creating trip, access, door, or exit hazards.
