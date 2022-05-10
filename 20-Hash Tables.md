## Hash Table

### What is a hash table?
A hash table is a data structure that uses a hash function to keep track of where data is put. Each piece of information to be stored has a name,
which is called a key. For example, a key might be a person's name. Each name is matched up to one piece of data called a value, like the person's
telephone number.

### What is the purpose of a hash table?
A hash table is a data structure that is used to store keys/value pairs. It uses a hash function to compute an index into an array in which an 
element will be inserted or searched. By using a good hash function, hashing can work well.

### structure 
Basically, a hash code turns a key into an integer. It’s very important that hash codes are deterministic: their output is determined only by their input. 
Hash codes should never have randomness to them. The same key should always produce the same hash code.

### creating a Hash
A hashtable traditionally is created from an array. I always like the size 1024. this is important for index placement. After you have created your array of
the appropriate size, do some sort of logic to turn that “key” into a numeric number value. Here is a possible suggestion:
Add or multiply all the ASCII values together.
Multiply it by a prime number such as 599.
Use modulo to get the remainder of the result, when divided by the total size of the array.
Insert into the array at that index.

Example:
```ruby 
Key = "Cat"
Value = "Josie"

67 + 97 + 116 = 280

280 * 599 = 69648

69648 % 1024 = 16

Key gets placed in index of 16. 
```
Each index of the array can hold many types of values. The trick is how the values are stored in comparison to efficiency. Each Index of the array contain “buckets”.
Each of these “buckets” holds one key/value pair combination. When there is no entry in a specific bucket, the buckets (each index of the array) all start null. 
The hash table starts each bucket empty and overwrites their value once a key generates a hashCode that corresponds with an index.
