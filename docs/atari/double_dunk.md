---
layout: "docu"
title: "Double Dunk"
actions: "Discrete"
agents: "2"
manual-control: "No"
action-shape: "(1,)"
action-values: "[0,17]"
observation-shape: "(210, 160, 3)"
observation-values: "(0,255)"
import: "from pettingzoo.atari import double_dunk_v0"
agent-labels: "agents= ['first_0', 'second_0']"
---

{% include info_box.md %}




An adversarial game that combines control and precise selection.

The game has two stages: selection and play. Selection can be
difficult because you have to hold the same action for a few steps and then
take the 0 action. Also, since both players have to select a play
in order for play to resume, there is possiblity of learning to
stall by not selecting anything.
Once play begins, each team has two players. You only control
one at a time, and and which one you control depends on the selected play.
Scoring should be familar to basketball fans (2-3 points per successful shot).

[Official double dunk manual](https://atariage.com/manual_html_page.php?SoftwareLabelID=153)


#### Environment parameters

Environment parameters are common to all Atari environments and are described in the [base Atari documentation](../atari) .
