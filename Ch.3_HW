# CITC_2375_01N
Homework/Projects for Internet Software Development class.
import math

# Constants
HOT_DOGS_PER_PACKAGE = 10
BUNS_PER_PACKAGE = 8
HOT_DOGS_PRICE_PER_PACKAGE = 3.49
BUNS_PRICE_PER_PACKAGE = 2.59
BUD_PRICE = 5.98

# Function to calculate required packages and leftovers
def calculate_packages_and_leftovers(people, hotdogs_per_person):
    total_hotdogs = people * hotdogs_per_person
    hotdog_packages = math.ceil(total_hotdogs / HOT_DOGS_PER_PACKAGE)
    buns_needed = total_hotdogs
    bun_packages = math.ceil(buns_needed / BUNS_PER_PACKAGE)
    hotdogs_leftover = (hotdog_packages * HOT_DOGS_PER_PACKAGE) - total_hotdogs
    buns_leftover = (bun_packages * BUNS_PER_PACKAGE) - buns_needed
    return hotdog_packages, bun_packages, hotdogs_leftover, buns_leftover

# Get user input
people = int(input("Enter the number of people attending the cookout: "))
hotdogs_per_person = int(input("Enter the number of hot dogs each person will be given: "))

# Calculate packages and leftovers
hotdog_packages, bun_packages, hotdogs_leftover, buns_leftover = calculate_packages_and_leftovers(people, hotdogs_per_person)

# Calculate total prices
hotdogs_total_price = hotdog_packages * HOT_DOGS_PRICE_PER_PACKAGE
buns_total_price = bun_packages * BUNS_PRICE_PER_PACKAGE

# Calculate total cost including beer
total_cost = hotdogs_total_price + buns_total_price + BUD_PRICE

# Display the results
print(f"a. Minimum number of hot dog packages required: {hotdog_packages}")
print(f"b. Minimum number of bun packages required: {bun_packages}")
print(f"c. Hot dogs leftover: {hotdogs_leftover}")
print(f"d. Buns leftover: {buns_leftover}")
print(f"e. Total price for hot dogs: ${hotdogs_total_price:.2f}")
print(f"f. Total price for hot dog buns: ${buns_total_price:.2f}")
print(f"g. Total cost including beer: ${total_cost:.2f}")
