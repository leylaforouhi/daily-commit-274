def calculate_median(numbers):
    if not numbers:
        return None

    ordered = sorted(numbers)
    middle = len(ordered) // 2

    if len(ordered) % 2 == 0:
        return (ordered[middle - 1] + ordered[middle]) / 2

    return ordered[middle]


if __name__ == "__main__":
    values = [12, 5, 19, 8, 14, 7]

    print("Values:", values)
    print("Median:", calculate_median(values))
