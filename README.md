📌 Donor Targeting Optimization (Business-Focused ML Project)

💼 Business Problem

A national nonprofit organization conducts large-scale direct mail campaigns to solicit donations. However:

Only ~5% of recipients respond
Mailing costs are high (printing + postage)
Most outreach is wasted on non-donors

👉 This results in low ROI and inefficient marketing spend

🎯 Business Objective

Use historical donor data to:

Identify individuals most likely to donate
Reduce unnecessary outreach costs
Maximize net fundraising revenue

💡 Project Goal

Develop a predictive classification model that scores each individual by likelihood to donate.

Instead of mailing everyone:

Target only high-probability donors
Reduce campaign size while maintaining (or increasing) revenue

📊 Analytical Approach

Data Used
Demographics (income, home value)
Donation history (last gift, lifetime value)
Engagement (recency, frequency of contact)
Models Built
Logistic Regression (baseline, interpretable)
Random Forest (non-linear patterns)
Support Vector Machine (advanced classification)

📈 Key Findings (Business Insights)

1. Recency Drives Donations
Customers who donated recently are significantly more likely to donate again
 Suggests strong value in retention strategies
2. Previous Gift Amount Matters
Higher past donations = higher probability of future donations
   Ideal segment for premium targeting
3. Income is NOT the Strongest Driver
Lower-to-mid income groups showed higher response rates
 Challenges assumption that “wealthier = better donors”
4. Diminishing Returns on Outreach
Excessive promotions reduce effectiveness
 Over-contacting leads to fatigue

Model Performance & Selection
Model	Strength
Logistic Regression	Best interpretability
Random Forest	Best practical prediction
SVM	Weak performance

 Random Forest selected for deployment due to better real-world prediction of donors

💰 Business Impact (Estimated)

Using the model, the organization can:

🎯 Target top ~30–40% high-probability donors
📉 Reduce mailing costs significantly
📈 Maintain or increase total donations

👉 Result: Higher ROI per campaign

🚀 Implementation Strategy

Score entire donor database using the model
Rank individuals by predicted probability
Select top segment for campaign targeting
Monitor response rate & refine model

📊 Example Use Case

Instead of mailing 100,000 people:

Mail only top 35,000 predicted donors
Achieve similar donation volume
Save ~65% in mailing costs

🛠️ Tools & Technologies

R (glm, randomForest, e1071)
Data cleaning & feature engineering
Model evaluation (ROC, AUC)
Data visualization

📌 Future Improvements

Add cost-sensitive modeling (profit optimization)
Deploy as dashboard (Tableau / Power BI)
Integrate real-time scoring

👤 Author

Doris Mbitazi Asongafac
