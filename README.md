# population-growth
Population Growth simple code

city_name = "Istanbul, Turkey"
pop_1927= 691000
pop_2017 = 15029231

pop_change = pop_2017 - pop_1927
"""calculate growth percentage"""
percentage_gr = (pop_change/ pop_1927) * 100

annual_gr = percentage_gr / (2017- 1927)

def population_growth(year_one, year_two, population_one, population_two):
  pop_change = population_two - population_one
  percentage_gr = (pop_change / population_one) * 100
  
  growth_rate = percentage_gr / (year_two - year_one)
  
  return growth_rate

set_one = population_growth(1927, 2017, pop_1927, pop_2017)
print(set_one)

set_two = population_growth(1950, 2000, 983000, 8831800)
print(set_two)

report = "The change in population from 1927 to 2017 is large and ever growing. The difference in the growth is : " + str(pop_change) + " The annual growth rate is: " + str(annual_gr) + "."
print(report)
