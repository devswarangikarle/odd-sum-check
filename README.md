# odd-sum-check
On an island, people only use odd numbers and avoid even numbers. A man visits the island and tells them that he used k distinct positive odd numbers to build his boat. The people ask the man to give them the number n, and they want to determine if the number n can be represented as a sum of k distinct positive odd numbers or not.

def can_be_represented_as_sum(n, k):
    if n >= k * k and n % 2 == k % 2:
        return "YES"
    
    return "NO"

n, k = map(int, input().split())

result = can_be_represented_as_sum(n, k)
print(result)
