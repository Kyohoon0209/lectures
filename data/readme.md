#hw3
hairstyles = ["bouffant", "pixie", "dreadlocks", "crew", "bowl", "bob", "mohawk", "flattop"]
prices = [30, 25, 40, 20, 20, 35, 50, 35]
last_week = [2, 3, 5, 8, 4, 4, 6, 2]

total_price = 0
for price in prices:
    total_price += price

average_price = total_price / len(prices)
print("평균 가격은", average_price)

new_prices = [price - 5 for price in prices]
print(new_prices)

total_revenue = 0
for i in range(len(hairstyles)):
    total_revenue += prices[i] * last_week[i]

average_daily_revenue = total_revenue / 7
print("평균 하루 수익은", average_daily_revenue)

cuts_under_30 = [hairstyles[i] for i in range(len(new_prices)) if new_prices[i] < 30]
print(cuts_under_30)

# hw2
subjects = ["physics", "calculus", "poetry", "history"]
grades = [98, 97, 85, 88]

gradebook = [["physics", 98], ["calculus", 97], ["poetry", 85], ["history", 88]]

print(gradebook)

gradebook.append(["computer science", 100])
gradebook.append(["visual arts", 93])

gradebook[5][1] += 5

gradebook[2].remove(85)
gradebook[2].append("Pass")

last_semester_gradebook = [["politics", 80], ["latin", 96], ["dance", 97], ["architecture", 65]]
full_gradebook = last_semester_gradebook + gradebook

print(full_gradebook)

