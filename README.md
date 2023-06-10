# AIM
Design and simulate the logic diagram using Verilog.
F=(X+Y')(X'+Y)Z'
# THEORY
Product Of Sum:
i.) POS stands for Product of Sums.
ii.) It is a technique of defining boolean terms as a product of sum terms.
iii.) It prefers maxterms.
iv.) In the case of POS, the Maxterms are defined as ‘M’
v.) It gives LOW(0) output.
vi.) In POS, we can get the final term by multiplying the sum terms.
### K map:
A Karnaugh map (K-map) is a visual method used to simplify the algebraic expressions in Boolean functions without having to resort to complex theorems or equation manipulations. A K-map can be thought of as a special version of a truth table that makes it easier to map out parameter values and arrive at a simplified Boolean expression.
# LOGIC DIAGRAM

![240146928-3a659af7-c387-426b-a796-878caa16f364](https://github.com/Vasanthamukilan/Simulation-project--Digital-Electronics/assets/119559694/71c19ba7-5152-4030-804b-e5143574f729)

# PROGRAM
```
/* 
Name: LAAKSHIT D
Reg No:212222230071
*/
module assignment1 (x,y,z,f);
input x,y,z;
output f;
wire a,b,c,d,e;
not (a,x);
not (b,y);
not (c,z);
and (d,a,b,c);
and (e,x,y,c);
or (f,d,e);
endmodule
```
# NETLIST DIAGRAM

![Screenshot 2023-06-10 090136](https://github.com/Vasanthamukilan/Simulation-project--Digital-Electronics/assets/119559694/918766a5-94db-4202-a072-4bdbcf70c421)

# TIMING DIAGRAM

![Screenshot 2023-06-10 090532](https://github.com/Vasanthamukilan/Simulation-project--Digital-Electronics/assets/119559694/e93491c6-ceae-479c-88cc-194740663ee8)

# REFERENCE
https://www.electroniclinic.com/sop-and-pos-digital-logic-designing-with-solved-examples/
