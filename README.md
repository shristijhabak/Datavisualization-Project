# Datavisualization-Project
DataSet-

The dataset used here for visualization is from the US consumer complaint database. The Consumer Complaint Database is a collection of complaints on a range of consumer financial products and services, sent to companies for response and it is created by Consumer Financial Protection Bureau. Consumer Financial Protection Bureau each week they send thousands of consumer complaints to the desired companies for response and then company responds or after 15 days whichever comes first, then the information is stored in the database and it is available for public.
 
The dataset was created in July 2011, the database generally updates daily, contains certain information for each complaint, including the source of the complaint, the date of submission, and the company where complaint was sent to for response. The database also includes information about the actions taken by the company in response to the complaint, such as, whether the company’s response was timely and how the company responded.

Link to data-https://catalog.data.gov/dataset/consumer-complaint-database


The dataset has 18 different attributes such as state, submitted via, consent provided, timely response etc., that has been used for visualization.

State	The state of the mailing address provided by the consumer.
Consumer consent provided?	Identifies whether the consumer opted in to publish their complaint narrative. We do not publish the narrative unless the consumer consents, and consumers can opt-out at any time.
Submitted via	How the complaint was submitted to the CFPB. For example, “Web” or “Phone.”
Timely response?	Whether the company gave a timely response. For example, “Yes” or “No.”
Product	The type of product the consumer identified in the complaint. For example, “Checking or savings account” or “Student loan.”

For the data-  Removed some of the attributes that we are not using for visualization such as Zip code, ComplaintId, Tags, Date etc. 



Questions that can be answered-

1.	a. We can look at the complaints people by state and look for any pattern. May people in the South are less likely to complaint. Or maybe people in the Midwest are less likely to complaint?


-	I was thinking of getting any pattern before implementing but after visualizing I am not getting any pattern.
-	I use a hexagon map to show the 59 different states of the US and color coding of each state to display the volume of complaints per 150,000 or the product with the most complaints in that state. The map can be switched between each representation by a button presented to the user. For the representation of number of complaints, sequential color is used as the channel lighter the color shows less number of complaints the darker the color the higher the number of complaints per 150,000. We can observe that California has most complaints than any other state, as we look on the hexagon map.

-	 

b. Is there any geographical pattern regarding the product people are mostly complaining? 
-For the complaints per product representation a range between green and blue have been used to identify each product. If the state is colored with the color for any one product then that product has the highest number of complaints in that state. In both representational forms the map states are interactive to the mouse rolling over revealing an information pane about that state. This information pane goes a more detailed view of the complaints for that state including where the complaints tend to be submitted.
-We can see from the map that people are mostly complaining regarding product mortgage and debt collection than any other product and also there are more number of states that are have complaints with mortgage than debt collection.


 
2.Explore what kind of complaints tend to result in a satisfactory response. We can look at the flow of each complaint from the initial submitting to the final resolution for clues. We want to find out answers to questions such as: is it better for a consumer to opt in to publish their complaint and submit via web, or submit through another source?
  
I used Sankey graph to see the volume of complaints for each submission type such as Web, email, referral etc. relevant to whether consent was provided or not, and then of which of those complaints were resolved or not. The volume of complaints relative to total number of complaints for each flow is represented by the height of the node and the size of the links between the nodes. The height of web submission type is more than referral or any other submission type that means more number people opt web submission type. 
The complaints are registered with different sources such as web, referral, email, phone, fax, postal mail. Mostly people prefer to file complaint via web than other sources. There are 252,901 people who provided consent through web and their complaint is not resolved whereas 50,659 people didn’t provided consent, but their complaint has been resolved. We can say from looking the graph that it’s better for people to submit their complaint via web than any other source as the percentage of resolution for the complaint is very less from other sources.
 

Stacked Bar Chart-
I have created static stacked bar chart where X-axis represents the number of complaints and Y-axis represents the submission type, where green color shows resolved number of complaints, red color shows the complaints that are unresolved, and orange shows not applicable complaints.
I also made a static stacked bar chart too to make it more specific. People mostly preferred to file their complaint through web but in web there are high number of complaints that are not applicable that is shown by orange color than any other submission type. Also,we can say number of complaints through are resolved than other submission type 


 






-.

