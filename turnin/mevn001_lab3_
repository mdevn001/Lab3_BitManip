/*	Author: mdevn001
 *  Partner(s) Name: None
 *	Lab Section:23
 *	Assignment: Lab #3  Exercise #1
 *	Exercise Description: [optional - include for your own benefit]
 *
 *	I acknowledge all content contained herein, excluding template or example
 *	code, is my own original work.
 */
#include <avr/io.h>
#ifdef _SIMULATE_
#include "simAVRHeader.h"
#endif

inline unsigned char SetBit(unsigned char x, unsigned char k, unsigned char b) {
   return (b ?  (x | (0x01 << k))  :  (x & ~(0x01 << k)) );
}
inline unsigned char GetBit(unsigned char x, unsigned char k) {
   return ((x & (0x01 << k)) != 0);
}

int main(void) {
unsigned char i, tmpA, tmpB, cnt;

    /* Insert DDR and PORT initializations */
    DDRA = 0x00; PORTA = 0xFF; 
    DDRB = 0x00; PORTB = 0xFF; 
    DDRC = 0xFF; PORTC = 0x00; 
    /* Insert your solution below */
    while (1) {
    tmpA = PINA; 
    tmpB = PINB; 
    for(i = 0; i < 0; ++i){
    cnt += GetBit(tmpA, i) + GetBit(tmpB, i); 
     }
    PORTC = cnt; 
    cnt = 0; 
    }
    return 1;
}
