# Checksum

This code is a simple 8-bit checksum algorithm written in MARIE Assembly Language; It verifies the correctness of a set of 4 bytes.
The sender receives the 4 bytes and calculates their 8-bit sum. MARIE uses a 16-bit
accumulator thus a mini loop was added to the code to discard the carry and simulate a 8-bit
sum. The sum is then used to calculate the checksum using two’s complement, which is sent to
the Receiver along with the 4 bytes. The Receiver performs the 8-bit sum of the bytes received.
The sample outputs show that when an incorrect byte is sent to the Receiver it displays a
non-zero number indicating an error. Otherwise, if the correct bytes are sent, the Receiver
outputs zero.
