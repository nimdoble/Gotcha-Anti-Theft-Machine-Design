First our lab 3 file, we first had to come up with the three inputs of D’s to input into our flip flops. 
How we did this was that we got our secret key value which was 11111111, then we created a state diagram 
on paper to show which input was mapped to which state and output. We were then able to create a state 
table then generate unique equations from this which we were able to implement into our circuit. We then 
created binary switches one to input a 1 into the diagram, one to input a 0 into the diagram, and the 
other to reset the inputs we inputted. We then mapped these inputs to a 16 bit lock and d flip flops. In 
the 16 bit lock we first map the reset input into the reset input into the lock to reset the lock and the 
inputs of 0 and 1 to the pulse to add our inputs to unlock the lock. Then with the d flip flops we map 
each of the next states to an output of and to check if all output to 1 to be able to pass the AND gate. 
Then we determine what the output is by comparing the output of the flip flops to the lock output to check 
if we have locked the lock or unlocked it.

In our next file Circuit3Part2, we essentially do the same hing as the first file we created. Where we 
create 3 different binary switches to input 0 and 1 and hard reset the inputs. Though with this we are 
using shift registers, created with d flip flops, to shift the binary bits as we input each bit. We then 
show the shifts in real time with hex displays. Instead of hard coding the password into the circuit we 
are using comparison to check if the input is correct. The hex keyboards are XNORed together with the 
input, this compares the value and if they all match, they will be ANDed together producing a 1 meaning 
the code is correct. We then need to AND the output with the 16bit lock to make sure we are not locked out. 
If we relate this to the real world, if the lock is unlocked and we have an output of 1 the motor will 
start. If the lock is locked but the output is 1, the car will not start. If the output is 0 it does not 
matter if the lock is locked or not, the motor will not start.

Lastly in the last file 16 bit lock, we create a lock that holds 16 digits. We do this by creating our pulse 
input and connecting it to our first d flip flop’s clock. Then each present state is mapped with each flip 
flop’s clock to give us a correct present state and next state. Then we create a reset input and attach to 
ach flip flop’s reset to reset our inputs. Finally the last d flip flop is connected to the previous next 
state's clock to give us our output’s present state, which is essentially our lock output. To check if our 
lock is locked or not.
