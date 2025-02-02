## Release/Patch Notes

### Version 0.9.9 - 2021-03-27

  * Fix - [GitHub #23] - Localization mistake, had two spaces in between "Critical" and "Success" or "Failure" in chat cards.
  * Fix - [GitHub #24] - The chat card that was generated from rolling a skill check by clicking on a weapon (e.g. Firearms for a pistol) was not being localized. Fixed this along with a related tooltip that wasn't being localized either.
  * Fix - [GitHub #25] - The chat card for damage and lethality was not bolding those terms like it would for other skill or percentile rolls.
  * Fix - [GitHub #26] - When clicking on the 'Roll Luck' button in the character sheet header, the resulting chat card was not being localized properly.
  * Fix - [GitHub #27] - Using a language setting that did not have a full translation was breaking adding skills to the agent's actor sheet. Should not break quite so quickly now, but will likely need a better long term fix at some point.
  * Fix - [GitHub #28] - Missing localization keys for break point tooltips added.
  * Fix - Made Agent sheet default width a little wider so skills with longer names aren't getting clipped off.  Also a few other alignment fixes in the CSS.

  * Enhancement - [GitHub #28] - Spanish language translation, many thanks to CthulhuRol for providing it!
  * Enhancement - Added a macro that allows for rolling the skill check on a weapon, so there can be macro buttons for both the damage and the skill check if desired.
    * Sample syntax: game.deltagreen.rollItemSkillCheckMacro("Combat Dagger");
  * Enhancement - Thanks to *Uriele* - Added functionality from the Handler's Guide (page 188) for 'Inhuman' stat tests, test where the stat (e.g. CON) is 20 or higher, giving a x5 target of 100 or higher.  In this event, the test auto succeeds on a roll of anything other than 100, and a roll lower than the stat value is a critical (along with regular critical logic).
  * Enhancement - Added 'Ritual' skill, which is calculated and is equal to 99 - current sanity (thanks to *Uriele* for mentioning it).  See page 166 under 'Ritual Activation' for the full rules.
  * Enhancement - Total protection rating of all _equipped_ armor now displayed by HP.

  * Font and Background Change and Configuration Options - *NOTE THIS CAN BE CHANGED IN THE SYSTEM SETTINGS BACK TO WHAT IT WAS!*
    * Enhancement - Added system setting for font choice, with a few options.  For example you can set a world to use typewriter style font for an older feel.
    * Enhancement - Added system setting for background image choice, with a few options.  Changed default from normal Foundry parchment to a lighter, more moder looking paper.  Also included option for old, used/crinkled paper for a more unsettling or hard-used look. 

### Version 0.9.7
* Enhancement - Can now click on the icon for armor/other gear to equip or unequip it.
* Enhancement - Changed so that players with the 'Limited' permission on an actor now only see the C.V. tab of the actor's character sheet, instead of the entire sheet.  Previously the 'Limited' permission and the 'Observer' permission gave the same result.  The 'Observer' permission is unchanged and still shows a read-only view of the entire sheet.
* Enhancement - Added ability to alter formula for damage rolls by either __right clicking__ *or* __holding shift and left clicking__.
* Enhancement - Added ability to alter targets for tests by either __right clicking__ *or* __holding shift and left clicking__.  Applies to the following rolls:
  * Skill tests 
  * Attribute tests 
  * Lethality tests
* Improved CSS on actor sheet in a few places.
  *  New Font (was previously in style sheet, but not properly applied).
  *  Nav bar alignment/border consistent across tabs for a cleaner look moving between sections.
  *  Gear sheet alignment cleaner with certain fields now being centered.
  *  CV sheet now has some padding on fields so things aren't so cramped looking.
* Fix - Thanks to @Hrunh for submitting update to localization in item sheet
* Fix - typo in Alertness skill (English locale), thanks to roestrei for report

### Version 0.9.6
* Incremented Core Compatible Version after testing against release version of Foundry 0.7.5.
* Made the gear section a little less ugly by adding some nicer section dividers.
* Fixed some awkward tooltip wording.

### Version 0.9.4
* Fix - Pharmacy and Surgery skills were missing.
* Fix - Accounting and Disguise base skill rating were 0%, should be 10%.
* Fix - Damage on medium pistol in compendium was wrong, also fixed some base range values that were off.
* Enhancement - Adding support for localization.  Character sheet and items sheets (gear, bonds, etc.) should be localized now, but not the compendium packs.
* Workaround - The (current alpha) 7.2 Foundry release seems to have a bug where rolls without a leading number ('d100') do not work, so updated all skill checks to roll '1d100' instead to avoid the issue.
* Enhancement - Added support for Dice So Nice module, since moving to custom chat message broke out of the box compatibility with it.

### Version 0.9.3
We will never speak of 0.9.1 or 0.9.2 ever again.

### Version 0.9.1
Added a few compendium packs with some common armor and weapon choices for Agents to equip themselves with.  

Note that weapon/armor statistics are not covered by the Open Game License like the other rules used in the system, they are included as an exception with permission from Arc Dream publishing.

### Version 0.9.0
Basic system functionality complete and submitted to Foundry VTT as an official system.