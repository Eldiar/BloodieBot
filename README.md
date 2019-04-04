# BloodieBot
A discord bot used in BloodFeast Guild Discord for Black Desert Online

## Implemented features:

## Upcomming features:

#### ---- Nodewar Scheduling and RSVP: ----

Commands:
!bl nw schedule [date]
!bl nw placed [server] [date]

Event chain:
- "!bl nw schedule [date]" is used
- Text channel with name "Node War [date]" is created by Bloodie
- 48 hours before Node War, RSVP message is sent:
  	
		@Nodewar
		RSVP - Node War Attendance - [date]
		Please let us know if you are attending the Node War on [date] at 20.00 CE(S)T
		[checkmark][cross]
  	
- If the checkmark is clicked bot updates the message with people who signed up for Node War:
  	
		The following people have signed up for Node War: [Amount of people]
	 	[name]
	 	[name]
		[name]
  	
- 12 hours before Node War, a fort placing reminder is sent:
  	
		@Officer
   		Remember to place the Node War fort!
  	
- 3.5 hours before Node War, if the command "!bl nw placed server" is not used, the bot will send another reminder:
	
		@Officer
   		Remember to place the Node War fort! You only have 1.5 hour left!
	
- 1.5 hours before Node War, the bot will send a foodbuff reminder:
	
		@Foodbuff
		Everyone who is participating in Node War, do not forget your food rotation! 1st foodbuff starts now.
	
- 1 hour before Node War, the bot will send another foodbuff reminder:
	
		@Foodbuff
		2nd foodbuff should start now!
	
- 0.5 hours before Node War, the bot will send a reminder to all participants:
		
		Node War is starting in 30 minutes
		Please get ready to join voicechat

		The Node War channel is: [channel]
		Do not forget to set your participation status to YES!

		3rd foodbuff should start now!
		Do not forget your **villa buff**, a **repair** and **potions**!

		Please bring the following materials to Node War:
		60 Iron ingot
		30 Melted copper shards
		60 Polished stone
