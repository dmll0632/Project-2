**Vanguard A/B Testing Project**


**Project Overview**

This project was developed to evaluate the effectiveness of a new user interface (UI) introduced by Vanguard. The main goal was to determine whether the new UI leads to higher completion rates, shorter action times, and fewer errors compared to the existing interface.

**Datasets**

Client Profiles:
Contains client attributes: age, gender, tenure, number of logins and calls in the last 6 months, and current balance.
Digital Footprints:
Two datasets tracking client, visitor, and visit IDs, detailing the steps taken until confirmation and the timing of these actions.
Experiment Roster:
Lists clients divided into control and test groups for the A/B test.


**Methodology**

Confirmation Sequence
A visit ID is considered confirmed if it follows the sequence: Start → Step1 → Step2 → Step3 → Confirm. Deviations from this sequence, such as repeating or backtracking steps, are assumed to indicate errors or confusion.

Objective:
The objective was to ensure a smooth flow from Start to Confirm without errors or repetition.

Assumptions:
Due to the lack of inside information about the specific steps within the app, we made the assumption that the aforementioned sequence represents the intended user flow. Any deviation from this sequence was interpreted as an indication of user error or confusion.


Analysis
Exploratory Data Analysis (EDA): Conducted to gain a better understanding of client behaviors and interactions with the UI.

KPI Dashboard: Developed using Tableau to compare key performance indicators (KPIs) between the control and test groups.


Conclusion
In the A/B testing analysis, the test group, which interacted with the new UI, visited the Vanguard website more frequently than the control group. However, the test group also experienced a higher error rate (9.26%) compared to the control group (6.89%).

Despite this, the test group had a higher completion rate of 0.68 compared to the control group’s 0.54. To assess whether this difference in completion rates was statistically significant, a hypothesis test was conducted.

Hypothesis Testing Results:
Null Hypothesis (H0): The completion rate of the test group is not more than 5% greater than the control group.
Alternative Hypothesis (H1): The completion rate of the test group is more than 5% greater than the control group.
The results showed that the observed difference in completion rates was not statistically significant at the 5% level. Therefore, we failed to reject the null hypothesis (H0), indicating that there is no significant difference in the completion rates between the new and existing UIs.
