Role playing server

The idea here is to have a helper for role play. Instead of using a ad-hoc
setup with Slack or IRC or whatever, provide just the needed features and
abstain from adding extraneous features.

# Wanted features

## DM features

Display media
Have private chats with players
Enable character sheets and edit them
Load a campaign

## General features

Chat together
Maintain stats / character sheets
Roll any kind of dices
Keep logs

# Inventory

## Concepts

* Campaign, a given installment of a game. Dungeon Masters can create
campaigns and invite players to join them.
* Campaign Templates are presets for campaigns, allowing to quickly spawn a Campaign.
* Character sheets, holding stats (stats types depend on the ruleset and may vary
  considerably from game to game). Owned by a Player. The Player can see their character sheet. The
  DM can edit it. The Player can edit some of its fields.  
* Character sheet templates define what a Character sheet contains. They consist in a list of fields
with name, permissions, visibility.


## Actors

* Administrator, able to see and delete any object on the Server.
* DungeonMaster (DM), in charge of the animation of a game
* Players

## Actions

* Roll Dices. Several dice rolls are possible. They are pre-configured by campaign.
* Role-play. Chat between players.
* Perform Narration. DM chat window, that has more options for presentation.

# Stories

## Create a Campaign

DungeonMaster connects to the server and wants to start a campaign. They create
it from a Campaign Template, that can be Empty.

Properties of the Campaign defined at this step include:
- Campaign Title,
- different available dices,
- Character Sheet Templates
- Introduction text

The DungeonMaster confirms the campaign creation. Then they can invite Players
to join.

## Animate a Campaign

DugeonMaster has started a Campaign and the Players have joined. DungeonMaster
narrates the action of the campaign and is able to describe it using Text, and
Images. Sound can also be played.
DungeonMaster can ask a Player to roll dices of the kind they choose.

DungeonMaster can chat in private with any single Player.

## Play in a Campaign

Player has joined a Campaign. They can view the Campaign Narration. At the
request of the DungeonMaster, they can roll dices. They can chat in the Player
Chat window.

They can request a private chat with the Dungeon Master.

## Access Character sheet

DungeonMaster can view all character sheets of their current campaign. They can
edit all fields (Player is notified of change to their character sheet).

Each Player can see their own character sheet. They can show it to any other
Player of the campaign at their option.

## Kill a Character sheet

DungeonMaster can mark any Character sheet as Dead. This Character sheet will
be marked as such in a form like

"Killed by DungeonMaster XXX in Campaign YYY on DateZZZ. Comment: AAABBBCCC".

This does not prevent a Character sheet to be enabled for another Campaign, with
approval from the DungeonMaster.

Characters can be Unkilled by the DungeonMaster who killed them and they will no
longer appear Killed in the campaigns by this DungeonMaster.

Killed-ness can either be global or bound to a DungeonMaster.

Global killed-ness can be Disputed with an Administrator. DungeonMaster Killed-ness
cannot be disputed.
