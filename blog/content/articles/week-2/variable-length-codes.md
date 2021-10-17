---
title: 🔢  Variable Length Codes
tags: [compression, week-2]
layout: post
url: articles/variable-length-codes
author: Eduardo Flores
publishdate: 2021-10-17T13:36:00.000Z
summary: Understanding compression algorithms means understanding how humans view and use data.
---

Variable length codes are a form of compression that is used to reduce the size of data by storing the data in a smaller number of bits.

Once a code has been assigned to a symbol, no other code can start with that same pattern.

# Huffman Tree

Perhaps one of the most interesting things I learned this week was the Huffman tree. It's used to encode symbols in an efficient way.

You start with a table of symbols and their frequencies, you start with the table sorted in ascending order by frequency.
Then you take the last two elements of the table and combine them into a new symbol, which has those elements as children.
You continue to do this with all the symbols until you have a single symbol left and all nodes have childrens.

Next, you assign a 0 to the left branch and a 1 to the right branch of each node.

To determine the code for each symbol, you follow the path from the leaf to the root of the tree.
Let's take `ADNZ` with frequency of `2541` respectively.

- 0 is assigned to `/`
- 1 is assigned to `\`

```
   DNAZ
  0/ \1
   D  NAZ
      0/ \1
      N  AZ
        0/ \1
        A   Z
```
