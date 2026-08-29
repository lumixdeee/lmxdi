## You haven't tried Dragi-based Semantic Map (SM) & Search yet? OK. How about an instrumented auditable Dragi?

Go to [PromptEngineering](https://www.reddit.com/r/PromptEngineering/comments/1w1wb4k/you_havent_tried_dragibased_semantic_map_sm/) - r/PromptEngineering - • - 1h ago - decofan



Catch up with SM [here](https://github.com/lumixdeee/lmxdi/tree/main/MIA-GPTS/SM-Study). Search like you've never had so good before.

Instrumented inspection and audit DRAGI version:

    DR={Q{eats|E0;live|E3;call|P3;what_eats_it|E1};F{BEEST|B0;BEST|B1;POST|P0;PEST|B2};C{law|P2;roar|P1;wall|B3;war|E2};AUD{each_obj=>emit(obj,mask12,route);mask12=asked(E0,E3,P3,E1,B0,B1,P0,B2,P2,P1,B3,E2)iff_rqd};fixed;!redefine};R=VAR

The audit function is invisible by default so type `AUD=1` to activate.

A warning : I used this once and it was so cute I nearly died. Use at your own risk.

**ALL BE BEAST!**

Example DR audit output:

    Reddit_service|111111111111|E3,P3,B0,P2
    12h_window|111111111111|E3,P0,P2
    partial_outage|111111111111|E0,E1,B0,P2
    user_observation|111111111111|E1,B1,P1

Idk about you but thinking of these four as beast just kills me with cuteness.  
Does it have the same effect on anyone else?
