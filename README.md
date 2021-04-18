# Pitney-Bowes

#### Business problem:
Pitney Bowes FDR (Fullilment, Delivery & Returns) line of business allows retailers to easily deliver parcels to customers and  facilitate the return of merchandise If Customers are unsatisfied with products they can simply drop off the return parcels at any USPS (United States Post Office) Office, and the package will get transported to the closest Pitney Bowes FDR hub to be inducted into the Pitney Bowes carrier network. 
Once inducted into our network, the parcel gets transported from hub to hub (the Pitney Bowes FDR network) to the merchant’s warehouse.  One sss
One major requirement of these merchant’s is for Pitney Bowes to provide a forecast of the expected number of parcels that will be delivered at their warehouses. This helps predict the number of resources required to unload parcels as well as where and how to store it. 
The challenge with providing this information is that The resulting volume of parcels delivered to the  merchant’s warehouse can vary widely and is driven by external factors like seasonal sales and holidays. In addition, most warehouses have specific labor schedules which limit how much volume can be processed per day. 
In this data challenge, you will be given 3 months of historic da ta for pa ckages that ha ve been delivered to a single  merchant warehouse. 
<b>The aim is to use this historic data to predict the parcel volumes to arrive at the client's facility over the next 5 days (i.e., 5 numbers for Monday through Friday).</b>

#### Data:

The data is aggregated by delivery and induction date. The delivery column shows the total number of parcels that have been delivered to the merchant on any given day. The induction columns give you the induction volume per day across our PB FDR facilities. The time it takes a parcel to travel from the induction facility to the  merchant facility depends largely on the distance between these facilities. However, other factors like traffic, construction, and weather can effect the ablity for parcels to move from facility to facility.  In addition, the delivery methods chosen can very (expedited, normal, snail mail, etc…) Often PB is not aware of the specific service selected, only the expected date of arrival at the merchant’s warehouse. We have not provided that data here – but you are free to make assumptions if you feel it would be helpful to your model.


#### Output Format:
TBD, but all we need are your <b>5 parcel-volume predictions for June, 3rd - June, 7th 2019</b>. To evaluate your preditcions, we use the Mean Absolute Percentage Error.

$MAPE = \frac{100}{n}\sum\limits_{i=1}^{n} \frac{|y_i - \hat{y}_i|}{y_i}$ 
