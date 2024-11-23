# INST326_Project03_56_Group
Project 3

class Caregiver:
    def __init__(self, name, phone, email, pay_rate):
        self.name = name
        self.phone = phone
        self.email = email
        self.pay_rate = pay_rate
        self.hours = 0  # Total hours worked by the caregiver

    def __repr__(self):
        return (f"Caregiver(name={self.name}, phone={self.phone}, email={self.email}, "
                f"pay_rate={self.pay_rate}, hours={self.hours})")


class CaregiverManager:
    def __init__(self):
        self.caregivers = []

    def add_caregiver(self, name, phone, email, pay_rate):
        """Add a new caregiver to the system."""
        new_caregiver = Caregiver(name, phone, email, pay_rate)
        self.caregivers.append(new_caregiver)

    def update_hours(self, name, hours):
        """Update total hours worked for a specific caregiver."""
        for caregiver in self.caregivers:
            if caregiver.name == name:
                caregiver.hours += hours
                print(f"Updated hours for {name}: {caregiver.hours} hours")
                return
        print(f"Caregiver {name} not found!")

    def display_caregivers(self):
        """Display all caregivers and their details."""
        if not self.caregivers:
            print("No caregivers in the system.")
            return
        for caregiver in self.caregivers:
            print(caregiver)

    def remove_caregiver(self, name):
        """Remove a caregiver from the system."""
        for caregiver in self.caregivers:
            if caregiver.name == name:
                self.caregivers.remove(caregiver)
                print(f"Removed caregiver {name}")
                return
        print(f"Caregiver {name} not found!")


# Example usage
if __name__ == "__main__":
    manager = CaregiverManager()

    # Adding caregivers
    manager.add_caregiver("Alice Smith", "123-456-7890", "alice@example.com", 20)
    manager.add_caregiver("Bob Jones", "987-654-3210", "bob@example.com", 18)

    # Displaying caregivers
    print("\nCurrent Caregivers:")
    manager.display_caregivers()

    # Updating hours worked
    manager.update_hours("Alice Smith", 6)
    manager.update_hours("Bob Jones", 12)

    # Displaying caregivers after update
    print("\nUpdated Caregivers:")
    manager.display_caregivers()

    # Removing a caregiver
    manager.remove_caregiver("Alice Smith")

    # Displaying caregivers after removal
    print("\nFinal Caregivers:")
    manager.display_caregivers()
