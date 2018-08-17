trigger and objective:
================================================================================================================================

	if the client submits a beneficiary details change request, and admin has NOT approved it, then show a visual indicator on the relevant fields to prompt then to APPROVE/"REJECT" the beneficiary changes.

Use cases
================================================================================================================================

	(admin only)

		#.	Contract Summary -> Allocate a beneficiary payment -> beneficiary table; 
		  	
		  		#.	(an admin is allocating the beneficiary; )
				#.	under the beneficiary dropdown list, show visual indicator beside the beneficiary entry; show text when hovering over the icon:

						"This payment contains changed beneficiary details which have not been approved. Please APPROVE/REJECT to continue."

				#.	allocate the beneficiary payment on the changed beneficiary; 
				#.	upon clicking "CONFIRM", redirect current tab to Compliance -> Beneficiary Changes; 
				#.	this redirection will be filtered to the single related beneficiary change (on that entry); 
				#.	the admin either accepts or rejects the change; 
				#.	upon clicking either "CONFIRM" or "REJECT", redirect current tab to whatever the previous screen was; 
						
						#.	if "CONFIRM", then the new beneficiary is automatically assigned to the beneficiary payment; 

		#.	Contract Summary -> allocated beneficiary payment entry; 

				#.	show visual indicator beside the beneficiary payment
						
						-	the visual indicator contains a hyperlink to Compliance -> Beneficiary Changes; 
						-	show text when hovering over the icon:
						
								"This payment contains changed beneficiary details which have not been approved. Please APPROVE/REJECT to continue."
				
				#.	upon clicking the hyperlink, redirection will be filtered to the single related beneficiary change (on that entry); 
				#.	the admin either accepts or rejects the change; 
				#.	upon clicking either "CONFIRM" or "REJECT", redirect current tab to whatever the previous screen was; 
						
						#.	if "CONFIRM", then the new beneficiary is automatically assigned to the beneficiary payment; 
		
		#.	Beneficiary Payments -> beneficiary payment entry; 

				#.	show visual indicator beside the beneficiary payment entry; 
				  	
						-	the visual indicator contains a hyperlink to Compliance -> Beneficiary Changes; 
						-	show text when hovering over the icon:
				  	
				  		"This payment contains changed beneficiary details which have not been approved.  Please APPROVE/REJECT to continue."

				#.	upon clicking the hyperlink, redirection will be filtered to the single related beneficiary change (on that entry); 
				#.	the admin either accepts or rejects the change; 
				#.	upon licking either "CONFIRM" or "REJECT", redirect current tab to whatever the previous screen was; 
				
						#.	if "CONFIRM", then the new beneficiary is automatically assigned to the beneficiary payment; 
		
		#.	Beneficiary Payments -> Edit a payment -> beneficiary table; 

				#.	(an admin is editing a beneficiary payment); 
				#.	under the beneficiary dropdown list, show visual indicator beside the beneficiary entry; show text when hovering over the icon:
				
						"This payment contains changed beneficiary details which have not approved.  Please APPROVE/REJECT to continue."

				#.	the admin selects the changed beneficiary (and make any number of changes on the same authentication token request); 
				#.	upon entering the Authentication Token and clicking "CONFIRM", redirect current tab to Compliance -> Beneficiary Changes; 
				#.	this redirection will be filtered to the single related beneficiary change (on that entry); 
				#.	the admin either accepts or rejects the change; 
				#.	upon clicking either "CONFIRM" or "REJECT", redirect the current tab to whatever the previous screen was; 
					
						#.	if "CONFIRM", then the new beneficiary is automatically assigned to the beneficiary payment; 
		
		#.	Customers -> Beneficiary -> beneficiary table
		
				#.	show visual indicator beside the beneficiary entry; 
				  	
						- the visual indicator contains a hyperlink to Compliance -> Beneficiary Changes; 
						- show text when hovering over the icon:
						  
							"This payment contains changed beneficiary details which have not been approved.  Please APPROVE/REJECT to continue."
				
				#.	upon clicking the hyperlink, redirection will be filtered to the single related beneficiary change (on that entry); 
				#.	the admin either accepts or rejects the change; 
				#.	upon clicking either "CONFIRM" or "REJECT", redirect current tab to whatever the previous screen was; 
				
						if "CONFIRM", then the new beneficiary is automatically assigned to the beneficiary payment.

	(client only)

		#.	My Beneficiaries -> beneficiary table
		
				#.	show visual indicator beside the beneficiary entry; show text when hovering over the icon:

						"You have submitted a beneficiary update request.  Please wait for the approval confirmation."