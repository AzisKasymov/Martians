def find_cargo_location():
    total_weight = 713
    box_weights = [200, 300, 213]
    cargo_locations = [0, 0, 0]

    while True:
        print("Введите километровую отметку для каждого ящика:")
        for i in range(3):
            cargo_locations[i] = int(input(f"Ящик {i + 1}: "))
