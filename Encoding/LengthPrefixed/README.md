# Length Prefixed Encoding

Length Prefixed encoding stores multiple strings in a single string by storing
the length of each individual field before each fragment as a Unicode codepoint.

```
␃Cat␋Hello World     
╰──╯╰──────────╯     
                     
␃ ◀─ ETX - Unicode   
C    Code Point 3    
a                    
t    Field length = 3
```