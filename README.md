#Data Science Hackathon form Cat_Loaded
-----------------------------------------------------
Advise from a friend to apply
Drop some columns
Handling time
Handling categorical
Handling distances ( longitude and latitude)
Standard Scaler

Splitting
Dummy Classifier will give you accuracy  higher than 50 %

Try Random Forest or Xgbclassifier will give you accuracy 56-57%

--------------------------------------

The dataset provided includes order dispatch details and rider metrics based on orders made on the Sendy platform. The challenge is to predict the reaction of a partner rider to an order: is a rider most likely to ignore, decline or accept the dispatch they receive? Sendy provides an API as well as a web and mobile application platform to link customers who have delivery needs with vetted transporters. The customers select their vehicle of choice, get their price quote upfront and pay using various payment options. The system optimises the route, looks for the closest available riders and dispatches the orders in the most efficient way. The training dataset provided here is a subset of over 200,000 dispatches and only includes direct orders (i.e. Sendy “express” orders) with bikes in Nairobi. All data in this subset have been fully anonymized while preserving the distribution. The objective of this challenge is to create a machine learning model that will predict whether a rider will accept, decline, or ignore an order sent to them.
Files available for download:

Train.csv - contains the target. This is the dataset that you will use to train your model.
Test.csv- resembles Train.csv but without the target-related columns. This is the dataset on which you will apply your model to.
SampleSubmission.csv - shows the submission format for this competition, with the ‘ID’ column mirroring that of Test.csv and the ‘target’ column containing your predictions. The order of the rows does not matter, but the names of the ID must be correct Variable definitions
Dispatch Data
ID - Unique ID for each order request
order_id – Unique number identifying the order
client_id - Unique number identifying the customer on a platform
client_type - Specifies the customer type (Business or Personal)
rider_id - Unique number to uniquely identify the rider
rider_license_status - Identifies riders who have a license to access restricted areas i.e. 0 (Cannot access a restricted area) and 1 (Can access a restricted area)
rider_carrier_type - Identifies the box option that a rider currently has i.e. 0 (No Box option) and 1 (Box option)
rider_amount - The earnings a partner would earn if they successfully complete an order.
order_license_status - Identifies orders that require a pick-up or drop-off in a restricted area i.e. 0 (Restricted area) and 1 (Non-Restricted area)
order_carrier_type - Identifies the box option the customer specified while placing their orders i.e. 0 (No box option), 1 (Box option), 2 (Any option)
vendor_type – For this competition limited to bikes. However, in practice, Sendy’s service extends to Vans and Trucks.
Pickup Latitude and Longitude (pickup_lat and pickup_long) - Latitude and longitude of pick up location
Destination Latitude and Longitude (drop_off_lat and drop_off_long) - Latitude and longitude of delivery location
Rider Latitude and Longitude (rider_lat and rider_long) - Latitude and longitude of the Rider at the time of dispatch.
target - The reaction of a rider in regards to a particular dispatch. Did a rider ignore (0), decline (1) or accept (2) a dispatch?

Dispatch times
dispatch_day - Day of Month i.e. 1-31

dispatch_day_of_week - Weekday (Monday = 1)
dispatch_time - Time of day the dispatch was sent out to the riders
