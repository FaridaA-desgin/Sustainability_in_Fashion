# Sustainability_in_Fashion

# Abstract
Sustainability entails meeting the needs of current generations without jeopardizing the needs of future generations while maintaining a balance of economic growth, environmental stewardship, and social well-being. Sustainability is measured the same way in each industry but our main focus in this study is the fashion industry. Globally, the fashion industry ranks second to the oil and gas industry in terms of pollution. Fashion production accounts for 10% of global carbon emissions, deplete water resources, and pollutes rivers and streams. Furthermore, 85% of all textiles are discarded each year, and washing certain types of clothing releases significant amounts of microplastics into the ocean. The purpose of this paper is to assist companies in reducing their carbon footprint by creating a model that shows a future look at the possible damage they will add or reduce to the environment. 

# Introduction
As consumers become increasingly aware of the environmental impact of the clothing they wear, sustainability is becoming increasingly essential in the fashion business. Many fashion businesses are working to incorporate sustainable practices into their manufacturing processes, such as using organic or recycled materials, lowering water consumption, and eliminating waste. There is also a growing trend of upcycling and circular fashion, in which old items are turned into new pieces, extending their life cycle and minimizing textile waste. Sustainable fashion benefits not only the environment but also the workers who make the items since corporations place a greater emphasis on fair labor practices and safe working conditions. While there is still much work to be done, the fashion industry is gradually transitioning to a more sustainable future, and consumers can play an important role in this transformation by making informed choices and supporting brands that promote sustainability.

For decades, the fashion industry has been known for its lack of sustainability. Textile manufacture is also incredibly resource-intensive, requiring enormous amounts of water, energy, and chemicals to produce just one piece of apparel. Furthermore, the textile business produces large volumes of textile waste, with millions of tons of garments ending up in landfills each year. The environmental effect of the fashion business extends beyond production and disposal to encompass garment shipping and packaging, which contributes to carbon emissions and trash. Furthermore, the industry has been chastised for unethical labor practices such as low wages, excessive working hours, and hazardous working conditions. While some businesses are taking steps to address these challenges, the fashion industry has a long way to go before it can be considered truly sustainable.

One of the many causes of the fashion industry's carbon footprint is fast fashion. Fast fashion is a design, manufacturing, and marketing method that focuses on producing large quantities of clothing quickly. Fast fashion, in particular, has the greatest impact on the environment and social sustainability; garments produced in this industry are typically poorly made and from harmful materials. A few examples of fast fashion are Zara, H&M, UNIQLO, GAP, Forever 21, Shein, Primark, and Fashion Nova. The well-known brand that is very popular now is Shein. Shein is a direct example of a fast fashion unsustainable company. Shein’s low prices and fast production made it so popular. Consumers enjoy the ability to purchase a large number of items without the hefty price tag attached but it comes at a cost.  Their low prices have caused clothing to be made with harmful chemicals, the company has poor working conditions, has copied independent designers’ items and it is simply unethical. Companies like Shein are the reason fast fashion is so acceptable and popular. Even though their items are made cheaply and won’t last a year, young consumers who can’t afford the price tag of good quality clothing are relieved that they can get 10 items for 50$. Good quality clothing starts at the price of 25$, so of course a young low-income consumer would choose 10 shirts for 50$ instead of 2 shirts for 50$. 

In this research, We will use Random Forests, a Time Series model, Linear Regression, and Neural Networks to create a model that predicts companies’ rank in the sustainable index in 6 years. The dataset that will be used is from Fashion Revolution. The data is an index and ranks 250 of the world’s biggest fashion brands and retailers based on their public disclosure of human rights and environmental policies, practices, and impacts, in their operations and supply chains. The data comprises 246 variables covering a wide range of social and environmental topics such as animal welfare, biodiversity, climate, due diligence, forced labor, freedom of association, gender equality, hazardous chemicals, living wages, purchasing practices, supplier disclosure, waste and recycling, working conditions and more.
Literature Review 

We will now examine past studies done by several different researchers. A study (Pervez et. al, 2023) used machine learning to introduce a sustainable resin-finishing process for cotton fabric via an industrial procedure. To forecast the crease recovery angle, tearing strength, and whiteness index, many machine-learning models were constructed in sequential order. Several measures, including the coefficient of determination, mean absolute error, and root mean square error, were used to assess the effectiveness of the modeling. Findings were contrasted with those from different regression models, including fuzzy modeling, partial least squares regression, and principal component regression. For this study, commercial cotton cloth that was 100% weaved was gathered from a nearby textile mill. A total of 27 datasets were taken from the cotton fabric's resin finishing process parameters, including the resin concentration (Knittex RCT), softener for polyethylene, catalyst (Knittex® Mo), curing temperature, and curing time, along with the responses for each, such as crease recovery angle, tearing strength, and whiteness index. The outcomes were contrasted with those from various regression models, including fuzzy modeling, partial least squares regression, and principal component regression. According to the findings of the study, the least square support vector regression model had significantly higher accuracy in predicting the cease recovery angle, tearing strength, and whiteness index than other models, as evidenced by the fact that its RMSE and MAE values were significantly lower. Moreover, it provided the highest R2 values attainable, up to 0.9627.

Another machine-learning approach was done to design customized garments. Wang et. al 2013, used machine learning techniques such as radial basis function artificial neural network (RBF ANN), genetic algorithms (GA), probabilistic neural network (PNN), and support vector regression (SVR). To meet the ergonomics needs of customers, RBF ANNs were first used to determine precise human body measurements. The formalized design solutions were then generated using the GA-based models in accordance with the customer profiles (demands). In order to quantitatively characterize the relationships between consumer profiles and garment profiles from the created design solutions, the assessment model was then developed. The evaluation results would be followed by a digital demonstration and recommendation of the design solutions to the customer in decreasing order. The PNN-based models, meanwhile, were developed to forecast clothing fitness based on virtual try-on. Additionally, a self-adjustment method based on SVR was developed to estimate and manage garment design parameters in response to customer feedback. The method improves the interactions between the digital garment demonstration, the designer's professional expertise, and the user's perception to identify the most appropriate design solution. An actual application scenario of customizing leisure pants was used to demonstrate the usefulness of the new methodology. The results demonstrate that the proposed method may powerfully support the designers' quality individualized design solutions for consumers more correctly, quickly, intelligently, and sustainably. This study created a dependable and effective line of communication between consumers, fashion designers, pattern makers, and clothing manufacturers.

# Methods
The models that will be used are Time Series Forecasting, Linear Regression, Random Forest, and Neural Networks. VAR (Vector Autoregression) is a time series model used for assessing and forecasting numerous connected variables at the same time. It is an extension of the Autoregressive (AR) model in which numerous time series variables and their lagged values are included. Each variable in the system is regressed on its own lagged values as well as the lagged values of other variables in the system in a VAR model. This enables the dynamic relationship and interdependencies of variables to be captured throughout time. The VAR model is appropriate for situations in which variables impact one another and display feedback effects. The VAR model, like other time series models, presupposes stationarity of the variables, which indicates that their statistical features do not vary over time. If the variables are not stationary, transformations such as differencing can be used to achieve stationarity. Forecasting in VAR models often entails iteratively producing forecasts based on estimated coefficients and lagged variable values. VAR models provide a framework for forecasting interdependencies among variables in a time series system. This model is ideal for the purpose of this study after which the LR, RF, and NN will be implemented. 

Linear regression is a statistical modeling approach that is used to explore and quantify the connection between one or more independent variables and a dependent variable. It presupposes that the independent variables and the dependent variable have a linear relationship, which means that changes in the dependent variable are directly proportional to changes in the independent variables. The purpose of a linear regression model is to find the best-fitting line that minimizes the difference between anticipated and actual dependent variable values. Estimating the coefficients that characterize the connection between the independent variables and the dependent variable yields the line. 
Random Forest is a common categorization machine learning technique. It is an ensemble learning approach that integrates numerous decision tree predictions to produce more accurate and robust predictions. The Random Forest constructs each decision tree using the bootstrap sample and randomly picked characteristics. The tree is created recursively by separating the data based on distinct characteristics and feature values, with each split seeking to decrease impurity or increase information gain. Random Forest is frequently utilized because of its efficiency in dealing with high-dimensional data, resilience, and ability to capture complicated correlations in data. It excels at working with huge datasets and can handle both category and numerical variables.

# Dataset 
The dataset that will be used in this research includes information from 250 of the world's leading fashion companies and retailers. Fashion brands that have reported over $ 400 million in annual turnover. The dataset contains brands from across Europe, North America, South America, Asia, and Africa. The dataset has reports from 2017-2022. The Index is a tool intended to encourage and incentivize the world's leading fashion companies to be more open about their social and environmental commitments. Transparency is essential for achieving systemic change in the global fashion business. When businesses make information available to the public, anybody can scrutinize their practices, hold them responsible for their promises, and push for positive change.  It will be impossible to achieve a sustainable, responsible, and equitable fashion business without openness. Animal welfare, biodiversity, climate, due diligence, forced labor, freedom of association, gender equality, hazardous chemicals, living wages, purchasing practices, supplier disclosure, waste and recycling, working conditions, and other topics are used as variables to rank each brand. 
When cleaning the data there were a lot of missing values, 64% of the data was missing and needed to be dropped. This led to a dataset of 90 brands in total that constantly had a percentage other than zero each year. Once the dataset was clean it was run through the models mentioned above. 

# Results
The VAR Time Series Model was the most insightful in predicting the desired outcome. Looking at Table 1, it is seen that the model predicted well and was consistent with the original year, 2017-2022. For example, the first column, Abercrombie & Fitch, in 2017-2022 had consistently low percentages throughout the years. This explains the model predictions, it is unlikely that this brand will have a spick in transparency in the next 6 years. But if we take a look at the second column, Mark & Spencer, the original data shows that the percentages were low but stayed around 40-50. This is why the model predicted the percentage in the 30-40s. 

Table 1: VAR Time Series Model Prediction
Table 2: Time Series Performance Metrics 

To properly evaluate the model's predictions we will look at a few evaluation metrics. The Mean Absolute Percentage Error (MAPE) is popular for assessing forecast accuracy. MAPE is defined as the total of the individual absolute mistakes divided by the demand (per period). The percentage of mistakes is averaged. The Mean Absolute Error (MAE) is the mean of the absolute error. The Root Mean Squared Error (RMSE) is calculated by taking the square root of the average squared error. Table 2 is a short look at the forecast models performance.
     The top 3 brands with the lowest values of the MAE are Mango, Matalan, and Mexx. For Mango it indicates that, on average, the predicted values differ from the actual values by 0.001, .01 for Matalan and .02 for Mexx. Which means that the values the time series model predicted are around the same percentage. This can be seen in Figure 1 and Figure 2 is the RMSE. So for both metrics for the purpose of this study a preferred larger value would have been more ideal to show how over time the predictions can vary based on what information each brand decides to make public. Even though these brands have the lowest metrics these won’t be the top sustainably brands forecasted. 

Figure 1: Top 3 Brands with the Lowest MAE
Figure 2: Top 3 Brands with the Lowest RMSE


To get a better understanding and visual representation of how the future predictions look, we will look at the top brands with the highest percentage. It is important to note that no brand has a percentage of 100% because it is impossible to be fully sustainable, there will always be waste. Looking at Figure 3 and 4 we can see the top 3 brands with the highest percentage are Walmart, Jordan, and GUESS. We can see that 2020 is the year that is the highest for all three brands. In 2020 is the time that COVID-19 started and many stores were closed, and production and distribution of many items from different industries were stopped. The conclusion can be made that brands were aware of how COVID-19 has helped reduce their environmental impact unwillingly. This explains that the brands were more willing to report and make information public in 2020 because they weren’t producing as much. The brand that seems to be keeping a percentage over 50% that the model forecast is GUESS. Looking at Figure 5-7 we can see the difference more clearly. GUESS was the only brand out of the three that did not decrease drastically after 2020. 
It is important to mention the linear regression and random forest models in their significance. For the purpose of this study the models weren’t used to predict anything just to see how the model will do with the forecasted data. The models were both able to accurately predict the years of each percentage of the original and time series model. For this study the models weren’t significant enough to add or show any change to the time series model. 

Figure 3:Top Brand Percentages Over Tim

Figure 4: Top Brand Percentages Over Time 

Figure 5: Jordan Forecast 

Figure 6: Walmart Forecast 

Figure 7: GUESS Forecast 


# Conclusions
The results of the VAR time series model shows that it is possible to create a model companies like Fashion Revaluation can use to determine whether a Fashion brand will be transparent and in return allow consumers to make sustainable decisions. It is important to note that consumers are also to blame, if they were not buying companies would not be selling. Low quality and poor kept items will require consumers to throw them out. There are so many options in being more sustainable. A few are donating, upcycling, thrifting, and using platforms like Rent-the-Runway. But the easiest cost free option is keeping yourself educated. Which is why this model can be used by consumers to predict and be aware of how transparent their favorite brands have been or will be over the next few years. No brand can be a hundred percent sustainable but understanding how your company is impacting the environment and community is always a first step. Being transparent shows initiative and commitment to improve. Fashion sustainability starts with the company but ends with the consumer. 

# References
Fletcher, Kate. "Durability, fashion, sustainability: The processes and practices of use." Fashion practice 4.2 (2012): 221-238.
Hur, Eunsuk, and Tom Cassidy. "Perceptions and attitudes towards sustainable fashion design: challenges and opportunities for implementing sustainability in fashion." International Journal of Fashion Design, Technology and Education (2019).
Joy, Annamma, et al. "Fast fashion, sustainability, and the ethical appeal of luxury brands." Fashion theory 16.3 (2012): 273-295.
Pervez, Md Nahid, et al. "Sustainable fashion: Design of the experiment assisted machine learning for the environmental-friendly resin finishing of cotton fabric." Heliyon (2023): e12883.
Nilashi, M., Rupani, P. F., Rupani, M. M., Kamyab, H., Shao, W., Ahmadi, H., ... & Aljojo, N. (2019). Measuring sustainability through ecological sustainability and human sustainability: A machine learning approach. Journal of Cleaner Production, 240, 118162.
Wang, Z., Tao, X., Zeng, X., Xing, Y., Xu, Z., & Bruniaux, P. (2023). Design of Customized Garments Towards Sustainable Fashion Using 3D Digital Simulation and Machine Learning-Supported Human–Product Interactions. International Journal of Computational Intelligence Systems, 16(1), 16.



