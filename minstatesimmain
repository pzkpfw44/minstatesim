import random

class Citizen:
    def __init__(self, name, wealth, productivity, ideology):
        self.name = name
        self.wealth = wealth
        self.productivity = productivity
        self.ideology = ideology  # Libertarian, Conservative, Progressive, etc.

    def work(self):
        income = self.productivity * random.uniform(0.8, 1.2)
        self.wealth += income
        return income

    def trade(self, other):
        if self.wealth > 10 and other.wealth > 10:
            trade_value = min(self.wealth, other.wealth) * random.uniform(0.05, 0.15)
            self.wealth -= trade_value
            other.wealth += trade_value

class MinimalState:
    def __init__(self, tax_rate=0.1, public_services=['Security', 'Legal System']):
        self.tax_rate = tax_rate
        self.public_services = public_services
        self.state_funds = 0

    def collect_taxes(self, citizens):
        total_tax = 0
        for citizen in citizens:
            tax = citizen.wealth * self.tax_rate
            citizen.wealth -= tax
            self.state_funds += tax
            total_tax += tax
        return total_tax

    def provide_services(self):
        if self.state_funds > 100:
            self.state_funds -= 100  # Cost of maintaining minimal state services
            return "State provided essential security and legal framework."
        return "State funds too low for services."

# Simulation Setup
citizens = [
    Citizen("Alice", wealth=100, productivity=20, ideology="Libertarian"),
    Citizen("Bob", wealth=150, productivity=25, ideology="Conservative"),
    Citizen("Charlie", wealth=200, productivity=30, ideology="Progressive")
]

minimal_state = MinimalState()

# Run simulation for 10 rounds
for round in range(10):
    print(f"\n--- Round {round + 1} ---")
    for citizen in citizens:
        income = citizen.work()
        print(f"{citizen.name} worked and earned {income:.2f}, now has {citizen.wealth:.2f}")
    
    tax_collected = minimal_state.collect_taxes(citizens)
    print(f"State collected {tax_collected:.2f} in taxes. State funds: {minimal_state.state_funds:.2f}")
    print(minimal_state.provide_services())
