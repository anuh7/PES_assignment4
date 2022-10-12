# PES_assignment4


The traffic lights have the following behavior:
-	When the traffic light is in the STOP state, Buffahiti residents use the color #611E3C .
-	When the traffic light is in the GO state, Buffahiti residents use the color #229622
-	When the traffic light is in the WARNING state, Buffahiti residents use the color #FFB200
-	When someone presses the button to cross the street (CROSSWALK state), the traffic light is blinking with the color #001030. 
- In the CROSSWALK state, the light blinks 250 msec off, 750 msec on. In all other states, the light is solid (not blinking).
- At any point in the above cycle, if the button is pressed to cross the street (represented on our FRDM-KL25Z by a touch anywhere on the capacitive slider), the traffic light should do the following:
- Transition, over a one-second period, from whatever the current color is to the CROSSWALK color (#001030). This one-second transition should follow the approach given above.
-	Stay in the CROSSWALK mode for 10 seconds, blinking 250 msec off, 750 msec on. (This duration is the same in both DEBUG and PRODUCTION modes.)
-	Transition, over a one-second period, from the CROSSWALK state to the GO state.

In the debug mode states remain for 5s and in production mode, they remain for 20s.

# PEER REVIEW 
By Daanish (11.10.2022 at 11:45pm)
- Use timing API functions (reset_timer, get_timer, reset_poll_timer and poll_timer)
- Use macros in systick.h and pwm_init.h for MOD register value and Systick Load register
- Comment variables declared in state_machine.c

