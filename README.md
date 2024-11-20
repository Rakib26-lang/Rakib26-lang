class Vehicle:
    def __init__(self, vehicle_id, vehicle_type, vehicle_capacity):
        self.vehicle_id = vehicle_id
        self.vehicle_type = vehicle_type
        self.vehicle_capacity = vehicle_capacity

class FleetManager:
    def __init__(self):
        self.vehicles = []

    def add_vehicle(self):
        vehicle_id = input("Enter Vehicle ID (e.g., V001): ")
        vehicle_type = input("Enter Vehicle Type (e.g., Truck, Van, Car): ")
        vehicle_capacity = int(input("Enter Vehicle Capacity (e.g., 1000 kg): "))

        new_vehicle = Vehicle(vehicle_id, vehicle_type, vehicle_capacity)
        self.vehicles.append(new_vehicle)
        print(f"Vehicle {vehicle_id} added successfully.")

# Example usage
if __name__ == "__main__":
    fleet_manager = FleetManager()
    fleet_manager.add_vehicle()
