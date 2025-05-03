<h1 align='center'> Huffman Text File Zipper </h1>

This project implements **Huffman Coding**, a lossless compression algorithm to compress and decompress text files efficiently. Text files, such as `.txt`, `.html`, and `.css`, can be compressed to reduce size for easier storage and transfer.

## How It Works:
1. **Compression**: 
   - Creates a **Min Heap** of characters based on their frequencies.
   - Builds a **Huffman Tree** by combining nodes with the lowest frequencies.
   - Assigns shorter codes to frequent characters and longer codes to less frequent ones.
   - Saves the encoded file with `.huf` extension.

2. **Decompression**:
   - Reads the encoded file and reconstructs the **Huffman Tree**.
   - Traverses the tree to retrieve original characters and reconstruct the original file.

## Features:
- **Lossless Compression**: No data loss during compression or decompression.
- **Efficient**: Reduces file sizes for better storage and faster transmission.

### Usage:
To use the tool:
1. Create an instance of the `Huffman` class:  
   `huffman h(inputFileName, outputFileName)`
2. Call `compress()` to compress a text file.
3. Call `decompress()` to decompress a `.huf` file.

## References:
- [Huffman coding, WikiWorld](https://www.wikiwand.com/en/Huffman_coding)
- *Introduction to Algorithms* by Thomas H. Cormen et al.

