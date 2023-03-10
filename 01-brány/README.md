# Lab 1: Michal Kovář

### De Morgan's laws

1. Equations of all three versions of logic function f(c,b,a):

   ![obr1](https://user-images.githubusercontent.com/124684834/218272760-8a5f47b6-5d88-4aed-a16a-782dc53274d4.png)

2. Listing of VHDL architecture from design file (`design.vhd`) for all three functions. Always use syntax highlighting, meaningful comments, and follow VHDL guidelines:

```vhdl
architecture dataflow of gates is
begin
    f_orig_o <= (not(b_i) and a_i) or (c_i and not(b_i or not(a_i)));
    f_nand_o <= not(not(a_i and not(b_i)) and not(c_i and not(b_i) and a_i));
    f_nor_o  <= not(b_i or not(a_i)) or not(not(c_i) or (b_i or not(a_i)));  
end architecture dataflow;
```

3. Complete table with logic functions' values:

   | **c** | **b** |**a** | **f_ORIG** | **f_(N)AND** | **f_(N)OR** |
   | :-: | :-: | :-: | :-: | :-: | :-: |
   | 0 | 0 | 0 | 0 | 0 | 0 |
   | 0 | 0 | 1 | 1 | 1 | 1 |
   | 0 | 1 | 0 | 0 | 0 | 0 |
   | 0 | 1 | 1 | 0 | 0 | 0 |
   | 1 | 0 | 0 | 0 | 0 | 0 |
   | 1 | 0 | 1 | 1 | 1 | 1 |
   | 1 | 1 | 0 | 0 | 0 | 0 |
   | 1 | 1 | 1 | 0 | 0 | 0 |

### Distributive laws
![obr3](https://user-images.githubusercontent.com/124684834/218272987-e602cba8-6d23-453e-a559-e9c9fb125d34.png)
1. Screenshot with simulated time waveforms. Always display all inputs and outputs (display the inputs at the top of the image, the outputs below them) at the appropriate time scale!

   ![obr2](https://user-images.githubusercontent.com/124684834/218272895-609bd387-2642-4567-9260-0418cc607567.png)

2. Link to your public EDA Playground example:

   [https://www.edaplayground.com/x/6iHe](https://www.edaplayground.com/x/6iHe)
