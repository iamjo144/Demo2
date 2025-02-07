```markdown
# Prime Number Generator

This script generates prime numbers up to a specified limit.

```python
def is_prime(num):
    if num <= 1:
        return False
    for i in range(2, int(num**0.5) + 1):
        if num % i == 0:
            return False
    return True

def generate_primes(limit):
    primes = []
    for num in range(2, limit + 1):
        if is_prime(num):
            primes.append(num)
    return primes

# Example usage
limit = 50
print(f"Prime numbers up to {limit}: {generate_primes(limit)}")
```
```