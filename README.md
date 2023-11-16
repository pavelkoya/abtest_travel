# abtest_travel_app
Calculating conversion A/B test of travel application with proportion z-score

* Evaluate the correctness of the test
* Analyze test results

Build a funnel from viewing a ticket search form to buying an airline ticket. The main funnel a user goes through consists of 8 steps:

№ | event_number | event_name
--|--|--
1 | step_1 |travel_search_form
2 | step_2 | travel_search_in_progress
3 | step_3 | travel_search_results
4 | step_4 | travel_flight_details
5 | step_5 | travel_tariff_confirmation
6 | step_6 | travel_select_passenger
7 | step_7 | travel_payment_method
8 | step_8 | 1) travel_card_payment_approved, 2) travel_credit_approved
  
Test name: last_seats_test

1. Groups: A (control), B (last-seats);
2. Start date: 2022-07-03;
3. Stop date: 2022-07-14;
4. Expected number of test participants: 6000.
5. Problem: There are users who look at tickets in advance, e.g. 2 weeks before a trip, but postpone the purchase for a couple of days. After a couple of days, the tickets may run out.
6. Hypothesis: We hypothesize that adding information about the number of remaining tickets at the current price will increase conversion to purchase by 5% because users will understand the benefit of buying in the current moment.
