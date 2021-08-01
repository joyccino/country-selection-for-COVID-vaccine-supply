# Country Selection for COVID Vaccine Supply

The Data for this project is from [ourworldindata.org](https://ourworldindata.org/coronavirus-source-data) and the Dataset can be found in [this GitHub Repository](https://github.com/owid/covid-19-data/tree/master/public/data/). <br>

# Task process
* Searching the appropriate dataset <br>
Information the dataset should contain: total tests, total cases, total deaths, positive rate, reproduction rate, <br>
population, gdp per capita, extreme poverty,available hospical beds, vaccinations rate, total vaccination ... <br>
* Select 200 countries with the hiehest number of confirmed cases per population.
* Among 200, select 180 countries with the highest fatality rate. (deaths/confirmed_cases)
* Among 180, select 160 countries with the highest reproduction rate.
* Among 160, select 130 countries with the lowest GDP per capita.
* Among 130, select 100 countries with the lowest fully_vaccinated_rate.
* Among 100, exclude 20 countries with the lowest vaccinated_rate. (This is because there is a high probability that 20 countries do not have a enough vaccine infrastructure, so even if covid vaccines are arrived, there is a high possibility that vaccination will not be carried out properly.)
* Drop rows if vaccinated_rate == NaN. (it is difficult to determine their vaccination status.)
* Drop 5 more countries with the highest number of fully_vaccinated people.
* Visualise on a map to locate the remaining 22 countries. It is confirmed that these countries are concentrated in South America and Asia.
* Find two or three countries with rich infrastructure and close proximity to neighboring countries that can become COVID-19 vaccine hubs.
* Among 22 countries, select 15 countries with the highest GDP per capita.
* Among 15 countries, select 9 countries with the extreme poverty rate less than 4.
* Devide the remaining countries into two groups : South-America and Asia-Europe.
* [South America] Argentina's primary vaccination rate is 53%, and the number of beds is the highest, and relatively stable vaccination and corona infection control are in progress.
* The population of Brazil is nearly 10 times that of the other two countries, so it could mean that they set the reasonable strategy for vaccination and infrastructure construction could more abundant than Argentina.
* According to some news articles, the new government of Peru is expected to be limited in its role as a global vaccine hub right at the moment, as it has been tasked with resolving political chaos and unifying divided public minds.
* Therefore, Brazil seems to be the most suitable country as a vaccine hub in South America.
* [Asia-Europe] Russia is excluded since they already have Sputnik V vaccine. The three countries with top GDP per capita is South Korea, Malaysia and Kazakhstan.
* Countries that are accelerating vaccination are Malaysia, Sri Lanka and South Korea. However, Sri Lanka is excluded since they has a large dependency on external vaccine support.
* Low total death rate could mean that the country's medical infrasturcture is well equipped. The three countries with the lowest total death rate are Malaysia, Kazakhstan and South Korea. Among them, Kazakhstan is excluded as they developed Kazbek (vaccine).
* Therefore, as Malaysia and South Koreahave the best conditions as vaccine hubs, if vaccine support to these two countries is given priority, they can swap vaccine swap with neighboring countries to increase vaccine availability. Afterwards, these two countries can provide their cold chain system to storage vaccine for the neighboring countries.
* In order to divide vaccine doses to above three countries, the size of cold chain market of each country should be understood. However, there is no related data available, 
hospital_beds_per_thousand will be used to determine the size of the country's health/medical infrastructure.
* As a result, 116066 doses of vaccine can be supplied to Malaysia, 749542 to South Korea and 134392 to Brazil.
