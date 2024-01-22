def factorize(n):
    # Start from 2 and try to divide the number
    for i in range(2, int(n ** 0.5) + 1):
        if n % i:
            continue
        return i, n // i
    return n, 1

def main():
    import sys
    if len(sys.argv) != 2:
        print(f"Usage: {sys.argv[0]} <file>")
        return

    filename = sys.argv[1]
    with open(filename, 'r') as f:
        for line in f:
            n = int(line.strip())
            p, q = factorize(n)
            print(f"{n}={p}*{q}")

if __name__ == "__main__":
    main()
