#Code Explanation 


```
int main(void)
{
    volatile unsigned int i;
    WDTCTL = WDTPW + WDTHOLD;                 // Stop watchdog timer
    P1DIR |= 0x01;                            // Set P1.0 to output direction

    while(1)
    {
        P1OUT ^= 0x01;                        // Toggle P1.0 using exclusive-OR

        for (i=10000; i>0; i--);
  }
}
```

``volatile unsigned int i;`` : Is a designation of a varriable named i.


``WDTCTL = WDTPW + WDTHOLD;`` : Is used to stop the watchdog timer entirly. This is used to reset the code fucnality whne stuck in a state. 


``P1DIR |= 0x01;`` : Is used to set values in a variable. By using the OR functionailty it then saves the value into theP1DIR variable. 


``P1OUT ^= 0x01;`` : Is to XOR the value in the register with the value outside of the P1OUT. By odingso it toggles the current value to whatever its not in the sense of working if theres a 1 at all the result goes to zero and vice versa..

``for (i=10000; i>0; i--);`` : Then is to create a delay in the lgiht turning on/off to show a noticable diffrence for the human eye.




