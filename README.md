#ifndel LCM16X2_H
#define LCM16X2_H
#define BUSYFLAG 0x80
#define BLINK 0x01
#define NOBLINK 0x00
unsigned char LCMReadState(void);
void LCMDelay(int);
void LCMWriteCmd(unsigned char);
void LCMWriteData(unsigned char);
void LCMClear(void);
void LCMInit(void);
void LCMGotoXY(unsigned char,unsigned char);
void LCMDisplayChar(unsigned char,unsigned char,unsigned char);
void LCMDisplayString(unsigned char,unsigned char,unsigned char*);
void LCMBlink(unsigned char,unsigned char,unsigned char);
#endif
