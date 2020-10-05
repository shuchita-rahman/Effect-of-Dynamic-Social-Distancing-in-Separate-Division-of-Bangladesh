### Effect-of-Dynamic-Social-Distancing-in-Separate-Division-of-Bangladesh

###  Abstract
Every 100 year throughout the history, a pandemic always ravaged humanity. In 1818 “Cholera”, 1918
“Spanish Flu” and now Corona. Novel corona has proven the world that how much our health system is
vulnerable in this modern age. From the beginning of this year researcher are trying to find every little
aspect about this virus. Researcher tried to discuss about the situation about COVID-19 in Bangladesh.
Still there is lack of data and information how division wise corona affecting Bangladesh. The
motivation of this report is (i)gathering scattered data of different division in one place, (ii)learning
how COVID-19 effecting Bangladesh in this division(Dhaka and Barisal),(ii)depending on the situation
how to we should take precaution in different division of Bangladesh. I have collected data from 4 th
April to 10 th May 2020 division wise. I have used extension of SEIR model to predict death for next 5
days. Then I am going to investigate how varying social distancing effect the division separately.
Keyword- COVID-19, SEIR model, Social distancing.
### 2. Introduction
The ongoing pandemic which broke the world’s health system known as corona pandemic or COVID-
19, caused by respiratory syndrome coronavirus (SARS-CoV-2).It was first discovered in December
13 th , Wuhan China. Then the virus rapidly spread throughout China. It took WHO(World Health
Organization)January 5 th ,2020 for declaring it as a pandemic. Till then there was already 60,0000
positive cases in China. Because of mutation this virus symptom varies changing from host to host.
Researcher minimize down to this three common symptoms fever, cough and shorten of breathing.
Other symptoms are sore throat, muscle pain, diarrhea,vomit etc. This virus mainly threaten to elderly
and people whom have respiratory, diabetes, heart diseases. COVID-19 primarily transmitted from
symptomatic people to other who are close contact through respiratory droplets, by direct contact with
infected persons, or by contact with contaminated objects or surfaces.
This virus is found in Bangladesh in 3 th March, 2020 from two returned individual from Italy.
Government took 17 day before announcing whole nation lock down. But after 88 day lock down
government reopen some of private and public institution. This strategy could be a guide in how
government should take the lock down strategy in division wise to control spreading the virus.
### 3. Data
The data is I have used in this report is currently taken from COVID-19 traker of Bangladesh which
resource is maintain by The John Hopkin University. For comparing prediction result I have used data
of WHO’s(World Health Organization) COVID-19 Situation Report of Bangladesh.
### 4. Methodology
In this section I will describe the procedure in details gradually before coming to a conclusion. First I
have collected data of confirmed, infected, recovered and death number causes by COVID_19 from 5 th
April to 10 th June of 8 division of Bangladesh. From the data I am choosing 2 division Dhaka, Barisal
to do rest of the work. As I want to predict data(confirmed, infected, recovered and death) for next 5day I trained my model to learn the parameter. Second, I have used extend SEIR model to predict data
for next 5 days. Third, I brought a new parameter for social distancing to show how division wise it
effect differently.
### 4.1 SEIR Model
The compartmental model SEIR is extension of SIR model. SEIR model is composed by four basic
compartment, taken by certain ‘t’ time.
S = Number of susceptible individual
E = Number of exposed individual
I = Number of Infectious individual
R = Number of Recovered individual
Hence it is based on four time function S(t), E(t), I(t), R(t). This function is normalized in a way that in
any given time it will fulfill following equation where N is the constant total population,
N = S + E+ I + R      (i)
The model predict infection diseases which transmitted from human to human, an individual
experienced long incubation duration where recovered confirmed lasting resistance.
![image](https://user-images.githubusercontent.com/14909839/94916997-86bad800-04d1-11eb-9030-7132a35a23bb.png)
The infection rate, Beta, represents the probability of transmitting diseases between susceptible and
infectious individual. Alpha(1/t_incubation), is the inverse rate of the incubation period. Gamma
(1/t_infectious), is recovered rate. It can be represents by the set of differential equation.
![image](https://user-images.githubusercontent.com/14909839/94917152-d26d8180-04d1-11eb-8075-fb1b824f4f49.png)
There is one parameter which need to mentioned is Ro, it is sum up of infected individual who
recovered from the virus and those who died in the virus. Following equation represents how dieases
spreading can be related to the parameter ,beta and gamma.
![image](https://user-images.githubusercontent.com/14909839/94917216-f4670400-04d1-11eb-9836-79888119a57b.png)
### 4.2 SEIRD Model
Diseases model play an important role to understand the complex pattern of the disease. Modeling is
the first step to understand what treatment and approaches can be most effective. From the dynamic of
COVID-19 I have learn that after getting infected by the virus some individual sadly die. For this
reason I have brought a new compartment D, death. This model is the extension of SEIR model. The
population also divided in 5 compartment.
N = S + E + I +R+ D                          (viii)
Here I am introducing to the new parameter ,delta. Death rate.
![image](https://user-images.githubusercontent.com/14909839/94917306-1f515800-04d2-11eb-92c0-18880d68b449.png)
Now the dynamic of this model value dependent on the setting of alpha, beta, gamma, and delta.
### 4.3 SEIRD Model with Dynamic Social Distancing
As we don’t know anything about preventing COVID-19, many countries including Bangladesh used
social distancing like avoiding large gathering, physical contact person to person, other efforts to
reduce the spreading. From the statics of the world data we see China and Italy were able to stop
spreading after taking this initiative. Hence, I am introducing to a new parameter rho, to understand
how social can effect the virus spreading. The value of rho, will be constant term between 0 to 1. 0
indicates the ideal approach whole country is lock down and quarantined, where 1 considered as no one
maintaining social distance. The introduction of , rho, will effect equation (ii) and (iii) where individual
is contacted by exposed or infectious individual. So our final equation for SEIRD model is following
![image](https://user-images.githubusercontent.com/14909839/94917433-545daa80-04d2-11eb-96fa-c73aea0a4513.png)
Hence the model is dependent on four parameter alpha, beta, gamma and rho.
Reason I have used the term dynamics because of the decision government has taken . After staying
lock down for 88 days government have decided to open most of the private, public office. It will effect
the parameter rho. Bangladesh is densely populated country where the population density is not divided
equally. Capital city Dhaka has most densely area, with a density of 23,234 per square per kilometer
where Barisal is lowest densely area, with a density of 10,514 per square kilometer.
So keeping, rho, value same for every division same is unreasonable.As the time will pass more more shop in Dhaka will open and things will get worse. In the following of my experiment I will try prove that in some division of Bangladesh the social distancing should be
maintained strictly, where other division it can be liberal.
### 5. Result
In the section I am going to discuss the result in two stage. In the first stage I applied SEIRD model to
predict future data and show it’s authentication. In second stage I applied different, rho, values for three
division to show the scenario.
### 5.1 Modeling Dhaka and Barisal
I am going to run the experiment twice taking this two division Dhaka and Barisal. Important note
Dhaka the is most densely populated division in Bangladesh, with 47,424,418 residence and Barisal
lowest populated division, with 83,25,666 residence. It will be easy to show the by taking this two
division.From the recent information the incubation period is 5 days. Applying differential SEIR model I find
the following data.
![image](https://user-images.githubusercontent.com/14909839/94917614-a8688f00-04d2-11eb-8391-c27d69f01b6d.png)

From WHO’s data of 15 th May in Dhaka and Barisal confirmed and death cases 9988 ,180 and 158 and
19. Which is closer to our prediction data. This result show how division wise is effecting virus
differently.
### 5.2 Applying Dynamic Social Distancing
Now I am going to use the parameter of last investigation for further query. For Dhaka alpha = .008,
beta = 1.920 and gamma = 0.035.
![image](https://user-images.githubusercontent.com/14909839/94917839-26c53100-04d3-11eb-9c8a-b70ea6b17898.png)
Again from last investigation we found parameter for Barisal alpha = 0.002, beta = 2.85 and gamma =
0.00
![image](https://user-images.githubusercontent.com/14909839/94917896-48261d00-04d3-11eb-94cf-dd59351f7fac.png)
To understand more accurately I am going to compare exposed individual of Barisal and Dhaka.
![image](https://user-images.githubusercontent.com/14909839/94917927-5b38ed00-04d3-11eb-9aca-3bb794fc395b.png)
### 6. Conclusion
This report show how division wise virus is effecting differently and taking same social distance
approach for every division is unrealistic. Hence without opening full lock down all over Bangladesh
division wise government should take separate strategy for each division.
### Reference
1. https://arxiv.org/pdf/2004.00553v1.pdf
2. https://arxiv.org/pdf/2005.02365v2.pdf
3. https://towardsdatascience.com/social-distancing-to-slow-the-coronavirus-768292f04296
4. https://www.thelancet.com/journals/langlo/article/PIIS2214-109X(20)30074-7/fulltext
 
data source : http://covid19tracker.gov.bd/
