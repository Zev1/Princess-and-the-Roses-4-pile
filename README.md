# Princess-and-the-Roses-4-pile
This contains the Sprague-Grundy values (nimbers) for the 4-pile variant of the combinatorial game Princess and the Roses. 

  The first step to finding these values was to reduce the 4-pile game to a 3-pile game. If A≥B≥C≥D≥0 are the sizes of the four piles, 
  then the game (D, B-C+D, A-C+D) with the following 7 moves has the same nimber as the original Princess and the Roses game:
  (-1, -1, -1),
  (-1, 0, 0),
  (-1, -2, -1),
  (-1, -1, -2),
  (0, -1, 0),
  (0, -1, -1),
  (0, 0, -1).
  These numbers are denoted as (x, y, z), with 0≤x≤y≤z.
  
The file positions_50.txt contains every position in this game up to and including (50, 50, 50), along with their Sprague-Grundy values. 
  They are ordered by increasing value of z, then y, then x.
  
The file positions_sorted_fancy.html contains the nimbers of every position in this game up to and including (50, 50, 50). The nimbers are sorted into pages 
  based on their x value. Each page contains a grid of y and z values, with each entry in the grid corresponding to the nimber of the position with the given 
  (x, y, z). Each page is split into 4 sections with different behaviour of the nimbers. 
    The upper section is white and green, and denotes positions where z<x+y and y≤2x+1. The green shows where exceptions may occurr, as this is the only region with many exceptions to its rules.
    The right section is red, and denotes positions where z<x+y and y>2x+1.
    The left section is red, and denotes positions where z≥x+y and y≤2x.
    The lower section is white, and denotes positions where z≥x+y and y>2x.
    Since this is an HTML file, it must be downloaded in order to be viewed without the source code. The file positions_sorted.txt contains the same content but without the colouring.
