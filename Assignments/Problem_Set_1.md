Andrew Parsons

COMP 320 - A. Brady

3 April 2018

# PROBLEM SET 1

Chapters 1 and 2. Due Monday, 9 April 2018.

1. *Read over questions 6, 7, and 8 from the Problem Set questions at the end of Chapter 1. Choose one of them to answer. (3 pts)*

  - #4: *Java uses a right brace to mark the end of all compound statements. What are the arguments for and against this design?*

  This is covered in syntax design addressed on page 12. In that section the author asserts that simplicity and readability are sometimes at odds with one another.

  The C family of languages uses ```{ ... }``` to encapsulate many statements. This is fairly simple, but readability is both improved and damaged in using a right brace to mark the end of a compound statement.

  A primary but weak supporting argument for using the right brace instead of an ```end``` or similar convention is an acknowledgment of legacy. Because the C family of languages uses this brace syntax, readability is improved for new Java programmers with C-family familiarity. This however is only advantageous when a new Java programmer is comfortable with this syntax in the first place.

  Ignoring this gentle nod to predecessors and relatives, Java's ending brace adds another character, and depending on convention, another line to code. This makes the code challenging to read because exactly which compound statement the right brace ends is obscured. Consider the following code snipet:

  ```
  // some Java here
          }
        }
  // some more here
      }
    }
  }
  ```
  Identifying exactly which right brace corresponds with is--from experience--quite taxing when reading and writing many nested compound statements.

  Another point to consider is that different types of compound statements all use the same encapsulation syntax in Java. This means that a conditional ```if``` and a loop ```while``` will both terminate with ```}```. This is advantageous when considering writability, as a programmer needs only to remember that all compounds end uniformly instead of trying to recall the compound-specific endings.

  A simple trick for deeply nested code blocks is using comments to denote for which each ending brace stands.

  ```
  // some Java here
          } // end if-statement
        } // end for-loop
  // some more here
      }
    } // end while-loop
  }
  ```
  This however is laborious and just adds text to a code block, decreasing legibility. A more elegant solution is noted on page 12, where Fortran 95 and Ada use ```end if``` and ```end loop```. Such an implementation would look something like the following:

  ```
  // some code here
          END IF
        END FOR
  // some more here
      END WHILE
    END
  ```
  This is clearly more legibile, however rather laborious to write. Additionally, if Java were to implement the above, the compiler would need to reserve quite a few more words.

2. *Answer Problem Set question 10 from the end of Chapter 1. (4 pts)*

3. *Choose one of Problem Set questions 11, 12, 15, 17, or 18 from the end of Chapter 1 and answer it. (3 pts)*

4. *Answer Problem Set question 16 from the end of Chapter 1. (12 pts)*

5. *Answer questions 1, 6, and 7 from the Problem Set at the end of Chapter 2. (3 pts each, except #6, which is worth 2 pts)*
