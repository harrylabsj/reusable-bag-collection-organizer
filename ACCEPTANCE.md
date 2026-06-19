# Acceptance Tests - Reusable Bag Door-Station Organizer

## Overview
- **Skill:** Reusable Bag Door-Station Organizer
- **Slug:** reusable-bag-collection-organizer
- **Version:** 1.0.0
- **Project:** daily-50-skills-2026-05-08
- **Total Tests:** 10

## AT-1: No-Purchase Boundary
- **Check:** The skill states that no purchases are required.
- **Expected:** It prioritizes existing bags, existing bins, shelves, drawers, hooks, or bag-in-bag bundles.
- **Pass:** The workflow does not depend on buying products or organizers.

## AT-2: Walk-Path Safety
- **Check:** The skill rejects unsafe storage locations.
- **Expected:** It avoids stairs, landings, tight hallways, door swing areas, exits, heater vents, cooktops, appliance controls, and wet floors.
- **Pass:** Bag storage is kept out of unsafe walk paths and access zones.

## AT-3: Gather And Sort Workflow
- **Check:** The workflow gathers bags and sorts them by type and purpose.
- **Expected:** Large totes, compact totes, insulated bags, produce bags, foldable bags, and damaged bags can be separated.
- **Pass:** The user can inventory the collection before assigning stations.

## AT-4: Station Assignment
- **Check:** The output includes a bag-zone map.
- **Expected:** Each station has a safe location, bag types, maximum count, reason, and safety notes.
- **Pass:** The plan creates visible and bounded storage stations.

## AT-5: Grab Rules
- **Check:** The output includes trip-based grab rules.
- **Expected:** Rules cover grocery trips, quick errands, insulated trips, returns, or other user routines.
- **Pass:** The user knows which bags to take before leaving.

## AT-6: Return Rules
- **Check:** The output includes after-use return rules.
- **Expected:** It covers emptying, checking, drying if damp, folding, and returning bags.
- **Pass:** Bags have a clear way back into the system.

## AT-7: Weekly Reset Card
- **Check:** The output includes a weekly reset card.
- **Expected:** It includes counts, stray-bag retrieval, insulated bag checks, damaged bag removal, and a safety check.
- **Pass:** The card is printable and useful for routine maintenance.

## AT-8: Household Scope
- **Check:** The skill stays within household organizing.
- **Expected:** It does not become an emergency kit, evacuation kit, hazardous storage guide, structural mounting plan, or shopping list.
- **Pass:** Scope remains a simple clutter and routine artifact.

## AT-9: Document Language
- **Input:** Any valid trigger.
- **Expected:** Output is English-only with no CJK text.
- **Pass:** Main output is in English.

## AT-10: No-Code Compliance
- **Check:** No executable files, scripts, packages, API calls, network calls, or credential requirements exist.
- **Expected:** `skill.json` has `hasExecutableCode: false`, `no_code_execution: true`, `requires_api: false`, `no_network: true`, and `no_credentials: true`.
- **Pass:** Skill is document-only and prompt-flow only.

## Install-First Success Path

- **Input:** User says "My reusable grocery bags are piling up in the kitchen, car trunk, and front closet. I have about 10 large totes, 5 insulated bags, 8 produce bags, and some that are ripped. I do groceries on Saturdays, farmers market on Sundays, and quick errands midweek. Create a door-station organizer using what I already have."
- **Steps:** Skill asks user to gather all bags from closets, counters, vehicles, hooks → sorts by function (large totes, compact totes, insulated bags, produce bags, foldable bags, damaged bags) → reduces excess to a practical working set → screens locations for walk-path, door, stair, and exit safety → assigns stations (existing shelf, bin, hook, car trunk spot, or bag-in-bag bundle) → creates trip-based grab rules (grocery: 2 large totes + 1 insulated bag; quick errand: 1 folding bag) → creates return rules (empty, check for receipts, air out, fold, return to station) → builds a printable bag-zone map and weekly reset card.
- **Output:** A reusable bag door-station organizer with sorted bag inventory, safe station assignments, grab rules for common trips, return rules, printable bag-zone map, and weekly reset card — all using existing storage without requiring purchases.

## Clean Scan Evidence

- **Executable code:** None (prompt-only, noExec)
- **API calls:** None required
- **Network access:** No (document-only)
- **Credentials:** None stored or requested
- **Secrets or .env:** None
- **Logs or temp files:** None
- **Package files or scripts:** None
- **Safety scan:** Clean — keeps all storage out of unsafe walk paths, stairs, door swing areas, exits, heater vents, cooktops; does not require purchases or structural installation; marks unsafe hooks/shelves as not approved; stays within household organizing scope (no emergency kits, hazardous storage, or product shopping).
