def find_cargo_location():
    total_weight = 713
    box_weights = [200, 300, 213]
    cargo_locations = [0, 0, 0]

    while True:
        print("enter kilometer mark:")
        for i in range(3):
            try:
                cargo_locations[i] = int(input(f"box {i + 1}: "))
            except ValueError:
                print("Error! enter a valid integer.")
                return
            
        for i in range(3):
            cargo_locations[i] += i + 1

        print("Boxes have been moved. Checking the result...")

        if sum(box_weights) == total_weight:
            print("Congratulations! You have found all the boxes. The Martians thank you!")
            break
        else:
            print("Error! The total weight of the boxes is not 713 kg. Please re-enter.")
if __name__ == "__main__":
    print("Welcome to the Mars Cargo Recovery Program!")
    find cargo()
