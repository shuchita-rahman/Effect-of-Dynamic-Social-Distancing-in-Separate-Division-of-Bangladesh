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



