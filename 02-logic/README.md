<<<<<<< HEAD
# Lab 2: INSERT_YOUR_FIRSTNAME INSERT_YOUR_LASTNAME
=======
# Lab 2: Michal Kovář
>>>>>>> 5c699e422d747236632847729279f3daa78aacef

### 2-bit comparator

1. Karnaugh maps for other two functions of 2-bit comparator:

   Greater than:

<<<<<<< HEAD
   ![K-maps](images/kmap_empty.png)

   Less than:

   ![K-maps](images/kmap_empty.png)

2. Mark the largest possible implicants in the K-map and according to them, write the equations of simplified SoP (Sum of the Products) form of the "greater than" function and simplified PoS (Product of the Sums) form of the "less than" function.

   ![Logic functions](images/comparator_min.png)
=======
   ![KMgreater](https://user-images.githubusercontent.com/124684834/219866502-74dd2357-67f3-446b-bda0-fe35da690c1b.jpg)

   Less than:

   ![KMless](https://user-images.githubusercontent.com/124684834/219866520-fa198106-87c5-4b37-bbe0-55ac04388f9c.jpg)

2. Mark the largest possible implicants in the K-map and according to them, write the equations of simplified SoP (Sum of the Products) form of the "greater than" function and simplified PoS (Product of the Sums) form of the "less than" function.

   ![zacatek](https://user-images.githubusercontent.com/124684834/219866548-98060d37-4746-428c-a6a9-17d8a371043e.png)
>>>>>>> 5c699e422d747236632847729279f3daa78aacef

### 4-bit comparator

1. Listing of VHDL stimulus process from testbench file (`testbench.vhd`) with at least one assert (use BCD codes of your student ID digits as input combinations). Always use syntax highlighting, meaningful comments, and follow VHDL guidelines:

<<<<<<< HEAD
   Last two digits of my student ID: **xxxx??**
=======
   Last two digits of my student ID: **xxxx41**
>>>>>>> 5c699e422d747236632847729279f3daa78aacef

```vhdl
    p_stimulus : process
    begin
        -- Report a note at the beginning of stimulus process
<<<<<<< HEAD
        report "Stimulus process started" severity note;

        -- First test case
        s_b <= "BCD_OF_YOUR_SECOND_LAST_ID_DIGIT"; -- Such as "0101" if ID = xxxx56
        s_a <= "BCD_OF_YOUR_LAST_ID_DIGIT";        -- Such as "0110" if ID = xxxx56
        wait for 100 ns;
        -- Expected output
        assert ((s_B_greater_A = 'WRITE_CORRECT_VALUE_HERE') and
                (s_B_equals_A  = 'WRITE_CORRECT_VALUE_HERE') and
                (s_B_less_A    = 'WRITE_CORRECT_VALUE_HERE'))
=======
        report "Stimulus process started";

        -- First test case
        s_b <= "0100"; -- Such as "0100" if ID = xxxx41
        s_a <= "0001";        -- Such as "0001" if ID = xxxx41
        wait for 100 ns;
        -- Expected output
        assert ((s_B_greater_A = '1') and
                (s_B_equals_A  = '0') and
                (s_B_less_A    = '0'))
>>>>>>> 5c699e422d747236632847729279f3daa78aacef
        -- If false, then report an error
        report "Input combination COMPLETE_THIS_TEXT FAILED" severity error;

        -- Report a note at the end of stimulus process
<<<<<<< HEAD
        report "Stimulus process finished" severity note;
=======
        report "Stimulus process finished";
>>>>>>> 5c699e422d747236632847729279f3daa78aacef
        wait;
    end process p_stimulus;
```

2. Link to your public EDA Playground example:

<<<<<<< HEAD
   [https://www.edaplayground.com/...](https://www.edaplayground.com/...)
=======
   [https://www.edaplayground.com/x/SGZg](https://www.edaplayground.com/x/SGZg)
>>>>>>> 5c699e422d747236632847729279f3daa78aacef
