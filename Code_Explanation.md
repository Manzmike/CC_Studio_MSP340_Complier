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

``volatile unsigned int i;`` : Is a designation of a varriable named i for counti



