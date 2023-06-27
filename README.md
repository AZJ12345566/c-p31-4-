# c-p31-4-
C语言学习笔记 p31 数据的存储(4)
#include<stdio.h>
//此题接上一章笔记
//1.当想存一个浮点数时，首先转换二进制
//2.在看符号位 0为正数 -1为负数 - s1
//3.M表示有效数字>=1,<2
//4.2^E表示指数位
//公式：(-1)^S*M*2^E

//9.0
//1001.0
//(-1)^0*1.001*2^3
//(-s)^s*M    *2^E
int main()
{
    int n=9;
    float *pFloat=(float*)&n;
    printf("n的值为：%d\n",n);
    printf("*pFloat的值为：%f\n",*pFloat);

    *pFloat=9.0;
    printf("num的值为：%d\n",n);
    printf("*pFloat的值为：%f\n",*pFloat);
    return 0;
}

int main()
{
    float f=5.5;
    //5.5
    //101.1
    //(-1)^0*1.011*2^2
    //S=0
    //M=1.011
    //E=2
    //0100 0000 1011 0000 0000 0000 0000 0000
    //0x40b00000
    return 0;
}

//放进去一码事，取出来又是一码事
int main()
{
    
    return 0;
}
