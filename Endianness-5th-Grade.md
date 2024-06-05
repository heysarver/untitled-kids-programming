# Endianness

## How Your Birthday is Stored in a Computer

1. **Your Birthday Date:**
   - Your birthday is January 10, 1995.

2. **Convert Your Birthday to a Big Number:**
   - Computers use a special big number called a Unix timestamp to remember dates. For your birthday, this big number is `789091200`.
   - Computers store numbers as binary, 0s and 1s.  Humans use 0-9 for each digit (presumably because of 10 fingers).  In binary `789091200` is `00101111100001110010100000000000`

3. **Breaking Down the Big Number:**
   - Imagine the number `789091200` is like a long train with four cars (each car represents a byte in binary):
     - Car 1: `00101111` (2F in hexadecimal)
     - Car 2: `10001110` (8E in hexadecimal)
     - Car 3: `00101000` (28 in hexadecimal)
     - Car 4: `00000000` (00 in hexadecimal)

4. **Big Endian Order:**
   - In a big endian system, the train cars are arranged in the original order:
     - Car 1: `00101111` (2F in hexadecimal)
     - Car 2: `10001110` (8E in hexadecimal)
     - Car 3: `00101000` (28 in hexadecimal)
     - Car 4: `00000000` (00 in hexadecimal)
   - Some older systems, like the Motorola 68000 series used in the original Macintosh, use big endian. Many network protocols, like TCP/IP, also use big endian.

5. **Final Order:**
   - So, when the computer remembers your birthday in a big endian way, it looks like this:
     - `2F 8E 28 00`

So, when the computer stores your birthday, it uses the numbers `2F 8E 28 00` in the original order, which is called big endian.

6. **Little Endian Order:**
   - In a little endian system, the train cars are rearranged backwards:
     - Car 1: `00000000` (00 in hexadecimal)
     - Car 2: `00101000` (28 in hexadecimal)
     - Car 3: `10001110` (8E in hexadecimal)
     - Car 4: `00101111` (2F in hexadecimal)
   - Most PCs, including those running Windows, Linux, and macOS, use little endian for storing data.

7. **Final Order:**
   - So, when the computer remembers your birthday in a little endian way, it looks like this:
     - `00 28 8E 2F`

So, when the computer stores your birthday, it uses the numbers `00 28 8E 2F` in a special backwards way called little endian.
