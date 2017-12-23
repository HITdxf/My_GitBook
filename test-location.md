数学公式的测试

$$a \ne 0$$  
$$a \ne 0$$  
$$x^{y^z}=(1+{\rm e}^x)^{-2xy^w}$$  
$$f(x_1,x_2)=x_1^2+x_2^2$$

$$a \ne 0$$  
$$a \ne 0$$  
$$x^{y^z}=(1+{\rm e}^x)^{-2xy^w}$$  
$$f(x_1,x_2)=x_1^2+x_2^2$$

```
double myPow(double x, int n) {  
    //if (x == 0) return x;  
    if (n == 0) return 1.0;  
    //if (n == 1) return x;  
      
    if (n < 0)  
    {  
        if (n == INT_MIN)  
            return 1.0 / (myPow(x,INT_MAX) * x);   
        else  
            return 1.0 / myPow(x, -n);  
          
    }  
      
    double half = myPow(x, n>>1);  
    if (n % 2 == 0)  
        return half * half;  
    else  
        return half * half * x;  
}  
```



