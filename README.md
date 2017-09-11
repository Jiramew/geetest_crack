# 极验 geetest crack 2*3.0.0

**To ask a question please submit an issue or message.**

**Please kindly star the project before using it. ←v←**      

**Please kindly give credit to the original author when you use it elsewhere. →v→**



Focus on line 6132 in js file and the following code does some magic.  

You will know what is `str`,      
You will know what is `cList`,      
You will know what is `sString`. ^o^      

```{java}
private String newFunc(String str) {
        String m;
        int n = 0;
        String ss = str;
        int c0 = Integer.parseInt(this.cList[0]);
        int c2 = Integer.parseInt(this.cList[2]);
        int c4 = Integer.parseInt(this.cList[4]);
        for (int i = 0; i < 4; i++) {
            m = this.sString.substring(n, n + 2);
            n += 2;
            int k = Integer.parseInt(m, 16);
            String v = fromCharCode(k);
            int q = (c0 * k * k + c2 * k + c4) % str.length();
            ss = ss.substring(0, q) + v + ss.substring(q);
        }
        return ss;
    }
```
