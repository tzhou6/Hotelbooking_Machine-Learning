# Hotel Booking Cancelation Estimator: Project Review

* Created a tool that estimates hotel cancelation to help the hotels better manage their room arrangement in order to increase the revenue and decline the room vacancy rate.
* Data is originally from the article Hotel Booking Demand Datasets, written by Nuno Antonio, Ana Almeida, and Luis Nunes for Data in Brief, Volume 22, February 2019.
* Trained classification models of Logistic Regression, Support Vector Machine (SVM), Random Forest, Decision Tree and XGBoost in Python
* Used GridsearchCV to implement Hyperparameters Tuning for model selection.
* Tested created models on hold-out data and performed model scoring selection using Confusion Matrix, F1 score, recall, precision, ROC-AUC.

# Code and Resources Used
* Python Version: 3.7
* Packages: pandas, numpy, sklearn, matplotlib, seaborn
* Data Resource: https://www.kaggle.com/jessemostipak/hotel-booking-demand

# Features 
* ADR	       Average Daily Rate as defined by [5]
* Adults	       Number of adults
* Agent	       ID of the travel agency that made the bookinga
* ArrivalDateDayOfMonth	       Day of the month of the arrival date
* ArrivalDateMonth	       Month of arrival date with 12 categories: “January” to “December”
* ArrivalDateWeekNumber	       Week number of the arrival date
* ArrivalDateYear	       Year of arrival date
* AssignedRoomType	       Code for the type of room assigned to the booking. Sometimes the assigned room type differs from the reserved room type due to hotel operation reasons (e.g. overbooking) or by customer request. Code is presented instead of designation for anonymity reasons
* Babies	       Number of babies
* BookingChanges	       Number of changes/amendments made to the booking from the moment the booking was entered on the PMS until the moment of check-in or cancellation
* Children	       Number of children
* Company	       ID of the company/entity that made the booking or responsible for paying the booking. ID is presented instead of designation for anonymity reasons
* Country	       Country of origin. Categories are represented in the ISO 3155–3:2013 format [6]
* CustomerType	       Type of booking, assuming one of four categories:
* DaysInWaitingList	       Number of days the booking was in the waiting list before it was confirmed to the customer
* DepositType	       Indication on if the customer made a deposit to guarantee the booking. This variable can assume three categories:
* DistributionChannel	       Booking distribution channel. The term “TA” means “Travel Agents” and “TO” means “Tour Operators”
* IsCanceled	       Value indicating if the booking was canceled (1) or not (0)
* IsRepeatedGuest	       Value indicating if the booking name was from a repeated guest (1) or not (0)
* LeadTime	       Number of days that elapsed between the entering date of the booking into the PMS and the arrival date
* MarketSegment	       Market segment designation. In categories, the term “TA” means “Travel Agents” and “TO” means “Tour Operators”
* Meal	       Type of meal booked. Categories are presented in standard hospitality meal packages:
* PreviousCancellations	       Number of previous bookings that were cancelled by the customer prior to the current booking
* RequiredCardParkingSpaces	       Number of car parking spaces required by the customer
* ReservationStatus	       Reservation last status, assuming one of three categories:
* ReservationStatusDate	       Date at which the last status was set. This variable can be used in conjunction with the ReservationStatus to understand when was the booking canceled or when did the customer checked-out of the hotel
* ReservedRoomType	       Code of room type reserved. Code is presented instead of designation for anonymity reasons
* StaysInWeekendNights	       Number of weekend nights (Saturday or Sunday) the guest stayed or booked to stay at the hotel
* StaysInWeekNights	       Number of week nights (Monday to Friday) the guest stayed or booked to stay at the hotel
* TotalOfSpecialRequests	       Number of special requests made by the customer (e.g. twin bed or high floor)
