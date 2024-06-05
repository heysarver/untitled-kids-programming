# Endianness

## How Your Birthday is Stored in a Computer

1. **Your Birthday Date:**
   - Your birthday is January 10, 1995.

2. **Convert Your Birthday to a Big Number:**
   - Computers use a special big number called a Unix timestamp to remember dates. For your birthday, this big number is `789091200`.

3. **Breaking Down the Big Number:**
   - Imagine the number `789091200` is like a long train with four cars:
     - Car 1: `00000000`
     - Car 2: `00111010`
     - Car 3: `00000111`
     - Car 4: `00101111`

4. **Little Endian Order:**
   - In a little endian system, the train cars are rearranged backwards:
     - Car 1: `00000000`
     - Car 2: `00111010`
     - Car 3: `00000111`
     - Car 4: `00101111`

5. **Final Order:**
   - So, when the computer remembers your birthday in a little endian way, it looks like this:
     - `00 3A 07 2F`

So, when the computer stores your birthday, it uses the numbers `00 3A 07 2F` in a special backwards way called little endian.

6. **Big Endian Order:**
   - In a big endian system, the train cars are arranged in the original order:
     - Car 1: `00000000`
     - Car 2: `00111010`
     - Car 3: `00000111`
     - Car 4: `00101111`

7. **Final Order:**
   - So, when the computer remembers your birthday in a big endian way, it looks like this:
     - `2F 07 3A 00`

So, when the computer stores your birthday, it uses the numbers `2F 07 3A 00` in the original order, which is called big endian.
