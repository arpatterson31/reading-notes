# Class Reading: Hash Tables

## Vocab terms and things I have learned

- **Hash:** ability to encode a key that will be mapped into a specific location in the hashtable

- **Buckets:** - what is contained in each index of the array of the hashtable

- **Collisions:** - when more than one key gets hashed to the same index in the hashtable

## Creating a Hash

- Hashtable is usually created from an array
- After the array is created, do some sort of logic to turn that "key" into a numeric number value (example: Add or multiply all the ASCII values together, Multiply it by a prime number such as 599, Use modulo to get the remainder of the result, when divided by the total size of the array, Insert into the array at that index)
- Each index of the array can hold many types of values
- Each index of the array contain “buckets”, and each of these “buckets” holds one key/value pair combination
- When there is no entry in a specific bucket, the buckets (each index of the array) all start null
- The hash table starts each bucket empty and overwrites their value once a key generates a hash code that corresponds with an index

## Storing Values

- accept a key
- calculate the hash of the key
- use modulus to convert the hash into an array index
- store the key with the value by appending both to the end of a linked list

## Reading Values

- accept a key
- calculate the hash of the key
- use modulus to convert the hash into an array index
- use the array index to access the short LinkedList representing a bucket
- search through the bucket looking for a node with a key/value pair that matches the key you were given
